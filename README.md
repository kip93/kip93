<!-- README template, populated using this action:
     https://github.com/kip93/kip93/blob/main/.github/workflows/readme.yml. -->

<h1 align="center">👋 Hello world! I'm @kip93</h1> <!-- LOGIN => username -->

### 👤 About me

I am a passionate self-taught backend software developer, and a strong advocate for libre software.


### 💬 Some facts

* 📅 Coding since 2013.
* 💼 Currently working @ [OroraTech](https://ororatech.com/).
* 👨‍💻 [Python](https://github.com/search?q=user%3Akip93&l=python) is ❤️. <!-- LOGIN => username -->
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

* ⏺️ Created new branch chore/calibre-web-ldap in [kip93/nixpkgs](https://github.com/kip93/nixpkgs)
  * *On 3 Mar 2024, 12:53:12*
* 🔃 Opened [#293002 python311Packages.flask-simpleldap: init at 1.4.0](https://github.com/NixOS/nixpkgs/pull/293002) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
                * 2 files changed `++40 --0`
  * *On 3 Mar 2024, 12:42:34*
* ⏺️ Created new branch chore/add-flask-simpleldap in [kip93/nixpkgs](https://github.com/kip93/nixpkgs)
  * *On 1 Mar 2024, 17:53:33*
* ➡️ Pushed 10000 commits in [kip93/nixpkgs](https://github.com/kip93/nixpkgs) on branch `master`
  * [#b2c10ff](https://github.com/kip93/nixpkgs/commit/b2c10ff) _1password: 2.24.0 -&gt; 2.25.0
  * [#27d6c24](https://github.com/kip93/nixpkgs/commit/27d6c24) nixos/networkd: accept `true` and `false` in addition to &#34;yes&#34; and &#34;no&#34; for DHCP= and LinkLocalAddressing=

These were the only two systemd configuration values that were missing the `boolValues ++` treatment, according to my `rg` through the codebase.
  * [#fc1b3a1](https://github.com/kip93/nixpkgs/commit/fc1b3a1) Merge pull request #290875 from fabaff/msal-bump

python311Packages.msal: 1.26.0 -&gt; 1.27.0
  * [#8078fb9](https://github.com/kip93/nixpkgs/commit/8078fb9) cryptomator: 1.11.1 -&gt; 1.12.3

Changelogs:

 - https://github.com/cryptomator/cryptomator/releases/tag/1.12.0
 - https://github.com/cryptomator/cryptomator/releases/tag/1.12.1
 - https://github.com/cryptomator/cryptomator/releases/tag/1.12.2
 - https://github.com/cryptomator/cryptomator/releases/tag/1.12.3
  * [#e64acf5](https://github.com/kip93/nixpkgs/commit/e64acf5) Merge pull request #291863 from fabaff/botocore-stubs-bump

python312Packages.botocore-stubs: 1.34.49 -&gt; 1.34.50
  * [#4d59ace](https://github.com/kip93/nixpkgs/commit/4d59ace) nixos/systemd-repart: add assertion for partition label length

The maximum length for a GPT label supported by systemd is 36
characters. When a repart definition contains a label that is longer
than the supported maximum length, it is ignored by systemd-repart and
a log message is produced.

The new assertion makes this obvious to the user at evaluation time,
allowing them to either drop the property entirely or choose a supported
label within the length limit instead.
  * [#6a14736](https://github.com/kip93/nixpkgs/commit/6a14736) python311Packages.llama-index-readers-json: init at 0.1.2
  * [#b1778d1](https://github.com/kip93/nixpkgs/commit/b1778d1) python311Packages.llama-index-readers-weather: init at 0.1.4
  * [#efe56d4](https://github.com/kip93/nixpkgs/commit/efe56d4) python311Packages.llama-index-embeddings-gemini: init at 0.1.3
  * [#de62316](https://github.com/kip93/nixpkgs/commit/de62316) python311Packages.llama-index-embeddings-google: init at 0.10.12
  * [#c93425a](https://github.com/kip93/nixpkgs/commit/c93425a) python311Packages.clarifai: 9.11.1 -&gt; 10.1.0

Diff: https://github.com/Clarifai/clarifai-python/compare/refs/tags/9.11.1...10.1.0

Changelog: https://github.com/Clarifai/clarifai-python/releases/tag/10.1.0
  * [#82f4c29](https://github.com/kip93/nixpkgs/commit/82f4c29) python311Packages.llama-index: init at 0.10.12
  * [#7756292](https://github.com/kip93/nixpkgs/commit/7756292) python311Packages.llama-index-question-gen-openai: init at 0.10.12
  * [#56f960b](https://github.com/kip93/nixpkgs/commit/56f960b) python311Packages.llama-index-legacy: init at 0.10.12
  * [#5753976](https://github.com/kip93/nixpkgs/commit/5753976) python311Packages.llama-index-indices-managed-llama-cloud: init at 0.10.12
  * [#d1599c2](https://github.com/kip93/nixpkgs/commit/d1599c2) python311Packages.llama-index-cli: init at 0.10.12
  * [#9b319de](https://github.com/kip93/nixpkgs/commit/9b319de) python311Packages.llama-index-vector-stores-chroma: init at 0.10.12
  * [#a2a7cdd](https://github.com/kip93/nixpkgs/commit/a2a7cdd) python311Packages.chromadb: init at 0.4.23

The AI-native open-source embedding database

https://github.com/chroma-core/chroma
  * [#bfd8bf5](https://github.com/kip93/nixpkgs/commit/bfd8bf5) python311Packages.pulsar-client: init at 3.4.0

https://pypi.org/project/pulsar-client/
  * [#681d70b](https://github.com/kip93/nixpkgs/commit/681d70b) python311Packages.opentelemetry-instrumentation-fastapi: init at 0.43b0
  * *On 1 Mar 2024, 17:47:08*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 3 Mar 2024, 13:47:44 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
