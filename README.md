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

* 🌟 Starred [DBCDK/morph](https://github.com/DBCDK/morph)
  * *On 19 Dec 2024, 23:52:53*
* 💬 Commented on [#10153 git-lfs support](https://github.com/NixOS/nix/issues/10153) from [NixOS/nix](https://github.com/NixOS/nix)
  * *On 19 Dec 2024, 14:33:18*
* 💬 Commented on [#10153 git-lfs support](https://github.com/NixOS/nix/issues/10153) from [NixOS/nix](https://github.com/NixOS/nix)
  * *On 18 Dec 2024, 17:31:01*
* ➡️ Pushed 100 commits in [b-camacho/nix](https://github.com/b-camacho/nix) on branch `lfs`
  * [#3081e7c](https://github.com/b-camacho/nix/commit/3081e7c) Merge pull request #12025 from NaN-git/strlen

optimize string concat
  * [#ad3a67a](https://github.com/b-camacho/nix/commit/ad3a67a) optimize string concat
  * [#ad296ea](https://github.com/b-camacho/nix/commit/ad296ea) Test: more specific error message for `head`

Sorry, I&#39;m not sure how to implement this. So just a test change.
And hopefully will be picked up by someone who is paying attention.
A hero.
  * [#ab5a9cf](https://github.com/b-camacho/nix/commit/ab5a9cf) Merge pull request #12016 from grahamc/patch-2

Disable suid and atime on the /nix mount point on Darwin
  * [#a7cdb55](https://github.com/b-camacho/nix/commit/a7cdb55) Merge pull request #12013 from DeterminateSystems/fix-11996

nix hash convert: Support SRI hashes that lack trailing &#39;=&#39; characters
  * [#49fa31f](https://github.com/b-camacho/nix/commit/49fa31f) Fix typo (#12015)
  * [#4137ead](https://github.com/b-camacho/nix/commit/4137ead) Disable suid and atime on the /nix mount point on Darwin

The Determinate Nix Installer has set nosuid and noatime in https://github.com/DeterminateSystems/nix-installer/pull/1338, and figured this perf and security improvement is worthy of upstreaming.

The /nix volume shouldn&#39;t have setuid binaries anyway, and filesystems seem to generally be noatime on macOS.
Further, the garbage collector doesn&#39;t use atime.
  * [#408c2fa](https://github.com/b-camacho/nix/commit/408c2fa) nix hash: Don&#39;t print &#39;nix hash&#39; deprecation message

Fixes #11997.
  * [#33b645c](https://github.com/b-camacho/nix/commit/33b645c) nix hash convert: Don&#39;t fail on uppercase base-16 hashes
  * [#52f1cd0](https://github.com/b-camacho/nix/commit/52f1cd0) nix hash convert: Support SRI hashes that lack trailing &#39;=&#39; characters

Fixes #11996.
  * [#d1894f3](https://github.com/b-camacho/nix/commit/d1894f3) tests: derivation-advanced-attributes unset NIX_STORE

when built by nix, NIX_STORE is set, which breaks $got when it
is not the default /nix/store
  * [#3b21ea4](https://github.com/b-camacho/nix/commit/3b21ea4) HttpBinaryCacheStore: Improve error message for unauthorized caches

Instead of the unhelpful

  warning: &#39;https://cache.flakehub.com&#39; does not appear to be a binary cache

you now get

  warning: unable to download &#39;https://cache.flakehub.com/nix-cache-info&#39;: HTTP error 401

           response body:

           {&#34;code&#34;:401,&#34;error&#34;:&#34;Unauthorized&#34;,&#34;message&#34;:&#34;Unauthorized.&#34;}
  * [#a8a572b](https://github.com/b-camacho/nix/commit/a8a572b) Merge pull request #12007 from mupdt/s3-binary-cache-error-request-id

s3-binary-cache: show the error&#39;s request ID
  * [#abcfdb4](https://github.com/b-camacho/nix/commit/abcfdb4) s3-binary-cache: show the error&#39;s request ID

The request ID is essential for traceability and debugging purposes.
It allows us to connect client-side to server-side events.
  * [#ff00eeb](https://github.com/b-camacho/nix/commit/ff00eeb) Merge pull request #12000 from NixOS/fix-men

fix: Add missing manpages to meson.build and more
  * [#63c0f0d](https://github.com/b-camacho/nix/commit/63c0f0d) Install init system configs only when relevant
  * [#038ab46](https://github.com/b-camacho/nix/commit/038ab46) Restore org.nixos.nix-daemon.plist installation
  * [#d67e24a](https://github.com/b-camacho/nix/commit/d67e24a) fix: Add missing manpages to meson.build
  * [#e83481f](https://github.com/b-camacho/nix/commit/e83481f) Allow `sudo` alternatives when installing from tarball
  * [#04975f7](https://github.com/b-camacho/nix/commit/04975f7) install: Allow to specify alternative `sudo` command
  * *On 18 Dec 2024, 17:19:10*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 21 Dec 2024, 19:47:37 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
