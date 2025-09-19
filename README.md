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
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 19 Sept 2025, 05:47:40 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
