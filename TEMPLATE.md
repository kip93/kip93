<!-- README template, populated using this action:
     https://github.com/kip93/kip93/blob/main/.github/workflows/readme.yml. -->

<h1 align="center">👋 Hello world! I'm @{{ LOGIN }}</h1> <!-- LOGIN => username -->

### 👤 About me

I am a passionate self-taught backend software developer, and a strong advocate for libre software.


### 💬 Some facts

* 📅 Coding since 2013.
* 💼 Currently working @ [OroraTech](https://ororatech.com/).
* 👨‍💻 [Python](https://github.com/search?q=user%3A{{ LOGIN }}&l=python) is ❤️. <!-- LOGIN => username -->
* 💻 [NixOS](https://github.com/NixOS/) /
     [Awesome](https://github.com/awesomeWM/) /
     [kitty](https://github.com/kovidgoyal/kitty/) /
     [xonsh](https://github.com/xonsh/).
* 🌐 I have a [portfolio website](https://kip93.net/) with some more information.
* 📝 Checkout my [résumé](https://kip93.net/resume/) for even more detail.
* 📫 Reach me @ [leandro@kip93.net](mailto:leandro@kip93.net).
* 🎲 Fun fact: My first program was not a "Hello World" (it was simple R/W in an [HC11 µC](https://en.wikipedia.org/wiki/68HC11) emulator).


-----------------------------------------------------------------------------------------------------------------------


### 📈 Stats

![](./stats.svg)


### 📚 Most used languages <!-- by percentage, in decreasing order -->

![](./languages.svg)


### 🏅 Achievements

![](./achievements.svg)


<details> <!-- Last activity -->
<!-- Almost verbatim copy of https://github.com/lowlighter/metrics/blob/latest/source/templates/markdown/partials/activity.ejs, but restructured to be foldable. -->
<summary><h3>📰 Recent activity</h3></summary>

<%_ if (plugins.activity.error) { _%>
    <%= plugins.activity.error.message _%>
<%_ } else if (plugins.activity.events.length) { _%>
    <%_ for (const {actor, type, repo, timestamp, ...event} of plugins.activity.events) { _%>
        <%_ if (type === "comment") { _%>
* 💬 Commented on [#<%= event.number %> <%= event.title %>](https://github.com/<%= repo %>/<%= {issue:"issues", pr:"pull", commit:"commit"}[event.on] %>/<%= event.number %>) from [<%= repo %>](https://github.com/<%= repo %>)
        <%_ } else if (type === "member") { _%>
* 💼 Added [<%= event.user %>](https://github.com/<%= event.user %>) as collaborator in [<%= repo %>](https://github.com/<%= repo %>)
        <%_ } else if (type === "star") { _%>
* 🌟 Starred [<%= repo %>](https://github.com/<%= repo %>)
        <%_ } else if (type === "release") { _%>
* 📦 <%- event.draft ? "Drafted release" : event.prerelease ? "Pre-released" : "Released" %> **<%= event.name %>** of [<%= repo %>](https://github.com/<%= repo %>)
        <%_ } else if (type === "fork") { _%>
* 🍽️ Forked [<%= repo %>](https://github.com/<%= repo %>) to [<%= event.forked %>](https://github.com/<%= event.forked %>)
        <%_ } else if (type === "push") { _%>
* ➡️ Pushed <%= event.size %> commit<%= s(event.size) %> in [<%= repo %>](https://github.com/<%= repo %>) <%= event.branch ? `on branch \`${event.branch}\`` : "" %>
                <%_ for (const commit of event.commits) { _%>
  * [#<%= commit.sha %>](https://github.com/<%= repo %>/commit/<%= commit.sha %>) <%= commit.message %>
                <%_ } _%>
        <%_ } else if (type === "issue") { _%>
* #️⃣ <%- event.action === "opened" ? "Opened" : event.action === "reopened" ? "Reopened" : "Closed" %> [#<%= event.number %> <%= event.title %>](https://github.com/<%= repo %>/issues/<%= event.number %>) in [<%= repo %>](https://github.com/<%= repo %>)
        <%_ } else if (type === "pr") { _%>
* 🔃 <%- event.action === "opened" ? "Opened" : event.action === "merged" ? "Merged" : "Closed" %> [#<%= event.number %> <%= event.title %>](https://github.com/<%= repo %>/pull/<%= event.number %>) in [<%= repo %>](https://github.com/<%= repo %>)
                * <%= event.files.changed %> file<%= s(event.files.changed) %> changed `++<%= event.lines.added %> --<%= event.lines.deleted%>`
        <%_ } else if (type === "wiki") { _%>
* 📝 Updated <%= event.pages.length %> wiki page<%= s(event.pages.length) %> in [<%= repo %>](https://github.com/<%= repo %>/wiki)
            <%_ for (const page of event.pages) { _%>
  * <%= page %>
            <%_ } _%>
        <%_ } else if (type === "public") { _%>
  * 🚀 Made [<%= repo %>](https://github.com/<%= repo %>) public
        <%_ } else if (type === "review") { _%>
* 🔍 Reviewed [#<%= event.number %> <%= event.title %>](https://github.com/<%= repo %>/pull/<%= event.number %>) in [<%= repo %>](https://github.com/<%= repo %>)
        <%_ } else if (type === "ref/create") { _%>
* ⏺️ Created new <%= event.ref.type %> <%= event.ref.type !== "repository" ? `${event.ref.name} in` : "" %> [<%= repo %>](https://github.com/<%= repo %>)
        <%_ } else if (type === "ref/create") { _%>
* 🚮 Deleted <%= event.ref.type %> `<%= event.ref.name %>` from [<%= repo %>](https://github.com/<%= repo %>)
        <%_ } _%>
        <%_ if (plugins.activity.timestamps) { _%>
  * *On <%= f.date(timestamp, {time:true, date:true, timeZone:config.timezone?.name}) %>*
        <%_ } _%>
    <%_ } _%>
<%_ } else { _%>
    No recent activity
<%_ } _%>
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v{{ VERSION }}</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ {{ meta.generated }} / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
