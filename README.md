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

* 🔍 Reviewed [#442957 python3Packages.pkg-about: 1.5.0 -&gt; 2.0.1](https://github.com/NixOS/nixpkgs/pull/442957) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 15 Sept 2025, 21:24:50*
* ➡️ Pushed 74 commits in [kip93/nix](https://github.com/kip93/nix) on branch `fix/self-override`
  * [#5e46df9](https://github.com/kip93/nix/commit/5e46df9) Merge pull request #13957 from NixOS/drop-old-serve-protocol

 Remove support for serve protocol version &lt; 5
  * [#9df99e0](https://github.com/kip93/nix/commit/9df99e0) Remove ServeProto::Command::ExportPaths

This seems to have been unused since the build-remote.pl removal in February 2017 (27dc76c1a5dbe654465245ff5f6bc22e2c8902da).
  * [#fa048e4](https://github.com/kip93/nix/commit/fa048e4) Remove support for serve protocol &lt; 5

This was introduced in August 2018 (2825e05d21ecabc8b8524836baf0b9b05da993c6).
  * [#8c789db](https://github.com/kip93/nix/commit/8c789db) Merge pull request #13956 from NixOS/drop-unused-addMultipleToStoreLegacy

Drop unused LegacySSHStore::addMultipleToStoreLegacy()
  * [#f8b15bf](https://github.com/kip93/nix/commit/f8b15bf) Merge pull request #13951 from NixOS/drop-old-daemon-protocol

Remove support for worker protocol version &lt; 18
  * [#5013b38](https://github.com/kip93/nix/commit/5013b38) Drop unused LegacySSHStore::addMultipleToStoreLegacy()
  * [#247d16a](https://github.com/kip93/nix/commit/247d16a) Merge pull request #13954 from xokdvium/empty-list-elems-fix

libexpr: Fix Value::mkList for empty lists
  * [#d1d3ed6](https://github.com/kip93/nix/commit/d1d3ed6) Add release note
  * [#7d26bf8](https://github.com/kip93/nix/commit/7d26bf8) Merge pull request #13906 from obsidiansystems/derivation-builder-simpler

More `DerivationBuilder` simplifications
  * [#9c186c3](https://github.com/kip93/nix/commit/9c186c3) Merge pull request #13932 from NixOS/move-pathInfoCache

Reduce false sharing between pathInfoCache and Store
  * [#2ed2c79](https://github.com/kip93/nix/commit/2ed2c79) libexpr: Fix Value::mkList for empty lists

This code used to save the pointer to a small
list allocated on the stack to the Value, which
is unintended.
  * [#3c331b7](https://github.com/kip93/nix/commit/3c331b7) Merge pull request #13953 from xokdvium/value-alignment

libexpr: Overalign Value to 16 bytes
  * [#4524235](https://github.com/kip93/nix/commit/4524235) libexpr: Overalign Value to 16 bytes

This is necessary to make use of 128 bit atomics on x86_64 [1],
since MOVAPD, MOVAPS, and MOVDQA need memory operands to be 16-byte
aligned. We are not losing anything here, because Value is already 16-byte
wide and Boehm allocates memory in granules that are 16 bytes by default
on 64 bit systems [2].

[1]: https://patchwork.sourceware.org/project/gcc/patch/YhxkfzGEEQ9KHbBC@tucnak/
[2]: https://github.com/bdwgc/bdwgc/blob/54ac18ccbc5a833dd7edaff94a10ab9b65044d61/include/gc/gc_tiny_fl.h#L31-L33
  * [#86d1995](https://github.com/kip93/nix/commit/86d1995) Remove WorkerProto::Op::ImportPaths

This was obsoleted in May 2016 (538a64e8c314f23ba0c5d76201f1c20e71884a21).
  * [#4fb61bc](https://github.com/kip93/nix/commit/4fb61bc) Remove WorkerProto::Op::ExportPath

This was obsoleted in May 2016 (538a64e8c314f23ba0c5d76201f1c20e71884a21).
  * [#137a551](https://github.com/kip93/nix/commit/137a551) Remove support for daemon protocol version &lt; 18

Version 18 was introduced in November 2016 (4b8f1b0ec066a5b994747b1afd050f5f62d857f6).
  * [#a73cf44](https://github.com/kip93/nix/commit/a73cf44) Reduce false sharing between pathInfoCache and Store

`perf c2c` shows a lot of cacheline conflicts between purely read-only
Store methods (like `parseStorePath()`) and the Sync classes. So
allocate pathInfoCache separately to avoid that.
  * [#2acb955](https://github.com/kip93/nix/commit/2acb955) Combine `DerivationBuilder::{prepareBuild,startBuilder}`

After many other cleanups, it turns out there is no reason for these to
be separate methods. We can combine them to simplify things.
  * [#14c206f](https://github.com/kip93/nix/commit/14c206f) `DerivationBuilder` no more callback soup for logging

`startBuilder` just returns the descriptor for the pipe now.
  * [#7f3314a](https://github.com/kip93/nix/commit/7f3314a) `DerivationBuilder::initialOutputs` make `const`

At one point I remember it did mutatate `initialOutputs`, but not
anymore!
  * *On 15 Sept 2025, 20:50:18*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 10 Oct 2025, 06:52:07 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
