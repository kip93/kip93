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
* ➡️ Pushed 1099 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#e4999e3](https://github.com/OroraTech/nixpkgs/commit/e4999e3) bitwarden: remove unused patch
  * [#97c12ac](https://github.com/OroraTech/nixpkgs/commit/97c12ac) python312Packages.urwid-readline: 0.13 -&gt; 0.14

Diff: https://github.com/rr-/urwid_readline/compare/refs/tags/0.13...0.14
  * [#2e312bb](https://github.com/OroraTech/nixpkgs/commit/2e312bb) python312Packages.urwid-readline: refactor
  * [#00be299](https://github.com/OroraTech/nixpkgs/commit/00be299) imagemagick: 7.1.1-28 -&gt; 7.1.1-29

Diff: https://github.com/ImageMagick/ImageMagick/compare/7.1.1-28...7.1.1-29

Changelog: https://github.com/ImageMagick/Website/blob/main/ChangeLog.md
  * [#524a9ec](https://github.com/OroraTech/nixpkgs/commit/524a9ec) live555: 2024.02.15 -&gt; 2024.02.23
  * [#5135272](https://github.com/OroraTech/nixpkgs/commit/5135272) live555: 2023.11.30 -&gt; 2024.02.15
  * [#5a56dbf](https://github.com/OroraTech/nixpkgs/commit/5a56dbf) edbrowse: enable Unix ODBC support
  * [#7659f7b](https://github.com/OroraTech/nixpkgs/commit/7659f7b) edbrowse: refactor

- finalAttrs design pattern
- get rid of nested with
- substitute vrthra to AndersonTorres on meta.maintainers
  * [#98802aa](https://github.com/OroraTech/nixpkgs/commit/98802aa) edbrowse: migrate to by-name
  * [#043c254](https://github.com/OroraTech/nixpkgs/commit/043c254) gegl: 0.4.46 → 0.4.48
  * [#3b0e6fc](https://github.com/OroraTech/nixpkgs/commit/3b0e6fc) fm-go: init at 0.16.0
  * [#83e0914](https://github.com/OroraTech/nixpkgs/commit/83e0914) python311Packages.cachecontrol: add dotlambda to maintainers
  * [#36cd3b4](https://github.com/OroraTech/nixpkgs/commit/36cd3b4) python311Packages.cachecontrol: 0.13.1 -&gt; 0.14.0

Diff: https://github.com/ionrock/cachecontrol/compare/refs/tags/v0.13.1...v0.14.0

Changelog: https://github.com/psf/cachecontrol/releases/tag/v0.14.0
  * [#afaaaef](https://github.com/OroraTech/nixpkgs/commit/afaaaef) flottbot: 0.13.0 -&gt; 0.13.1
  * [#b7db650](https://github.com/OroraTech/nixpkgs/commit/b7db650) python311Packages.llama-index-embeddings-openai: init at 0.10.12
  * [#f691d8d](https://github.com/OroraTech/nixpkgs/commit/f691d8d) python311Packages.llama-index-multi-modal-llms-openai: init 0.10.12
  * [#d2fb7e1](https://github.com/OroraTech/nixpkgs/commit/d2fb7e1) python311Packages.llama-index-program-openai: init at 0.10.12
  * [#1332bc4](https://github.com/OroraTech/nixpkgs/commit/1332bc4) python311Packages.llama-index-agent-openai: init at 0.10.12
  * [#9bf729a](https://github.com/OroraTech/nixpkgs/commit/9bf729a) python311Packages.llama-index-llms-openai: init at 0.10.12
  * [#1ab2a11](https://github.com/OroraTech/nixpkgs/commit/1ab2a11) python311Packages.llama-index-readers-file: init at 0.10.12
  * *On 1 Mar 2024, 15:54:18*
* ➡️ Pushed 6394 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#38e2e00](https://github.com/OroraTech/nixpkgs/commit/38e2e00) Merge pull request #290703 from r-ryantm/auto-update/werf

werf: 1.2.292 -&gt; 1.2.294
  * [#4208934](https://github.com/OroraTech/nixpkgs/commit/4208934) python312Packages.botocore-stubs: 1.34.48 -&gt; 1.34.49
  * [#1ce0f9b](https://github.com/OroraTech/nixpkgs/commit/1ce0f9b) python311Packages.boto3-stubs: 1.34.48 -&gt; 1.34.49
  * [#abd34e0](https://github.com/OroraTech/nixpkgs/commit/abd34e0) obs-studio-plugins.obs-3d-effect: 0.0.2 -&gt; 0.1.0
  * [#23fcd51](https://github.com/OroraTech/nixpkgs/commit/23fcd51) ayatana-indicator-session: Re-enable test-service test
  * [#e9dcfb3](https://github.com/OroraTech/nixpkgs/commit/e9dcfb3) Merge #291106: opencolorio: fix tests on staging-next
  * [#2b0673c](https://github.com/OroraTech/nixpkgs/commit/2b0673c) opencolorio: fix tests on staging-next
  * [#85a7517](https://github.com/OroraTech/nixpkgs/commit/85a7517) Merge pull request #291058 from r-ryantm/auto-update/fishPlugins.forgit

fishPlugins.forgit: 24.01.0 -&gt; 24.02.0
  * [#7d52ac6](https://github.com/OroraTech/nixpkgs/commit/7d52ac6) python311Packages.dask: provide dataframe extra for tests

Tests would previously error out with:

&gt; ImportError: Dask dataframe requirements are not installed.
  * [#088e4ab](https://github.com/OroraTech/nixpkgs/commit/088e4ab) broot: 1.33.1 -&gt; 1.34.0

https://github.com/Canop/broot/releases/tag/v1.34.0
  * [#d01044e](https://github.com/OroraTech/nixpkgs/commit/d01044e) zabbix40: drop, no more supported upstream

Security/limited support ended in October 2023.

https://www.zabbix.com/life_cycle_and_release_policy
  * [#a65967a](https://github.com/OroraTech/nixpkgs/commit/a65967a) nixos/nix: documentation: fix outdated reference to /etc/nix.conf
  * [#8e8148f](https://github.com/OroraTech/nixpkgs/commit/8e8148f) git-absorb: 0.6.11 -&gt; 0.6.12

Diff: https://github.com/tummychow/git-absorb/compare/refs/tags/0.6.11...0.6.12
  * [#d743b7f](https://github.com/OroraTech/nixpkgs/commit/d743b7f) Merge pull request #291095 from r-ryantm/auto-update/vdrPlugins.softhddevice

vdrPlugins.softhddevice: 2.0.9 -&gt; 2.1.1
  * [#bf289c8](https://github.com/OroraTech/nixpkgs/commit/bf289c8) hugo: 1.123.2 -&gt; 1.123.3

https://github.com/gohugoio/hugo/releases/tag/v0.123.3
  * [#ef22d82](https://github.com/OroraTech/nixpkgs/commit/ef22d82) linuxPackages.r8168: 8.048.03 -&gt; 8.052.01
  * [#50f953b](https://github.com/OroraTech/nixpkgs/commit/50f953b) cri-o: 1.29.1 -&gt; 1.29.2

Update pkgs/applications/virtualization/cri-o/default.nix

Co-authored-by: Pol Dellaiera &lt;pol.dellaiera@protonmail.com&gt;
  * [#4d6c7b9](https://github.com/OroraTech/nixpkgs/commit/4d6c7b9) Merge pull request #291083 from r-ryantm/auto-update/obs-studio-plugins.obs-shaderfilter

obs-studio-plugins.obs-shaderfilter: 2.0.0 -&gt; 2.2.2
  * [#126adb6](https://github.com/OroraTech/nixpkgs/commit/126adb6) Merge pull request #291022 from r-ryantm/auto-update/libretro.genesis-plus-gx

libretro.genesis-plus-gx: unstable-2024-02-16 -&gt; unstable-2024-02-23
  * [#0e1cb44](https://github.com/OroraTech/nixpkgs/commit/0e1cb44) Merge pull request #291019 from r-ryantm/auto-update/libretro.gambatte

libretro.gambatte: unstable-2024-02-09 -&gt; unstable-2024-02-23
  * *On 27 Feb 2024, 23:15:49*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 2 Mar 2024, 03:47:37 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
