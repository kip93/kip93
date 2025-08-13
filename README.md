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

* ⏺️ Created new branch fix/lfs-ssh in [kip93/nix](https://github.com/kip93/nix)
  * *On 13 Aug 2025, 14:41:01*
  * *On 13 Aug 2025, 14:28:43*
* ➡️ Pushed 737 commits in [kip93/nix](https://github.com/kip93/nix) on branch `master`
  * [#c81202b](https://github.com/kip93/nix/commit/c81202b) Merge pull request #13096 from NixOS/no-use-registries

getFlake(): Don&#39;t use registries for refetching
  * [#ee59af9](https://github.com/kip93/nix/commit/ee59af9) Merge pull request #13098 from roberth/fix-string-ctor

Fix flake-c out of bounds access
  * [#a525c7e](https://github.com/kip93/nix/commit/a525c7e) doc/manual: Add language/evaluation
  * [#9491613](https://github.com/kip93/nix/commit/9491613) Fix flake-c out of bounds access

The explicit include is needed for clangd to not get confused somehow,
which is also what threw me off initially and made me pick the wrong
constructor.
The (pointer, number, number) constructor first constructs a C string
and then takes a substring from that, but we didn&#39;t specify that the
buffer needs to be NUL-terminated, and then what would be the point of
the size argument anyway...

basic_string.h:

&gt;	basic_string(const _Tp&amp; __t, size_type __pos, size_type __n,
&gt;		     const _Alloc&amp; __a = _Alloc())
&gt;	: basic_string(_S_to_string_view(__t).substr(__pos, __n), __a) { }

Valgrind on nixops4/rust/nix-flake tests:

==1344422== Conditional jump or move depends on uninitialised value(s)
==1344422==    at 0x48513E8: strlen (vg_replace_strmem.c:505)
==1344422==    by 0x488E941: UnknownInlinedFun (char_traits.h:391)
==1344422==    by 0x488E941: UnknownInlinedFun (string_view:141)
==1344422==    by 0x488E941: UnknownInlinedFun (basic_string.h:790)
==1344422==    by 0x488E941: nix_flake_reference_and_fragment_from_string (nix_api_flake.cc:81)
==1344422==    by 0x127332: nix_flake::FlakeReference::parse_with_fragment (lib.rs:123)
  * [#3f811c2](https://github.com/kip93/nix/commit/3f811c2) Merge pull request #13094 from xokdvium/file-content-address-fmt-string

libutil: Add missing format arguments to UsageError ctor
  * [#953ec00](https://github.com/kip93/nix/commit/953ec00) getFlake(): Don&#39;t use registries for refetching

`newLockedRef` is already resolved so there is no need to re-resolve
it.
  * [#9fff868](https://github.com/kip93/nix/commit/9fff868) libutil: Add missing format arguments to UsageError ctor

Once again found by an automated migration to `std::format`.
I&#39;ve tested that boost::format works fine with `std::string_view`
arguments.
  * [#2704757](https://github.com/kip93/nix/commit/2704757) Merge pull request #13086 from xokdvium/bad-format-string

libutil: Fix invalid boost format string in infinite symlink recursion error
  * [#96a1740](https://github.com/kip93/nix/commit/96a1740) Merge pull request #13088 from NixOS/fix-ignore-local-registries

Fix ignore local registries
  * [#94edfb1](https://github.com/kip93/nix/commit/94edfb1) Merge pull request #13087 from xokdvium/libutil-git-permission-format

libutil: Use correct argument to Error format ctor
  * [#6405d68](https://github.com/kip93/nix/commit/6405d68) tests/flakes: add regression test for resolving user flakes
  * [#1b5c8aa](https://github.com/kip93/nix/commit/1b5c8aa) libutil: Use correct argument to Error format ctor

It seems that the intention was to format a number in base 8 (as
suggested by the %o format specifier), but `perms` is a `std::string`
and not a number. Looks like `rawMode` is the correct thing to use here.
  * [#bfb357c](https://github.com/kip93/nix/commit/bfb357c) libutil: Fix invalid boost format string in infinite symlink recursion error

Found while working on an automated migration to `std::format`.
  * [#b287f33](https://github.com/kip93/nix/commit/b287f33) Merge pull request #13085 from NixOS/bump-nixpkgs

flake.lock: Update
  * [#3e7d85d](https://github.com/kip93/nix/commit/3e7d85d) flake.lock: Update

Flake lock file updates:

• Updated input &#39;nixpkgs&#39;:
    &#39;github:NixOS/nixpkgs/f675531bc7e6657c10a18b565cfebd8aa9e24c14?narHash=sha256-gbl9hE39nQRpZaLjhWKmEu5ejtQsgI5TWYrIVVJn30U%3D&#39; (2025-04-09)
  → &#39;github:NixOS/nixpkgs/8a2f738d9d1f1d986b5a4cd2fd2061a7127237d7?narHash=sha256-sPwcCYuiEopaafePqlG826tBhctuJsLx/mhKKM5Fmjo%3D&#39; (2025-04-23)
  * [#a8fb23b](https://github.com/kip93/nix/commit/a8fb23b) Merge pull request #13079 from cole-h/cole-h/push-romznoxnzppy

nix-cli: restore binary-dist artifact to Hydra static builds
  * [#68de26d](https://github.com/kip93/nix/commit/68de26d) lockFlake(): Allow registry lookups for the top-level flake

Fixes #13050.
  * [#e1b6824](https://github.com/kip93/nix/commit/e1b6824) nix-cli: restore binary-dist artifact to Hydra static builds
  * [#dda265f](https://github.com/kip93/nix/commit/dda265f) Reapply &#34;Actually ignore system/user registries during locking&#34;

This reverts commit 3b5f0d9fb3af870b832bdcadcf8080649bcd0cd5.
  * [#8db8371](https://github.com/kip93/nix/commit/8db8371) glossary: re-introduce &#34;derivation&#34;

The &#34;derivation&#34; is one of the key concepts and captures the most distinctive aspect of Nix:
that we work with a certain type data (linked files) in a certain manner (using pure functions).

Here we finally arrange all the important pieces to show how they belong
together, while referring to the respective reference documentation for details.

This change also unbreaks downstream links to `//glossary#gloss-derivation`,
which had been broken by removing the glossary entry
  * *On 13 Aug 2025, 14:27:56*
* 🌟 Starred [Koenkk/zigbee-OTA](https://github.com/Koenkk/zigbee-OTA)
  * *On 22 Jul 2025, 16:06:33*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 13 Aug 2025, 23:48:12 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
