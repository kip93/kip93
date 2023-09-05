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
* ➡️ Pushed 196 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `chore/fix-sphinx-hook`
  * [#1a8886c](https://github.com/OroraTech/nixpkgs/commit/1a8886c) code-maat: init at 1.0.3

* the JAR is provided in ./libexec/code-maat (e.g. to reuse as a JAR dependnecy
in a Java project)
* the JAR is wrapped as an executable in ./bin/code-maat

Closes https://github.com/NixOS/nixpkgs/issues/208339
  * [#6959687](https://github.com/OroraTech/nixpkgs/commit/6959687) nixos/mautrix-telegram: drop removed --base-config flag

See also: https://github.com/mautrix/python/commit/9b67b17ac4927f63cc9a71dc450b9296c849b3ab
  * [#57df80f](https://github.com/OroraTech/nixpkgs/commit/57df80f) python310Packages.mautrix: 0.20.0 -&gt; 0.20.1

Changelog: https://github.com/mautrix/python/releases/tag/v0.20.1
Diff: https://github.com/mautrix/python/compare/v0.20.0...v0.20.1
  * [#5ee40b8](https://github.com/OroraTech/nixpkgs/commit/5ee40b8) exiv2: fix build on armv7l-linux

Remove failing tests for now, they&#39;re fixed in 0.28
  * [#5ab4510](https://github.com/OroraTech/nixpkgs/commit/5ab4510) nixos/budgie: Use the Network Manager Applet indicator

Signed-off-by: Federico Damián Schonborn &lt;fdschonborn@gmail.com&gt;
  * [#1db1e3c](https://github.com/OroraTech/nixpkgs/commit/1db1e3c) stdenv: Fix possible issues discovered with

```
set -o errexit -o nounset -o pipefail
shopt -s inherit_errexit
```

in `stdenv/default-builder.sh`
  * [#2127f21](https://github.com/OroraTech/nixpkgs/commit/2127f21) khard: add manpages to output
  * [#60241e2](https://github.com/OroraTech/nixpkgs/commit/60241e2) ldtk: 1.3.3 -&gt; 1.3.4
  * [#c0158e9](https://github.com/OroraTech/nixpkgs/commit/c0158e9) dosfstools: backport reproducible builds patch

Upstream, dosfstools respects SOURCE_DATE_EPOCH since this commit:
https://github.com/dosfstools/dosfstools/commit/8da7bc93315cb0c32ad868f17808468b81fa76ec
This means tools like mkfs.vfat will create deterministic outputs when SOURCE_DATE_EPOCH is set.
A backport in nixpkgs is warranted since this was already merged in 2021 and no release of dosfstools has been made since then.

Co-authored-by: Paul Meyer &lt;49727155+katexochen@users.noreply.github.com&gt;
  * [#dffc973](https://github.com/OroraTech/nixpkgs/commit/dffc973) hotdoc: 0.13.7 -&gt; 0.15
  * [#cb49832](https://github.com/OroraTech/nixpkgs/commit/cb49832) Remove dotnet dependency
  * [#582e30f](https://github.com/OroraTech/nixpkgs/commit/582e30f) wasabiwallet: 2.0.3 -&gt; 2.0.4
  * [#ebc420c](https://github.com/OroraTech/nixpkgs/commit/ebc420c) signal-desktop-beta: 6.24.0-beta.1 -&gt; 6.30.0-beta.2
  * [#25f0477](https://github.com/OroraTech/nixpkgs/commit/25f0477) signal-desktop: 6.27.1 -&gt; 6.29.1
  * [#2a3e20a](https://github.com/OroraTech/nixpkgs/commit/2a3e20a) geos: pull upstream fix for gcc-13 build failure

Without the change build against `gcc-13` fails as:

    $ nix build --impure --expr &#39;with import ./. {}; geos.override { stdenv = gcc13Stdenv; }&#39; -L
    ...
    /build/geos-3.11.2/include/geos/shape/fractal/HilbertEncoder.h:41:5: error: &#39;uint32_t&#39; does not name a type
       41 |     uint32_t encode(const geom::Envelope* env);
          |     ^~~~~~~~
    /build/geos-3.11.2/include/geos/shape/fractal/HilbertEncoder.h:21:1: note: &#39;uint32_t&#39; is defined in header &#39;&lt;cstdint&gt;&#39;; did you forget to &#39;#include &lt;cstdint&gt;&#39;?
       20 | #include &lt;vector&gt;
      +++ |+#include &lt;cstdint&gt;
  * [#55e4f1f](https://github.com/OroraTech/nixpkgs/commit/55e4f1f) cm256cc: pull fix pending upstream inclusion for gcc-13

Without the change build fails on `gcc-13` as:

    $ nix build --impure --expr &#39;with import ./. {}; cm256cc.override { stdenv = gcc13Stdenv; }&#39; -L
    ...
    /build/source/unit_test/data.h:37:9: error: &#39;uint16_t&#39; does not name a type
       37 |         uint16_t i;
          |         ^~~~~~~~
    /build/source/unit_test/data.h:33:1: note: &#39;uint16_t&#39; is defined in header &#39;&lt;cstdint&gt;&#39;; this is probably fixable by adding &#39;#include &lt;cstdint&gt;&#39;
       32 | #include &lt;string.h&gt;
      +++ |+#include &lt;cstdint&gt;
  * [#04df8d6](https://github.com/OroraTech/nixpkgs/commit/04df8d6) make-startupitem: fix typo in comment
  * [#0ab3a1f](https://github.com/OroraTech/nixpkgs/commit/0ab3a1f) nixos/nftables: add redirect for /etc/hosts
  * [#75e405c](https://github.com/OroraTech/nixpkgs/commit/75e405c) nixos/nftables: use environment.etc for redirects
  * [#9e51ec8](https://github.com/OroraTech/nixpkgs/commit/9e51ec8) nixos/nftables: add checkRulesetRedirects option
  * *On 5 Sept 2023, 09:45:56*
* ➡️ Pushed 198 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#9e04571](https://github.com/OroraTech/nixpkgs/commit/9e04571) nixos/mautrix-whatsapp: use  static user and group

The DynamicUser mechanism does not allow share the bridge
registration.yaml file with matrix-synapse in any easy way:

1. the mautrix-whatsapp group under which the service runs is not in
   /etc/group, so you can&#39;t add matrix-synapse to this.
   This makes the group read bit on the file useless as the group is
   effectively always empty.

2. It&#39;s not possible to use ACLs or copy the file during preStart or
   postStart because the commands are executed with low priviledges.

By using a normal (static) user/group the secret can be shared with
synapse as follows:

  services.matrix_synapse.settings.app_service_config_files =
    [ &#34;/var/lib/mautrix-whatsapp/whatsapp-registration.yaml&#34; ];

  users.users.matrix-synapse.extraGroups = [ &#34;mautrix-whatsapp&#34; ];
  * [#e932745](https://github.com/OroraTech/nixpkgs/commit/e932745) nixos/mautrix-whatsapp: fix docbook description

Until NixOS 23.11 is release all options must be marked as migrated from
docbook to markdown.
  * [#1a8886c](https://github.com/OroraTech/nixpkgs/commit/1a8886c) code-maat: init at 1.0.3

* the JAR is provided in ./libexec/code-maat (e.g. to reuse as a JAR dependnecy
in a Java project)
* the JAR is wrapped as an executable in ./bin/code-maat

Closes https://github.com/NixOS/nixpkgs/issues/208339
  * [#6959687](https://github.com/OroraTech/nixpkgs/commit/6959687) nixos/mautrix-telegram: drop removed --base-config flag

See also: https://github.com/mautrix/python/commit/9b67b17ac4927f63cc9a71dc450b9296c849b3ab
  * [#57df80f](https://github.com/OroraTech/nixpkgs/commit/57df80f) python310Packages.mautrix: 0.20.0 -&gt; 0.20.1

Changelog: https://github.com/mautrix/python/releases/tag/v0.20.1
Diff: https://github.com/mautrix/python/compare/v0.20.0...v0.20.1
  * [#5ee40b8](https://github.com/OroraTech/nixpkgs/commit/5ee40b8) exiv2: fix build on armv7l-linux

Remove failing tests for now, they&#39;re fixed in 0.28
  * [#5ab4510](https://github.com/OroraTech/nixpkgs/commit/5ab4510) nixos/budgie: Use the Network Manager Applet indicator

Signed-off-by: Federico Damián Schonborn &lt;fdschonborn@gmail.com&gt;
  * [#2127f21](https://github.com/OroraTech/nixpkgs/commit/2127f21) khard: add manpages to output
  * [#60241e2](https://github.com/OroraTech/nixpkgs/commit/60241e2) ldtk: 1.3.3 -&gt; 1.3.4
  * [#c0158e9](https://github.com/OroraTech/nixpkgs/commit/c0158e9) dosfstools: backport reproducible builds patch

Upstream, dosfstools respects SOURCE_DATE_EPOCH since this commit:
https://github.com/dosfstools/dosfstools/commit/8da7bc93315cb0c32ad868f17808468b81fa76ec
This means tools like mkfs.vfat will create deterministic outputs when SOURCE_DATE_EPOCH is set.
A backport in nixpkgs is warranted since this was already merged in 2021 and no release of dosfstools has been made since then.

Co-authored-by: Paul Meyer &lt;49727155+katexochen@users.noreply.github.com&gt;
  * [#cb49832](https://github.com/OroraTech/nixpkgs/commit/cb49832) Remove dotnet dependency
  * [#582e30f](https://github.com/OroraTech/nixpkgs/commit/582e30f) wasabiwallet: 2.0.3 -&gt; 2.0.4
  * [#ebc420c](https://github.com/OroraTech/nixpkgs/commit/ebc420c) signal-desktop-beta: 6.24.0-beta.1 -&gt; 6.30.0-beta.2
  * [#25f0477](https://github.com/OroraTech/nixpkgs/commit/25f0477) signal-desktop: 6.27.1 -&gt; 6.29.1
  * [#2a3e20a](https://github.com/OroraTech/nixpkgs/commit/2a3e20a) geos: pull upstream fix for gcc-13 build failure

Without the change build against `gcc-13` fails as:

    $ nix build --impure --expr &#39;with import ./. {}; geos.override { stdenv = gcc13Stdenv; }&#39; -L
    ...
    /build/geos-3.11.2/include/geos/shape/fractal/HilbertEncoder.h:41:5: error: &#39;uint32_t&#39; does not name a type
       41 |     uint32_t encode(const geom::Envelope* env);
          |     ^~~~~~~~
    /build/geos-3.11.2/include/geos/shape/fractal/HilbertEncoder.h:21:1: note: &#39;uint32_t&#39; is defined in header &#39;&lt;cstdint&gt;&#39;; did you forget to &#39;#include &lt;cstdint&gt;&#39;?
       20 | #include &lt;vector&gt;
      +++ |+#include &lt;cstdint&gt;
  * [#55e4f1f](https://github.com/OroraTech/nixpkgs/commit/55e4f1f) cm256cc: pull fix pending upstream inclusion for gcc-13

Without the change build fails on `gcc-13` as:

    $ nix build --impure --expr &#39;with import ./. {}; cm256cc.override { stdenv = gcc13Stdenv; }&#39; -L
    ...
    /build/source/unit_test/data.h:37:9: error: &#39;uint16_t&#39; does not name a type
       37 |         uint16_t i;
          |         ^~~~~~~~
    /build/source/unit_test/data.h:33:1: note: &#39;uint16_t&#39; is defined in header &#39;&lt;cstdint&gt;&#39;; this is probably fixable by adding &#39;#include &lt;cstdint&gt;&#39;
       32 | #include &lt;string.h&gt;
      +++ |+#include &lt;cstdint&gt;
  * [#04df8d6](https://github.com/OroraTech/nixpkgs/commit/04df8d6) make-startupitem: fix typo in comment
  * [#0ab3a1f](https://github.com/OroraTech/nixpkgs/commit/0ab3a1f) nixos/nftables: add redirect for /etc/hosts
  * [#75e405c](https://github.com/OroraTech/nixpkgs/commit/75e405c) nixos/nftables: use environment.etc for redirects
  * [#9e51ec8](https://github.com/OroraTech/nixpkgs/commit/9e51ec8) nixos/nftables: add checkRulesetRedirects option
  * *On 5 Sept 2023, 07:42:17*
* ➡️ Pushed 1 commit in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `feature/pkgs-native`
  * [#5dd00f1](https://github.com/OroraTech/nixpkgs/commit/5dd00f1) pkgsNative: init
  * *On 4 Sept 2023, 15:13:20*
* 💬 Commented on [#253261 pkgsNative: init](https://github.com/NixOS/nixpkgs/pull/253261) from [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 4 Sept 2023, 15:09:04*
 <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.33.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 5 Sept 2023, 10:58:30 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
