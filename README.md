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
* ➡️ Pushed 680 commits in [OroraTech/nixpkgs](https://github.com/OroraTech/nixpkgs) on branch `master`
  * [#240ef42](https://github.com/OroraTech/nixpkgs/commit/240ef42) fw-ectool: init at unstable-2022-12-03
  * [#13d3b0c](https://github.com/OroraTech/nixpkgs/commit/13d3b0c) nixos/security/wrappers: add one regression test for #98863

Note that this regression test checks only s[gu]id wrappers. The issue
for capability wrappers is not fixed yet.
  * [#c64bbd4](https://github.com/OroraTech/nixpkgs/commit/c64bbd4) nixos/security/wrappers: remove all the assertions about readlink(/proc/self/exe)

Given that we are no longer inspecting the target of the /proc/self/exe
symlink, stop asserting that it has any properties. Remove the plumbing
for wrappersDir, which is no longer used.

Asserting that the binary is located in the specific place is no longer
necessary, because we don&#39;t rely on that location being writable only by
privileged entities (we used to rely on that when assuming that
readlink(/proc/self/exe) will continue to point at us and when assuming
that the `.real` file can be trusted).

Assertions about lack of write bits on the file were
IMO meaningless since inception: ignoring the Linux&#39;s refusal to honor
S[UG]ID bits on files-writeable-by-others, if someone could have
modified the wrapper in a way that preserved the capability or S?ID
bits, they could just remove this check.

Assertions about effective UID were IMO just harmful: if we were
executed without elevation, the caller would expect the result that
would cause in a wrapperless distro: the targets gets executed without
elevation. Due to lack of elevation, that cannot be used to abuse
privileges that the elevation would give.

This change partially fixes #98863 for S[UG]ID wrappers. The issue for
capability wrappers remains.
  * [#e355020](https://github.com/OroraTech/nixpkgs/commit/e355020) nixos/security/wrappers: read capabilities off /proc/self/exe directly

/proc/self/exe is a &#34;fake&#34; symlink. When it&#39;s opened, it always opens
the actual file that was execve()d in this process, even if the file was
deleted or renamed; if the file is no longer accessible from the current
chroot/mount namespace it will at the very worst fail and never open the
wrong file. Thus, we can make a much simpler argument that we&#39;re reading
capabilities off the correct file after this change (and that argument
doesn&#39;t rely on things such as protected_hardlinks being enabled, or no
users being able to write to /run/wrappers, or the verification that the
path readlink returns starts with /run/wrappers/).
  * [#1bdbc0b](https://github.com/OroraTech/nixpkgs/commit/1bdbc0b) nixos/security/wrappers: stop using `.real` files

Before this change it was crucial that nonprivileged users are unable to
create hardlinks to SUID wrappers, lest they be able to provide a
different `.real` file alongside. That was ensured by not providing a
location writable to them in the /run/wrappers tmpfs, (unless
disabled) by the fs.protected_hardlinks=1 sysctl, and by the explicit
own-path check in the wrapper. After this change, ensuring
that property is no longer important, and the check is most likely
redundant.

The simplification of expectations of the wrapper will make it
easier to remove some of the assertions in the wrapper (which currently
cause the wrapper to fail in no_new_privs environments, instead of
executing the target with non-elevated privileges).

Note that wrappers had to be copied (not symlinked) into /run/wrappers
due to the SUID/capability bits, and they couldn&#39;t be hard/softlinks of
each other due to those bits potentially differing. Thus, this change
doesn&#39;t increase the amount of memory used by /run/wrappers.

This change removes part of the test that is obsoleted by the removal of
`.real` files.
  * [#44fde72](https://github.com/OroraTech/nixpkgs/commit/44fde72) nixos/security/wrappers: generate a separate and more complete apparmor policy fragment for each wrapper

This change includes some stuff (e.g. reading of the `.real` file,
execution of the wrapper&#39;s target) that belongs to the apparmor policy
of the wrapper. This necessitates making them distinct for each wrapper.
The main reason for this change is as a preparation for making each
wrapper be a distinct binary.
  * [#c0e607d](https://github.com/OroraTech/nixpkgs/commit/c0e607d) nixos/tests/wrappers: test apparmor configuration

Wrappers generate pieces of apparmor policies for inclusion, which are
used only in a single place in nixpkgs, for `ping`. They are built only
if apparmor is enabled.

This change causes the test to test:
 - that the apparmor includes can be generated,
 - that `ping` works with apparmor enabled (as the only policy that
   references these includes).

Ideally there would be some other NixOS test that verifies that `ping`
specifically works. Sadly, there isn&#39;t one.
  * [#1475601](https://github.com/OroraTech/nixpkgs/commit/1475601) lib.generators.toGitINI: added test

Added basic generators.toGitINI test.
Mostly taken from https://github.com/nix-community/home-manager/blob/958c06303f43cf0625694326b7f7e5475b1a2d5c/tests/modules/programs/git/git.nix.
The ${&#34;\t} escape is used so that the lines aren&#39;t recognized as &#34;Wrong
indent style&#34;.
  * [#200c3ba](https://github.com/OroraTech/nixpkgs/commit/200c3ba) nixos/woodpecker-agents: add &#39;path&#39; option

See #249602.
  * [#a88b90c](https://github.com/OroraTech/nixpkgs/commit/a88b90c) lib.generators.toGitINI: escape string values in configuration

This should handle the special characters that typically occur.
Upstreaming of https://github.com/nix-community/home-manager/commit/642d9ffe24eec1290e94d70e8129ba74922fddf2
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
  * [#64a71ae](https://github.com/OroraTech/nixpkgs/commit/64a71ae) nixos/galene: do not restrict AF_NETLINK

Built-in TURN server requires AF_NETLINK address family.
  * [#1247042](https://github.com/OroraTech/nixpkgs/commit/1247042) geogebra: Fix 3D view

Fixes: https://github.com/NixOS/nixpkgs/issues/217855
  * [#ba2f38d](https://github.com/OroraTech/nixpkgs/commit/ba2f38d) nixos/zigbee2mqtt: persist groups set via ui
  * [#ae7fb11](https://github.com/OroraTech/nixpkgs/commit/ae7fb11) mir: 2.13.0 -&gt; 2.14.1
  * [#676c18e](https://github.com/OroraTech/nixpkgs/commit/676c18e) wlcs: 1.5.0 -&gt; 1.6.0
  * [#93efcda](https://github.com/OroraTech/nixpkgs/commit/93efcda) nixos/networkd: add DHCPServer PXE boot options

Signed-off-by: Matt Layher &lt;mdlayher@gmail.com&gt;
  * [#e320ebd](https://github.com/OroraTech/nixpkgs/commit/e320ebd) lean4: init at 4.0.0
  * *On 12 Sept 2023, 09:08:59*
* ➡️ Pushed 4 commits in [kip93/nixplusplus](https://github.com/kip93/nixplusplus) on branch `main`
  * [#ca1bcc2](https://github.com/kip93/nixplusplus/commit/ca1bcc2) Remove 1 level of depth in secrets module
  * [#3ea2027](https://github.com/kip93/nixplusplus/commit/3ea2027) More user defaults
  * [#0a22768](https://github.com/kip93/nixplusplus/commit/0a22768) Don&#39;t get stuck on kernel panic
  * [#a6b84b3](https://github.com/kip93/nixplusplus/commit/a6b84b3) Set default bootloader as systemd
  * *On 11 Sept 2023, 16:01:38*
* 🌟 Starred [StevenBlack/hosts](https://github.com/StevenBlack/hosts)
  * *On 10 Sept 2023, 22:24:41*
* ➡️ Pushed 17 commits in [kip93/nixplusplus](https://github.com/kip93/nixplusplus) on branch `main`
  * [#3c9658e](https://github.com/kip93/nixplusplus/commit/3c9658e) Fix config cross compilation&#39;s system args
  * [#b1ae1fa](https://github.com/kip93/nixplusplus/commit/b1ae1fa) Add special arg for nix++ flake
  * [#3d9a951](https://github.com/kip93/nixplusplus/commit/3d9a951) Improve memory defaults
  * [#2378a77](https://github.com/kip93/nixplusplus/commit/2378a77) Add cross compiled config boilerplate
  * [#294aca8](https://github.com/kip93/nixplusplus/commit/294aca8) Add expression for single config
It&#39;s a common enough use case after all
  * [#8536b15](https://github.com/kip93/nixplusplus/commit/8536b15) Fix config expression
  * [#2bbe571](https://github.com/kip93/nixplusplus/commit/2bbe571) Add comment
  * [#a51951b](https://github.com/kip93/nixplusplus/commit/a51951b) Use home-manager by default
  * [#60626fa](https://github.com/kip93/nixplusplus/commit/60626fa) Improve nixos toplevel name
  * [#c951c8a](https://github.com/kip93/nixplusplus/commit/c951c8a) Use newer version of nix
  * [#bc6b383](https://github.com/kip93/nixplusplus/commit/bc6b383) Fix registry
  * [#421074c](https://github.com/kip93/nixplusplus/commit/421074c) Fix typo on module packages expression
  * [#3dd8e57](https://github.com/kip93/nixplusplus/commit/3dd8e57) Remove module docs
Turns out, simple md files are not enough
  * [#dc8dda2](https://github.com/kip93/nixplusplus/commit/dc8dda2) Add categorized supported systems
  * [#1db7abb](https://github.com/kip93/nixplusplus/commit/1db7abb) Fix minor typo
  * [#4b565a9](https://github.com/kip93/nixplusplus/commit/4b565a9) Fix format
  * [#3426451](https://github.com/kip93/nixplusplus/commit/3426451) Update inputs
  * *On 10 Sept 2023, 22:01:55*
 <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.33.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 12 Sept 2023, 11:57:31 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
