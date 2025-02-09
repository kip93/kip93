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

* ➡️ Pushed 36 commits in [b-camacho/nix](https://github.com/b-camacho/nix) on branch `lfs`
  * [#39ef2e2](https://github.com/b-camacho/nix/commit/39ef2e2) Merge pull request #12375 from DeterminateSystems/fetchTree-errors

fetchTree: Distinguish between fetchGit and fetchTree consistently in error messages
  * [#5f6658b](https://github.com/b-camacho/nix/commit/5f6658b) fetchTree: Distinguish between fetchGit and fetchTree consistently
  * [#26539a0](https://github.com/b-camacho/nix/commit/26539a0) Add mbig-obj flag to allow cross-compiling libexpr to mingw32
  * [#7c8c71f](https://github.com/b-camacho/nix/commit/7c8c71f) Totally exclude nix::setStackSize on Windows
  * [#3032512](https://github.com/b-camacho/nix/commit/3032512) GitExportIgnoreSourceAccessor: Don&#39;t show «unknown»

In general we should set the path display prefix on the inner
accessor, so we now pass the display prefix to getAccessor().
  * [#177a067](https://github.com/b-camacho/nix/commit/177a067) Merge pull request #12372 from roberth/test-characterisation-log-to-stderr

tests/functional/characterisation/framework: Log to stderr
  * [#102d90e](https://github.com/b-camacho/nix/commit/102d90e) Fix duplicate setPathDisplay()

Fixes messages like &#39;copying /tmp/repo/tmp/repo to the store&#39;. The
PosixSourceAccessor already sets the prefix. Setting the prefix twice
shouldn&#39;t be a problem, but GitRepoImpl::getAccessor() returns a
wrapped accessor so it&#39;s not actually idempotent.
  * [#cfe9329](https://github.com/b-camacho/nix/commit/cfe9329) Merge pull request #12378 from DeterminateSystems/fix-shellcheck

Fix shellcheck warnings
  * [#fa87ad6](https://github.com/b-camacho/nix/commit/fa87ad6) Fix shellcheck warnings
  * [#a5de2dd](https://github.com/b-camacho/nix/commit/a5de2dd) tests/functional/characterisation/framework: Log to stderr

It seems that `meson test --print-errorlogs` only captures stderr,
so this makes it forward the logs as intended.

We might want to redirect stdout in our common setup script instead.
  * [#fbe2940](https://github.com/b-camacho/nix/commit/fbe2940) Merge pull request #12363 from roberth/issue-12161

Issue #12161, add `meta.mainProgram`
  * [#8d74495](https://github.com/b-camacho/nix/commit/8d74495) Merge pull request #12362 from roberth/refactor-realiseString

refactor: Extract EvalState::realiseString
  * [#6a2198d](https://github.com/b-camacho/nix/commit/6a2198d) Merge pull request #12251 from nix-windows/local-store/fix-infinite-loop

local-store: fix infinite loop on Windows
  * [#850329d](https://github.com/b-camacho/nix/commit/850329d) packages.nix-cli: Add meta.mainProgram
  * [#0d7418b](https://github.com/b-camacho/nix/commit/0d7418b) packages.default: Add meta.mainProgram
  * [#7465fbe](https://github.com/b-camacho/nix/commit/7465fbe) refactor: Extract EvalState::realiseString
  * [#b36637c](https://github.com/b-camacho/nix/commit/b36637c) nix-profile{,-daemon}.fish: Do not source twice

In order for the script not be sourced multiple times by the same shell
instance, `__ETC_PROFILE_NIX_SOURCED` needs to be set with a `--global`
flag.

Both files are almost identical.  And style differences make it harder
to see what is actually different and keep them in sync, when it is
required.
  * [#666d656](https://github.com/b-camacho/nix/commit/666d656) nix-profile-daemon.fish: fmt

`nix-profile.fish` and part of `nix-profile-daemon.fish` use 4 space
indentation.  Which is also the indentation that the fish shell
documentation is using.

Reformatting a chunk of `nix-profile-daemon.fish` from 2 space
indentation to 4 space indentation for consistency.
  * [#3bd7fa3](https://github.com/b-camacho/nix/commit/3bd7fa3) local-store: fix infinite loop on Windows

Also switch to std::filesystem.
  * [#b644e57](https://github.com/b-camacho/nix/commit/b644e57) Remove broken stack size logic from Windows

The API only changes the stack size once there&#39;s already a stack
overflow exception. Pretty useless.
  * *On 3 Feb 2025, 18:07:33*
* ➡️ Pushed 36 commits in [kip93/nix](https://github.com/kip93/nix) on branch `lfs`
  * [#39ef2e2](https://github.com/kip93/nix/commit/39ef2e2) Merge pull request #12375 from DeterminateSystems/fetchTree-errors

fetchTree: Distinguish between fetchGit and fetchTree consistently in error messages
  * [#5f6658b](https://github.com/kip93/nix/commit/5f6658b) fetchTree: Distinguish between fetchGit and fetchTree consistently
  * [#26539a0](https://github.com/kip93/nix/commit/26539a0) Add mbig-obj flag to allow cross-compiling libexpr to mingw32
  * [#7c8c71f](https://github.com/kip93/nix/commit/7c8c71f) Totally exclude nix::setStackSize on Windows
  * [#3032512](https://github.com/kip93/nix/commit/3032512) GitExportIgnoreSourceAccessor: Don&#39;t show «unknown»

In general we should set the path display prefix on the inner
accessor, so we now pass the display prefix to getAccessor().
  * [#177a067](https://github.com/kip93/nix/commit/177a067) Merge pull request #12372 from roberth/test-characterisation-log-to-stderr

tests/functional/characterisation/framework: Log to stderr
  * [#102d90e](https://github.com/kip93/nix/commit/102d90e) Fix duplicate setPathDisplay()

Fixes messages like &#39;copying /tmp/repo/tmp/repo to the store&#39;. The
PosixSourceAccessor already sets the prefix. Setting the prefix twice
shouldn&#39;t be a problem, but GitRepoImpl::getAccessor() returns a
wrapped accessor so it&#39;s not actually idempotent.
  * [#cfe9329](https://github.com/kip93/nix/commit/cfe9329) Merge pull request #12378 from DeterminateSystems/fix-shellcheck

Fix shellcheck warnings
  * [#fa87ad6](https://github.com/kip93/nix/commit/fa87ad6) Fix shellcheck warnings
  * [#a5de2dd](https://github.com/kip93/nix/commit/a5de2dd) tests/functional/characterisation/framework: Log to stderr

It seems that `meson test --print-errorlogs` only captures stderr,
so this makes it forward the logs as intended.

We might want to redirect stdout in our common setup script instead.
  * [#fbe2940](https://github.com/kip93/nix/commit/fbe2940) Merge pull request #12363 from roberth/issue-12161

Issue #12161, add `meta.mainProgram`
  * [#8d74495](https://github.com/kip93/nix/commit/8d74495) Merge pull request #12362 from roberth/refactor-realiseString

refactor: Extract EvalState::realiseString
  * [#6a2198d](https://github.com/kip93/nix/commit/6a2198d) Merge pull request #12251 from nix-windows/local-store/fix-infinite-loop

local-store: fix infinite loop on Windows
  * [#850329d](https://github.com/kip93/nix/commit/850329d) packages.nix-cli: Add meta.mainProgram
  * [#0d7418b](https://github.com/kip93/nix/commit/0d7418b) packages.default: Add meta.mainProgram
  * [#7465fbe](https://github.com/kip93/nix/commit/7465fbe) refactor: Extract EvalState::realiseString
  * [#b36637c](https://github.com/kip93/nix/commit/b36637c) nix-profile{,-daemon}.fish: Do not source twice

In order for the script not be sourced multiple times by the same shell
instance, `__ETC_PROFILE_NIX_SOURCED` needs to be set with a `--global`
flag.

Both files are almost identical.  And style differences make it harder
to see what is actually different and keep them in sync, when it is
required.
  * [#666d656](https://github.com/kip93/nix/commit/666d656) nix-profile-daemon.fish: fmt

`nix-profile.fish` and part of `nix-profile-daemon.fish` use 4 space
indentation.  Which is also the indentation that the fish shell
documentation is using.

Reformatting a chunk of `nix-profile-daemon.fish` from 2 space
indentation to 4 space indentation for consistency.
  * [#3bd7fa3](https://github.com/kip93/nix/commit/3bd7fa3) local-store: fix infinite loop on Windows

Also switch to std::filesystem.
  * [#b644e57](https://github.com/kip93/nix/commit/b644e57) Remove broken stack size logic from Windows

The API only changes the stack size once there&#39;s already a stack
overflow exception. Pretty useless.
  * *On 3 Feb 2025, 18:07:29*
* ➡️ Pushed 1 commit in [kip93/cp437-tools](https://github.com/kip93/cp437-tools) on branch `main`
  * [#906d7c3](https://github.com/kip93/cp437-tools/commit/906d7c3) Clean up README
  * *On 3 Feb 2025, 03:27:41*
* ➡️ Pushed 1 commit in [kip93/cp437-tools](https://github.com/kip93/cp437-tools) on branch `main`
  * [#b3e126d](https://github.com/kip93/cp437-tools/commit/b3e126d) Fix tests + lint scripts
  * *On 3 Feb 2025, 02:50:21*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 9 Feb 2025, 09:47:53 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
