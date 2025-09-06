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

* 🔍 Reviewed [#439966 python3Packages.pkg-about: 1.4.0 -&gt; 1.5.0](https://github.com/NixOS/nixpkgs/pull/439966) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 4 Sept 2025, 13:37:13*
* ➡️ Pushed 27 commits in [kip93/nix](https://github.com/kip93/nix) on branch `master`
  * [#2eacb3c](https://github.com/kip93/nix/commit/2eacb3c) Merge pull request #13851 from lovesegfault/http-binary-cache-store-once

refactor(libstore/http-binary-cache-store): pragma once
  * [#0590b13](https://github.com/kip93/nix/commit/0590b13) Revert &#34;Add a crude tracing mechansim for the build results&#34;

The commit says it was added for CA testing --- manual I assume, since
there is no use of this in the test suite. I don&#39;t think we need it any
more, and I am not sure whether it was ever supposed to have made it to
`master` either.

This reverts commit 2eec2f765a86b8954f3a74ff148bc70a2d32be27.
  * [#241abcc](https://github.com/kip93/nix/commit/241abcc) refactor(libstore/http-binary-cache-store): pragma once
  * [#35978ca](https://github.com/kip93/nix/commit/35978ca) Merge pull request #13848 from obsidiansystems/factor-out-drv-check

Factor out `checkOutputs`
  * [#d1bdaef](https://github.com/kip93/nix/commit/d1bdaef) Factor out `checkOutputs`

We currently just use this during the build of a derivation, but there is no
reason we wouldn&#39;t want to use it elsewhere, e.g. to check the outputs
of someone else&#39;s build after the fact.

Moreover, I like pulling things out of `DerivationBuilder` that are
simple and don&#39;t need access to all that state. While
`DerivationBuilder` is unix-only, this refactor also make the code more
portable &#34;for free&#34;.

The header is private, at Eelco&#39;s request.
  * [#6c8f5ef](https://github.com/kip93/nix/commit/6c8f5ef) Merge pull request #13802 from obsidiansystems/post-build-hook-later

Move `runPostBuildHook` out of `DerivationBuilder`
  * [#193ad73](https://github.com/kip93/nix/commit/193ad73) Merge pull request #13808 from obsidiansystems/derivation-builder-kvm

Create `StringSet DerivationBuilderParams::systemFeatures`
  * [#f4a0161](https://github.com/kip93/nix/commit/f4a0161) Create `StringSet DerivationBuilderParams::systemFeatures`

Do this to avoid checking &#34;system features&#34; from the store config
directly, because we rather not have `DerivationBuilder` depend on
`Store`.
  * [#79211b6](https://github.com/kip93/nix/commit/79211b6) Merge pull request #13846 from obsidiansystems/derivation-builder-params-aggregate-initialize

No more `DerivationBuilderParams:` constructor!
  * [#f5f9e32](https://github.com/kip93/nix/commit/f5f9e32) No more `DerivationBuilderParams:` constructor!

I am not sure how/why this started working. C++23?
  * [#564593b](https://github.com/kip93/nix/commit/564593b) Merge pull request #13837 from xokdvium/bump-nixpkgs

flake: Update nixpkgs
  * [#8ee7479](https://github.com/kip93/nix/commit/8ee7479) Merge pull request #13819 from obsidiansystems/relative-url

Implement `parseURLRelative`, use in `HttpBinaryCacheStore`
  * [#e82210b](https://github.com/kip93/nix/commit/e82210b) Implement `parseURLRelative`, use in `HttpBinaryCacheStore`

This allows us to replace some very hacky and not correct string
concatentation in `HttpBinaryCacheStore`. It will especially be useful
with #13752, when today&#39;s hacks started to cause problems in practice,
not just theory.

Also make `fixGitURL` returned a `ParsedURL`.
  * [#625477a](https://github.com/kip93/nix/commit/625477a) flake: Update nixpkgs

• Updated input &#39;nixpkgs&#39;:
    &#39;github:NixOS/nixpkgs/cd32a774ac52caaa03bcfc9e7591ac8c18617ced?narHash=sha256-VtMQg02B3kt1oejwwrGn50U9Xbjgzfbb5TV5Wtx8dKI%3D&#39; (2025-08-17)
  → &#39;github:NixOS/nixpkgs/d98ce345cdab58477ca61855540999c86577d19d?narHash=sha256-O2CIn7HjZwEGqBrwu9EU76zlmA5dbmna7jL1XUmAId8%3D&#39; (2025-08-26)

This update contains d1266642a8722f2a05e311fa151c1413d2b9653c, which
is necessary for the TOML timestamps to get tested via nixpkgsLibTests job.
  * [#231f3af](https://github.com/kip93/nix/commit/231f3af) Merge pull request #13835 from obsidiansystems/better-string-split

Better `stringSplit`
  * [#cc4aa70](https://github.com/kip93/nix/commit/cc4aa70) Better `stringSplit`

I need this for some `ParseURL` improvements, but I figure this is
better to send as its own PR.

I changed the tests willy-nilly to sometimes use
`std::list&lt;std::string_view&gt;` instead of `Strings` (which is
`std::list&lt;std::string&gt;`).

Co-Authored-By: Sergei Zimmerman &lt;sergei@zimmerman.foo&gt;
  * [#0bd9d6a](https://github.com/kip93/nix/commit/0bd9d6a) Merge pull request #13832 from kip93/fix/empty-ports

Handle empty ports with new URL parsing
  * [#7989e31](https://github.com/kip93/nix/commit/7989e31) Handle empty ports
  * [#0250d50](https://github.com/kip93/nix/commit/0250d50) Move `runPostBuildHook` out of `DerivationBuilder`

It is suppposed to be &#34;post build&#34; not &#34;during the build&#34; after all. Its
location now matches that for the hook case (see elsewhere in
`DerivationdBuildingGoal`).

It was in a try-catch before, and now it isn&#39;t, but I believe that it is
impossible for it to throw `BuildError`, which is sufficient for this
code motion to be correct.
  * [#f0c7fbc](https://github.com/kip93/nix/commit/f0c7fbc) Add /etc/ssl/certs/ca-certificates.crt in docker.nix
  * *On 28 Aug 2025, 22:24:09*
  * *On 26 Aug 2025, 17:56:17*
* 💬 Commented on [#13832 Handle empty ports with new URL parsing](https://github.com/NixOS/nix/issues/13832) from [NixOS/nix](https://github.com/NixOS/nix)
  * *On 26 Aug 2025, 16:19:36*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 6 Sept 2025, 03:48:24 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
