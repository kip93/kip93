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

* ➡️ Pushed 368 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#026179d](https://github.com/OroraTech/nixpkgs/commit/026179d) vtm: 0.9.9t -&gt; 0.9.9u

Diff: https://github.com/netxs-group/vtm/compare/v0.9.9t...v0.9.9u
  * [#b4a0a97](https://github.com/OroraTech/nixpkgs/commit/b4a0a97) ArchiSteamFarm: 5.4.8.3 -&gt; 5.4.9.3
  * [#32371a3](https://github.com/OroraTech/nixpkgs/commit/32371a3) timoni: add update script
  * [#3da98e6](https://github.com/OroraTech/nixpkgs/commit/3da98e6) pferd: 3.4.3 -&gt; 3.5.0
  * [#43555b3](https://github.com/OroraTech/nixpkgs/commit/43555b3) mfoc-hardnested: unstable-2021-08-14 -&gt; unstable-2023-03-27

- Migrate to by-name hierarchy
- Use the finalAttrs pattern for easier overrides
- Fix build on aarch64-darwin
  * [#4f461f7](https://github.com/OroraTech/nixpkgs/commit/4f461f7) nixos/modules/system/resolved: disable DNSSEC validation by default

Historically, we allowed downgrade of DNSSEC, but some folks argue
this may decrease actually the security posture to do opportunistic DNSSEC.

In addition, the current implementation of (opportunistic) DNSSEC validation
is broken against &#34;in the wild&#34; servers which are usually slightly non-compliant.

systemd upstream recommended to me (in personal communication surrounding
the All Systems Go 2023 conference) to disable DNSSEC validation until
they work on it in a significant capacity, ideally, by next year.
  * [#d811965](https://github.com/OroraTech/nixpkgs/commit/d811965) musikcube: 3.0.1 -&gt; 3.0.2

remove with lib
  * [#8ff38d7](https://github.com/OroraTech/nixpkgs/commit/8ff38d7) scala_3: 3.3.0 -&gt; 3.3.1
  * [#fa7ea4f](https://github.com/OroraTech/nixpkgs/commit/fa7ea4f) scala_2_13: 2.13.11 -&gt; 2.13.12
  * [#babf61b](https://github.com/OroraTech/nixpkgs/commit/babf61b) wasmer: 4.1.2 -&gt; 4.2.0

Diff: https://github.com/wasmerio/wasmer/compare/refs/tags/v4.1.2...v4.2.0
  * [#66a5b62](https://github.com/OroraTech/nixpkgs/commit/66a5b62) wasmer: 4.1.1 -&gt; 4.1.2

Diff: https://github.com/wasmerio/wasmer/compare/refs/tags/v4.1.1...v4.1.2
  * [#399f01d](https://github.com/OroraTech/nixpkgs/commit/399f01d) wasmer: 4.0.0 -&gt; 4.1.1

Diff: https://github.com/wasmerio/wasmer/compare/refs/tags/v4.0.0...v4.1.1
  * [#456ce8d](https://github.com/OroraTech/nixpkgs/commit/456ce8d) jetbrains: fix darwin errors on macOS 13

As the jetbrains products have notarized binaries no further post processing is required more about this can be found in https://github.com/NixOS/nixpkgs/commit/3ea22dab7d906f400cc5983874dbadeb8127c662
  * [#227a75a](https://github.com/OroraTech/nixpkgs/commit/227a75a) python311Packages.aliyun-python-sdk-kms: 2.16.1 -&gt; 2.16.2

Changelog: https://github.com/aliyun/aliyun-openapi-python-sdk/blob/master/aliyun-python-sdk-kms/ChangeLog.txt
  * [#6be969d](https://github.com/OroraTech/nixpkgs/commit/6be969d) xorg: add meta.mainProgram to various utilities

See #246386
  * [#c44396d](https://github.com/OroraTech/nixpkgs/commit/c44396d) mergerfs: 2.36.0 -&gt; 2.37.0
  * [#f453cea](https://github.com/OroraTech/nixpkgs/commit/f453cea) python311Packages.libpcap: init at 1.11.0b7
  * [#930d246](https://github.com/OroraTech/nixpkgs/commit/930d246) optipng: Use libpng instead of libpng-1.2
  * [#8985e49](https://github.com/OroraTech/nixpkgs/commit/8985e49) python311Packages.aws-sam-translator: 1.73.0 -&gt; 1.74.0

Diff: https://github.com/aws/serverless-application-model/compare/refs/tags/v1.73.0...v1.74.0

Changelog: https://github.com/aws/serverless-application-model/releases/tag/v1.74.0
  * [#2f57513](https://github.com/OroraTech/nixpkgs/commit/2f57513) pgrok: 1.3.4 -&gt; 1.4.0

https://github.com/pgrok/pgrok/releases/tag/v1.4.0
  * *On 19 Sept 2023, 08:39:39*
* ➡️ Pushed 2 commits in [nixcon/NixConContent](https://github.com/nixcon/NixConContent) on branch `main`
  * [#d46873f](https://github.com/nixcon/NixConContent/commit/d46873f) Merge pull request #21 from zmitchell/zmitchell-nixcon-slides

Add zmitchell slides
  * [#9fc9472](https://github.com/nixcon/NixConContent/commit/9fc9472) Add slides
  * *On 19 Sept 2023, 08:22:36*
* 🔃 Merged [#21 Add zmitchell slides](https://github.com/nixcon/NixConContent/pull/21) in [nixcon/NixConContent](https://github.com/nixcon/NixConContent)
                * 1 file changed `++0 --0`
  * *On 19 Sept 2023, 08:22:35*
* ➡️ Pushed 1 commit in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `feature/add-pycyphal`
  * [#7b13a35](https://github.com/OroraTech/nixpkgs/commit/7b13a35) python311Packages.pyuavcan: add deprecation warning
  * *On 19 Sept 2023, 08:01:09*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 19 Sept 2023, 08:48:25 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
