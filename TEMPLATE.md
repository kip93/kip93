<!-- README template, populated using this https://github.com/kip93/kip93/blob/main/.github/workflows/readme.yml. -->

<h1 align="center">👋 Hello world! I'm @{{ LOGIN }}</h1> <!-- LOGIN => username -->

### 👤 About me

I am a passionate self-taught backend software developer, and a strong advocate for libre software.

### 💬 Some facts

* 📅 Coding since 2013.
* 💼 Currently working @ [MuleSoft](https://github.com/mulesoft/).
* 👨‍💻 [Python](https://github.com/search?q=user%3A{{ LOGIN }}&l=python) is ❤️. <!-- LOGIN => username -->
* 💻 [NixOS](https://github.com/NixOS/) / [Awesome](https://github.com/awesomeWM/) / [kitty](https://github.com/kovidgoyal/kitty/) / [xonsh](https://github.com/xonsh/).
* 🌐 I have a [portfolio website](https://kip93.net/) with some more information.
* 📝 Checkout my [résumé](https://kip93.net/resume/) for even more detail.
* 📫 Reach me @ [leandro.kip93@gmail.com](mailto:leandro.kip93@gmail.com).
* 🎲 Fun fact: My first line of code was not a "Hello World".

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### 📈 Stats

![](./stats.svg)

### 📚 Most used languages <!-- by percentage, in decreasing order -->

![](./languages.svg)

### 🏅 Achievements

![](./achievements.svg)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<%- await include(`partials/activity.ejs`) %> <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v{{ VERSION }}</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ {{ meta.generated }} / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
