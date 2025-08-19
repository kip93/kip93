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

* 🌟 Starred [brybrant/lava-lamp](https://github.com/brybrant/lava-lamp)
  * *On 18 Aug 2025, 20:03:45*
* ➡️ Pushed 61 commits in [kip93/nix](https://github.com/kip93/nix) on branch `master`
  * [#4e776a5](https://github.com/kip93/nix/commit/4e776a5) Merge pull request #13753 from obsidiansystems/simplify-derivation-goal

Simplify `DerivationGoal` in many ways
  * [#677b1c0](https://github.com/kip93/nix/commit/677b1c0) prepare merge queues for nix
  * [#f64000e](https://github.com/kip93/nix/commit/f64000e) Merge pull request #13756 from xokdvium/fix-copy-path-message

libstore: Fix makeCopyPathMessage
  * [#e74ef41](https://github.com/kip93/nix/commit/e74ef41) libstore: Fix makeCopyPathMessage

Old code completely ignored query parameters and it seems ok to keep
that behavior. There&#39;s a lot of code out there that parses nix code
like nix-output-monitor and it can&#39;t parse messages like:

&gt; copying path &#39;/nix/store/wha2hi4yhkjmccqhivxavbfspsg1wrsj-source&#39; from &#39;https://cache.nixos.org&#39; to &#39;local://&#39;...

Let&#39;s not break these tools without a good reason. This goes in line
with what other code does by ignoring parameters in logs.

The issue is just in detecting the shorthand notations for the store
reference - not in printing the url in logs.

By default the daemon opens a local store with ?path-info-cache-size=0,
so that leads to the erronenous &#39;local://&#39;.
  * [#4b4895e](https://github.com/kip93/nix/commit/4b4895e) Merge pull request #13755 from xokdvium/concise-uri-logs

treewide: Remove getUri and replace with getHumanReadableURI where appropriate
  * [#1b7ffa5](https://github.com/kip93/nix/commit/1b7ffa5) treewide: Remove getUri and replace with getHumanReadableURI where appropriate

The problem with old code was that it used getUri for both the `diskCache`
as well as logging. This is really bad because it mixes the textual human
readable representation with the caching.

Also using getUri for the cache key is really problematic for the S3 store,
since it doesn&#39;t include the `endpoint` in the cache key, so it&#39;s totally broken.

This starts separating the logging / cache concerns by introducing a
`getHumanReadableURI` that should only be used for logging. The caching
logic now instead uses `getReference().render(/*withParams=*/false)` exclusively.
This would need to be fixed in follow-ups, because that&#39;s really fragile and
broken for some store types (but it was already broken before).
  * [#e6f3a19](https://github.com/kip93/nix/commit/e6f3a19) libstore: Fix makeCopyPathMessage after config getUri refactor
  * [#4a2de1d](https://github.com/kip93/nix/commit/4a2de1d) `DerivationGoal` Make some fields immutable

We can set both during construction, yay!
  * [#f155dff](https://github.com/kip93/nix/commit/f155dff) `DerivationGoal::done` Clean up parameter types

We don&#39;t need to ask all these callers to build these single-entry maps
for us.
  * [#c940283](https://github.com/kip93/nix/commit/c940283) `DerivationBuilder`

Move output result filtering logic and assert just into the branch where
it is not obviously a no op / meeting the assertion.

Add a comment too, while we are at it.
  * [#14441f9](https://github.com/kip93/nix/commit/14441f9) `DerivationGoal` inline `gaveUpOnSubstitution` lambda

We can shuffle around control flow so it&#39;s only called once. You&#39;ll
definitely want to review this diff ignoring whitespace.
  * [#88275e5](https://github.com/kip93/nix/commit/88275e5) `DerivationGoal` slight cleanup of some impure drv logic
  * [#7707d0a](https://github.com/kip93/nix/commit/7707d0a) Get rid of `filterDrvOutputs`

We don&#39;t need it any more, because we only used it in the
single-wanted-output `DerivationGoal`.
  * [#766a52c](https://github.com/kip93/nix/commit/766a52c) `DerivationOutput`: Remove `outputKnown` state

Now that `DerivationGoal::checkPathValidity` is legible, we can see that
it only sets `outputKnown`, and doesn&#39;t read it. Likewise, with
co-routines, we don&#39;t have tiny scopes that make local variables
difficult. Between these two things, we can simply have
`checkPathValidity` return what it finds, rather than mutate some state,
and update everyting to use local variables.

The same transformation could probably be done to the other derivation
goal types (which currently, unfortunately, contain their own
`checkPathValidity`s, though they are diverging, and we hope and believe
that they continue to diverge).
  * [#2324fe3](https://github.com/kip93/nix/commit/2324fe3) `DerivationBuilder::checkPathValidity`: Big simplify

`Store::queryPartialDerivationOutputMap` is nothing but checking
statically-known output paths, and then `Store::queryRealisation`, and
we were doing both of those things already. Inline that and simplify,
again taking advantage of the fact that we only care about one output.
  * [#b6ca60c](https://github.com/kip93/nix/commit/b6ca60c) `DerivationBuilder::checkPathValidity`: Simplify `allValid` calc

Now that the loops is gone, we can just inline this mutation to a single
simple expression.
  * [#2600391](https://github.com/kip93/nix/commit/2600391) Simplify `DerivationGoal` loop -&gt; if

More taking advantage of single wanted output. Also `auto *` not `auto`
for easy reading.
  * [#1a6f928](https://github.com/kip93/nix/commit/1a6f928) Don&#39;t use `InitialOutput` in `DerivationGoal`

We don&#39;t need the `wanted` field. Just inline the other two fields.
  * [#14173d7](https://github.com/kip93/nix/commit/14173d7) Simplify `DerivationGoal` by just storing a singular `initialOutput`

We know we want exactly want output in `DerivationGoal` now (since
recent refactors), so we can start simplifying things to take advantage
of this.
  * [#4b6edfc](https://github.com/kip93/nix/commit/4b6edfc) `DerivationBuildingGoal`: Check outputs beforehand

See the comment in the code for details. Some of the code is duplicated
for now, but we&#39;ll be cleaning that up soon.
  * *On 18 Aug 2025, 14:37:31*
  * *On 14 Aug 2025, 16:20:35*
* 💬 Commented on [#13743 Fix Git LFS SSH issues](https://github.com/NixOS/nix/pull/13743) from [NixOS/nix](https://github.com/NixOS/nix)
  * *On 13 Aug 2025, 16:03:14*
</details>


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v3.34.0</a> 🛠️<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ 19 Aug 2025, 18:51:48 / All times UTC ⌚ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
