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

* 🔃 Opened [#6500 Fix cross compilation due to #5920](https://github.com/nix-community/home-manager/pull/6500) in [nix-community/home-manager](https://github.com/nix-community/home-manager)
                * 1 file changed `++9 --5`
  * *On 19 Feb 2025, 22:45:26*
* ⏺️ Created new branch fix/xdg-mime-cross-compile-24.11 in [kip93/home-manager](https://github.com/kip93/home-manager)
  * *On 19 Feb 2025, 22:39:34*
* ➡️ Pushed 1 commit in [kip93/home-manager](https://github.com/kip93/home-manager) on branch `fix/xdg-mime-cross-compile`
  * [#e97567d](https://github.com/kip93/home-manager/commit/e97567d) xdg-mime: Fix cross compilation
  * *On 19 Feb 2025, 22:36:57*
* ➡️ Pushed 321 commits in [kip93/home-manager](https://github.com/kip93/home-manager) on branch `fix/xdg-mime-cross-compile`
  * [#f9fd45c](https://github.com/kip93/home-manager/commit/f9fd45c) volnoti: add self to maintainers
  * [#9ae941a](https://github.com/kip93/home-manager/commit/9ae941a) abook: remove platform linux assertion

Abook is also available on other platforms, e.g., Darwin.
  * [#5e2f47c](https://github.com/kip93/home-manager/commit/5e2f47c) hypridle: fix service when no config file

The systemd user service depends on

  config.xdg.configFile.&#34;hypr/hypridle.conf&#34;.source

for `X-Restart-Triggers`. When `cfg.settings` is the default `{}`,
this causes failure since

  config.xdg.configFile.&#34;hypr/hypridle.conf&#34;.source

will not exist.

Making the addition conditional on `cfg.settings` actually having
content, which would mean `xdg.configFile.&#34;hypr/hypridle.conf&#34;` does
exist, avoids the error.
  * [#bd58a11](https://github.com/kip93/home-manager/commit/bd58a11) hyprpaper: fix service when no config file

The systemd user service depends on

  config.xdg.configFile.&#34;hypr/hyprpaper.conf&#34;.source

for `X-Restart-Triggers`. When `cfg.settings` is the default `{}`,
this causes failure since

  config.xdg.configFile.&#34;hypr/hyprpaper.conf&#34;.source

will not exist.

Making the addition conditional on `cfg.settings` actually having
content, which would mean `xdg.configFile.&#34;hypr/hyprpaper.conf&#34;` does
exist, avoids the error.
  * [#67cd481](https://github.com/kip93/home-manager/commit/67cd481) flake.lock: Update

Flake lock file updates:

• Updated input &#39;nixpkgs&#39;:
    &#39;github:NixOS/nixpkgs/5e4fbfb6b3de1aa2872b76d49fafc942626e2add?narHash=sha256-OZiZ3m8SCMfh3B6bfGC/Bm4x3qc1m2SVEAlkV6iY7Yg%3D&#39; (2024-11-15)
  → &#39;github:NixOS/nixpkgs/23e89b7da85c3640bbc2173fe04f4bd114342367?narHash=sha256-y/MEyuJ5oBWrWAic/14LaIr/u5E0wRVzyYsouYY3W6w%3D&#39; (2024-11-19)
  * [#92fef25](https://github.com/kip93/home-manager/commit/92fef25) podman: install package and create config files

Co-authored-by: Dylan Wilson &lt;dylan@bytepen.com&gt;
  * [#ba9367b](https://github.com/kip93/home-manager/commit/ba9367b) emacs: add darwin service
  * [#16fe781](https://github.com/kip93/home-manager/commit/16fe781) conky: update systemd exec path to config package

Currently systemd ExecStart uses pkgs.conky as executable path, this
commit changes it to the package defined by services.conky.package.
  * [#445d721](https://github.com/kip93/home-manager/commit/445d721) home-cursor: add hyprcursor support

Add the option to enable hyprcursor support by setting the relevant
environment variables.
  * [#8cf9cb2](https://github.com/kip93/home-manager/commit/8cf9cb2) tests: fix integration test
  * [#a46e702](https://github.com/kip93/home-manager/commit/a46e702) espanso: fix test failure
  * [#d37f154](https://github.com/kip93/home-manager/commit/d37f154) flake.lock: Update

Flake lock file updates:

• Updated input &#39;nixpkgs&#39;:
    &#39;github:NixOS/nixpkgs/76612b17c0ce71689921ca12d9ffdc9c23ce40b2?narHash=sha256-IigrKK3vYRpUu%2BHEjPL/phrfh7Ox881er1UEsZvw9Q4%3D&#39; (2024-11-09)
  → &#39;github:NixOS/nixpkgs/5e4fbfb6b3de1aa2872b76d49fafc942626e2add?narHash=sha256-OZiZ3m8SCMfh3B6bfGC/Bm4x3qc1m2SVEAlkV6iY7Yg%3D&#39; (2024-11-15)

Co-authored-by: github-actions[bot] &lt;github-actions[bot]@users.noreply.github.com&gt;
  * [#a42fa14](https://github.com/kip93/home-manager/commit/a42fa14) syncthing: expand declarative configuration

This expands the Syncthing configuration to allow declarative
settings. Code mostly pulled from the Nixpkgs module.

Changes compared to the NixOS module are:

Removed the following options:

- user, group, systemService: Unnecessary since Syncthing always runs
  as the user declaring the configuration.

- dataDir configDir, databaseDir: Pointed to ~/.local/state/syncthing,
  the default Syncthing directory.

- openDefaultPorts: We don&#39;t have access to the system firewall.

Furthermore, multiple changes to systemd services were made to
maintain consistency with other Home Manager modules, sandboxing
options might need to be reviewed further.

Fixes #4049
  * [#705cf37](https://github.com/kip93/home-manager/commit/705cf37) Translate using Weblate (Ukrainian)

Currently translated at 100.0% (37 of 37 strings)

Co-authored-by: wadsaek &lt;wadsaek@gmail.com&gt;
Translate-URL: https://hosted.weblate.org/projects/home-manager/cli/uk/
Translation: Home Manager/Home Manager CLI
  * [#094265f](https://github.com/kip93/home-manager/commit/094265f) Translate using Weblate (Italian)

Currently translated at 100.0% (37 of 37 strings)

Co-authored-by: Lorenzo Bevilacqua &lt;lorenzobevilacqua02@gmail.com&gt;
Translate-URL: https://hosted.weblate.org/projects/home-manager/cli/it/
Translation: Home Manager/Home Manager CLI
  * [#0bd5e9c](https://github.com/kip93/home-manager/commit/0bd5e9c) librewolf: hide bookmarks option
  * [#1846299](https://github.com/kip93/home-manager/commit/1846299) librewolf: use mkFirefoxModule
  * [#f3a2ff6](https://github.com/kip93/home-manager/commit/f3a2ff6) zsh-abbr: update source path (#6084)
  * [#05d3b62](https://github.com/kip93/home-manager/commit/05d3b62) home-manager: prepare 25.05-pre
  * [#0918bb0](https://github.com/kip93/home-manager/commit/0918bb0) ci: make dependabot consider release-24.11
  * *On 19 Feb 2025, 22:32:31*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 21 Feb 2025, 02:59:49 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
