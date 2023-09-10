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


-----------------------------------------------------------------------------------------------------------------------


**[📰 Recent activity](https://github.com/kip93)**
* ➡️ Pushed 144 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `chore/fix-sphinx-hook`
  * [#75900df](https://github.com/OroraTech/nixpkgs/commit/75900df) ocamlPackages.awa: remove spurious dependency
  * [#652837d](https://github.com/OroraTech/nixpkgs/commit/652837d) freerdpUnstable: 2.11.0 -&gt; 2.11.1
  * [#046eca9](https://github.com/OroraTech/nixpkgs/commit/046eca9) frugal: 3.16.24 -&gt; 3.16.27
  * [#47a99ab](https://github.com/OroraTech/nixpkgs/commit/47a99ab) pdns: 4.8.1 -&gt; 4.8.2

Changelog: https://doc.powerdns.com/authoritative/changelog/4.8.html#change-4.8.2
  * [#ba881ef](https://github.com/OroraTech/nixpkgs/commit/ba881ef) firefox-esr-102-unwrapped: remove

The Firefox ESR 102.0 series has reached its end of life.

Removes package and test and references to them.
  * [#42f7491](https://github.com/OroraTech/nixpkgs/commit/42f7491) perlPackages.Tk: fix build with clang 16

The jpeg `configure` script fails to detect clang as a functioning C
compiler because it uses a test with a `main` that returns an implicit
`int`, which results in an error with clang 16.
  * [#df4236c](https://github.com/OroraTech/nixpkgs/commit/df4236c) buildbot: supports reloading configuration

buildbot will reload configuration on sighup
  * [#6198bb8](https://github.com/OroraTech/nixpkgs/commit/6198bb8) buildbot-www-react: init 3.9.2
  * [#0958110](https://github.com/OroraTech/nixpkgs/commit/0958110) wimboot: 2.7.5 -&gt; 2.7.6
  * [#6de832b](https://github.com/OroraTech/nixpkgs/commit/6de832b) nixos/logrotate: add extraArgs option
  * [#847757c](https://github.com/OroraTech/nixpkgs/commit/847757c) python311Packages.adb-shell: 0.4.3 -&gt; 0.4.4

Diff: https://github.com/JeffLIrion/adb_shell/compare/v0.4.3...v0.4.4
  * [#189b142](https://github.com/OroraTech/nixpkgs/commit/189b142) nixos/networkd: Reload (not restart) when only .network units change

Underneath, systemd-networkd’s reload is just `networkctl reload`. Per
`man networkctl`, calling `reload` is expected to fully handle new,
modified, and removed .network files, but it only handles *new* .netdev
files. For simplicity, assume .network -&gt; reload and .netdev -&gt; restart.

It’s desirable to perform reload instead of restart, as restart has the
potential to bring down interfaces, resulting in a loss of network
connectivity.
  * [#dbb69f8](https://github.com/OroraTech/nixpkgs/commit/dbb69f8) nixos/restic: add wrapper scripts that set parameters for backup

and use in test
  * [#4732cbf](https://github.com/OroraTech/nixpkgs/commit/4732cbf) nixos/restic: use openssh as configured in programs.ssh
  * [#200c3ba](https://github.com/OroraTech/nixpkgs/commit/200c3ba) nixos/woodpecker-agents: add &#39;path&#39; option

See #249602.
  * [#6dd4c5f](https://github.com/OroraTech/nixpkgs/commit/6dd4c5f) nixos/woodpecker-agents: use &#39;literalExample&#39;

The next commit is going to add an option which takes a list of
packages. So the example must be converted to make it documentable.

This will also allow adding comments, to explain why some options are
used.
  * [#7d246a2](https://github.com/OroraTech/nixpkgs/commit/7d246a2) nixos/woodpecker-agents: fix typos in doc

The name of the backend is `local`, not `exec`.

`environmentFile` is supposed to be a list.
  * [#f715120](https://github.com/OroraTech/nixpkgs/commit/f715120) nixos/woodpecker-agents: fix &#39;podman&#39; example

The name should match the fact that we&#39;re using `podman` instead of
`docker`.

And the group was wrong.
  * [#5110d34](https://github.com/OroraTech/nixpkgs/commit/5110d34) wstunnel: correct listen option
  * [#ba2f38d](https://github.com/OroraTech/nixpkgs/commit/ba2f38d) nixos/zigbee2mqtt: persist groups set via ui
  * *On 9 Sept 2023, 19:34:53*
* 🔍 Reviewed [#254280 wallabag: rebase data env patch](https://github.com/NixOS/nixpkgs/pull/254280) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 9 Sept 2023, 19:30:05*
* 🔍 Reviewed [#254234 iosevka: 26.3.0 -&gt; 26.3.3](https://github.com/NixOS/nixpkgs/pull/254234) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 9 Sept 2023, 19:01:03*
* 🔍 Reviewed [#253612 xandikos: 0.2.8 -&gt; 0.2.10](https://github.com/NixOS/nixpkgs/pull/253612) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 9 Sept 2023, 18:59:58*
 <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.33.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 10 Sept 2023, 03:57:17 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
