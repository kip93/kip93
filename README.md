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

* ➡️ Pushed 53 commits in [kip93/nix](https://github.com/kip93/nix) on branch `master`
  * [#08e42e2](https://github.com/kip93/nix/commit/08e42e2) Merge pull request #13769 from obsidiansystems/simplify-derivation-building-goal

Handle structured attrs, &#34;export references graph&#34; outside of `DerivationBuilder`
  * [#1d3ddb2](https://github.com/kip93/nix/commit/1d3ddb2) Further consolidate environment variable processing outside `DerivationBuilder`

Now, `DerivationBuilder` only concerns itself with `finalEnv` and
`extraFiles`, in straightforward unconditional code. All the fancy
desugaring logic is consolidated in `DerivationBuildingGoal`.

We should better share the pulled-out logic with `nix-shell`/`nix
develop`, which would fill in some missing features, arguably fixing
bugs.
  * [#e3c74f5](https://github.com/kip93/nix/commit/e3c74f5) Desugar structured attrs, &#34;export reference graph&#34; outside `DerivationBuilder`

I think this is a better separation of concerns. `DerivationBuilder`
doesn&#39;t need to to the final, query-heavy details about how these things
are constructed. It just operates on the level of &#34;simple, stupid&#34; files
and environment variables.
  * [#92b10cf](https://github.com/kip93/nix/commit/92b10cf) `DerivationBuilderImpl::writeStructuredAttrs` remove a rewrite

As much as I prefer rewriting the parsed rather than unparsed JSON for
elegance, this gets in the way of the separation of concerns that I am
trying to do.

As a practical matter, any rewriting that this did will also be done by
the second round of rewriting that remains below, so removing this code
should have no effect.
  * [#2767ae3](https://github.com/kip93/nix/commit/2767ae3) Deduplicate &#34;export reference graph&#34; logic a bit

The first part on `drvOptions.exportReferencesGraph` is the same in both
cases. It is just how the information is finally rendered that is
different.
  * [#ca86d34](https://github.com/kip93/nix/commit/ca86d34) Merge pull request #13799 from obsidiansystems/typed-sandbox-paths

Make `sandbox-settings` better typed, get `globals.hh` out of other headers
  * [#a712445](https://github.com/kip93/nix/commit/a712445) Make `Settings::sandboxPaths` well-typed

Parsing logic is moved from `DerivationBuilder`, where is doesn&#39;t
belong, to `Settings` itself, where it does.
  * [#5221263](https://github.com/kip93/nix/commit/5221263) No more `globals.hh` in headers

This is needed to rearrange include order, but I also think it is a good
thing anyways, as we seek to reduce the use of global settings variables
over time.
  * [#bce29ab](https://github.com/kip93/nix/commit/bce29ab) Move header outside Unix-only portion

We&#39;ll neeed some definitions elsewhere
  * [#8463fef](https://github.com/kip93/nix/commit/8463fef) Expose `ChrootPath`, `PathsInChroot`

Will want these for settings in a moment.
  * [#d53c7b8](https://github.com/kip93/nix/commit/d53c7b8) Push `#include` down to `.cc` file

That is where it should be.
  * [#4ab579b](https://github.com/kip93/nix/commit/4ab579b) Remove constructor from `ChrootPath`

I rather use designated initializers.
  * [#0df147b](https://github.com/kip93/nix/commit/0df147b) Bump the version of the SQLite caches

This avoids problems with older versions of Nix that don&#39;t put the
caches in WAL mode. That&#39;s generally not a problem, until you do something like

  nix build --print-out-paths ... | cachix

which deadlocks because cachix tries to switch the caches to truncate
mode, which requires exclusive access. But the first process cannot
make progress because the cachix process isn&#39;t reading from the pipe.
  * [#4ab8ff5](https://github.com/kip93/nix/commit/4ab8ff5) SQLite: Use std::filesystem::path
  * [#349d2c5](https://github.com/kip93/nix/commit/349d2c5) Use WAL mode for SQLite cache databases

With &#34;truncate&#34; mode, if we try to write to the database while another
process has an active write transaction, we&#39;ll block until the other
transaction finishes. This is a problem for the evaluation cache in
particular, since it uses long-running transactions.

WAL mode does not have this issue: it just returns &#34;busy&#34; right away,
so Nix will print

  error (ignored): SQLite database &#39;/home/eelco/.cache/nix/eval-cache-v5/...&#39; is busy

and stop trying to write to the evaluation cache. (This was the
intended/original behaviour, see AttrDb::doSQLite().)
  * [#bb600e1](https://github.com/kip93/nix/commit/bb600e1) Merge pull request #13796 from NixOS/onboarding-room-list

onboarding.md: List the private rooms
  * [#088cc17](https://github.com/kip93/nix/commit/088cc17) Merge pull request #13795 from xokdvium/factor-out-s3url

libstore: Introduce ParsedS3URL type
  * [#4134258](https://github.com/kip93/nix/commit/4134258) onboarding.md: List the private rooms

We forgot one in the latest onboarding
  * [#69fcc2c](https://github.com/kip93/nix/commit/69fcc2c) libstore: Introduce ParsedS3URL type

This systematizes the way our s3:// URLs are parsed in filetransfer.cc.
Yoinked out and refactored out of [1].

[1]: https://github.com/NixOS/nix/pull/13752

Co-authored-by: Bernardo Meurer Costa &lt;beme@anthropic.com&gt;
  * [#5fe6c53](https://github.com/kip93/nix/commit/5fe6c53) nix flake prefetch-inputs: Add

This command fetches all inputs of a flake in parallel.

Example runtime for

  $ chmod -R u+w /tmp/nix2; rm -rf /tmp/nix2; rm ~/.cache/nix/fetcher-cache-v3.sqlite*; rm -rf ~/.cache/nix/tarball-cache/ ~/.cache/nix/gitv3/; time nix flake prefetch-inputs --store /tmp/nix2 https://api.flakehub.com/f/pinned/informalsystems/cosmos.nix/0.3.0/018ce9ed-d0be-7ce5-81b6-a3c6e3ae1187/source.tar.gz

with http-connections = 1:

real    4m11.859s
user    2m6.931s
sys     0m25.619s

and http-connections = 25 (the default):

real    0m57.146s
user    2m49.506s
sys     0m36.008s
  * *On 25 Aug 2025, 21:08:29*
* 🔍 Reviewed [#436761 python3Packages.pycyphal: 1.18.0 -&gt; 1.24.3](https://github.com/NixOS/nixpkgs/pull/436761) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 25 Aug 2025, 16:31:39*
* 🔍 Reviewed [#436761 python3Packages.pycyphal: 1.18.0 -&gt; 1.24.3](https://github.com/NixOS/nixpkgs/pull/436761) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 25 Aug 2025, 15:27:38*
* 🔍 Reviewed [#436199 python3Packages.pkg-about: 1.3.7 -&gt; 1.4.0](https://github.com/NixOS/nixpkgs/pull/436199) in [NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
  * *On 25 Aug 2025, 14:30:29*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 26 Aug 2025, 13:02:07 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
