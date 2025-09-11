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

* ➡️ Pushed 66 commits in [kip93/nix](https://github.com/kip93/nix) on branch `fix/self-override`
  * [#44d096f](https://github.com/kip93/nix/commit/44d096f) `nix_store_is_valid_path` param `path` should be `const`
  * [#7e4608a](https://github.com/kip93/nix/commit/7e4608a) More `extern &#34;C&#34;` for FFI

This allows us to catch the header and file getting out of sync, because
we are not doing overloading by mistake.
  * [#eb56b18](https://github.com/kip93/nix/commit/eb56b18) DerivationBuildingGoal: Make almost everything private
  * [#c6ba120](https://github.com/kip93/nix/commit/c6ba120) `DerivationBuildingGoal::started` make local (lambda) variable
  * [#3b9c510](https://github.com/kip93/nix/commit/3b9c510) `DerivationBuildingGoal::outputLocks` make local variable
  * [#a63ac8d](https://github.com/kip93/nix/commit/a63ac8d) Inline `DerivationBuildingGoal::hookDone`
  * [#51dadad](https://github.com/kip93/nix/commit/51dadad) Move up `assert(!hook);`

We don&#39;t need to keep doing this every loop iteration, hook stuff it is only set
above.
  * [#7c1e5b3](https://github.com/kip93/nix/commit/7c1e5b3) In `DerivationBuildingGoal` Demote `actLock` to local variable

It doesn&#39;t need to be a field any more, because we just use it with two
loops.
  * [#4c44a21](https://github.com/kip93/nix/commit/4c44a21) Get rid of a `tryToBuild` tail recursive call with loop

This will make it easier to convert somethings to RAII.
  * [#95c5779](https://github.com/kip93/nix/commit/95c5779) `DerivationBuildingGoal::tryToBuild` pull hook waiting out of switch

Do this with a new `useHook` boolean we carefully make sure is set in
all cases. This change isn&#39;t really worthwhile by itself, but it allows
us to make further refactors (see later commits) which are
well-motivated.
  * [#c7603c6](https://github.com/kip93/nix/commit/c7603c6) Mark tmpDir as const
  * [#2fe629c](https://github.com/kip93/nix/commit/2fe629c) Fix deadlock in SSHMaster::addCommonSSHOpts()

When useMaster is true, startMaster() acquires the state lock, then
calls isMasterRunning(), which calls addCommonSSHOpts(), which tries
to acquire the state lock again, causing a deadlock.

The solution is to move tmpDir out of the state. It doesn&#39;t need to be
there in the first place because it never changes.
  * [#1286d5d](https://github.com/kip93/nix/commit/1286d5d) Fix macOS HUP detection using kqueue instead of poll

On macOS, poll() is fundamentally broken for HUP detection. It loses event
subscriptions when EVFILT_READ fires without matching the requested events
in the pollfd. This causes daemon processes to linger after client disconnect.

This commit replaces poll() with kqueue on macOS, which is what poll()
uses internally but without the bugs. The kqueue implementation uses
EVFILT_READ which works for both sockets and pipes, avoiding EVFILT_SOCK
which only works for sockets.

On Linux and other platforms, we continue using poll() with the standard
POSIX behavior where POLLHUP is always reported regardless of requested events.

Based on work from the Lix project (https://git.lix.systems/lix-project/lix)
commit 69ba3c92db3ecca468bcd5ff7849fa8e8e0fc6c0

Fixes: https://github.com/NixOS/nix/issues/13847
Related: https://git.lix.systems/lix-project/lix/issues/729
Apple bugs: rdar://37537852 (poll), FB17447257 (poll)

Co-authored-by: Jade Lovelace &lt;jadel@mercury.com&gt;
  * [#cbcb434](https://github.com/kip93/nix/commit/cbcb434) libexpr: Convert Symbol comparisons to switch statements

Now that Symbols are statically allocated at compile time with known IDs,
we can use switch statements instead of if-else chains for Symbol comparisons.
This provides better performance through compiler optimizations like jump tables.

Changes:
- Add public getId() method to Symbol class to access the internal ID
- Convert if-else chains comparing Symbol values to switch statements
  in primops.cc&#39;s derivationStrictInternal function
- Simplify control flow by removing the &#39;handled&#39; flag and moving the
  default attribute handling into the switch&#39;s default case

The static and runtime Symbol IDs are guaranteed to match by the
copyIntoSymbolTable implementation which asserts this invariant.

Co-authored-by: John Ericson &lt;git@JohnEricson.me&gt;
  * [#1935c19](https://github.com/kip93/nix/commit/1935c19) Merge pull request #13890 from xokdvium/mkstring-no-copy

Re-introduce mkStringNoCopy (revised)
  * [#6bdb5e8](https://github.com/kip93/nix/commit/6bdb5e8) Fix downstream MinGW build by not looking for Boost Regex
  * [#34181af](https://github.com/kip93/nix/commit/34181af) libexpr: Use mkStringNoCopy in prim_typeOf

This would lead to an unnecessary allocation. Not
a significant issue by any means, but it doesn&#39;t
have to allocate for most cases.
  * [#d62cfc1](https://github.com/kip93/nix/commit/d62cfc1) Re-introduce mkStringNoCopy (revised)

In b70d22b `mkStringNoCopy()` was renamed to
`mkString()`, but this is a bit risky since in code like

    vStringRegular.mkString(&#34;regular&#34;);

we want to be sure that the right overload is picked. (This is
especially problematic since the overload that takes an
`std::string_view` *does* allocate.)  So let&#39;s be explicit.

(Rebased from https://github.com/NixOS/nix/pull/11551)
  * [#725a2f3](https://github.com/kip93/nix/commit/725a2f3) don&#39;t include derivation name in temporary build directories

With the migration to /nix/var/nix/builds we now have failing builds
when the derivation name is too long.
This change removes the derivation name from the temporary build to have
a predictable prefix length:

Also see: https://github.com/NixOS/infra/pull/764
for context.
  * [#7b8ceb5](https://github.com/kip93/nix/commit/7b8ceb5) libutil, libexpr: #10542 abstract over getrusage for getting cpuTime stat and implement windows version

Update src/libutil/windows/current-process.cc

Prefer `nullptr` over `NULL`

Co-authored-by: Sergei Zimmerman &lt;sergei@zimmerman.foo&gt;

Update src/libutil/unix/current-process.cc

Prefer C++ type casts

Co-authored-by: Sergei Zimmerman &lt;sergei@zimmerman.foo&gt;

Update src/libutil/windows/current-process.cc

Prefer C++ type casts

Co-authored-by: Sergei Zimmerman &lt;sergei@zimmerman.foo&gt;

Update src/libutil/unix/current-process.cc

Don&#39;t allocate exception

Co-authored-by: Sergei Zimmerman &lt;sergei@zimmerman.foo&gt;
  * *On 9 Sept 2025, 18:06:13*
* 🔍 Reviewed [#440581 python3Packages.pycyphal: 1.24.3 -&gt; 1.24.5](https://github.com/NixOS/nixpkgs/pull/440581) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 9 Sept 2025, 14:29:24*
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
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 11 Sept 2025, 03:51:18 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
