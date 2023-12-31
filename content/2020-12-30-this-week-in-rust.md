Title: This Week in Rust 371
Number: 371
Date: 2020-12-30
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/rust-lang/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/rust-lang/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/rust-lang/this-week-in-rust/pulls).

# Updates from Rust Community

No newsletters this week.

### Official
* [Inside] [Please welcome cjgillot and Nadrieril to compiler-contributors](https://blog.rust-lang.org/inside-rust/2020/12/28/cjgillot-and-nadrieril-for-compiler-contributors.html)
* [Inside] [1.49.0 pre-release testing](https://blog.rust-lang.org/inside-rust/2020/12/29/1.49.0-prerelease.html)

### Project/Tooling Updates
* [IntelliJ Rust Changelog #138](https://intellij-rust.github.io/2020/12/28/changelog-138.html)
* [Rust Analyzer Changelog #57](https://rust-analyzer.github.io/thisweek/2020/12/28/changelog-57.html)
* [Redox OS 0.6.0](https://www.redox-os.org/news/release-0.6.0/)

### Observations/Thoughts
* [Call Site Dependency Injection](https://matklad.github.io/2020/12/28/csdi.html)
* [A look at tokio 1.0 API Changes](https://leshow.github.io/post/udp_tokio_1_0/)
* [Memory-Safety Challenge Considered Solved? An In-Depth Study with All Rust CVEs](https://arxiv.org/abs/2003.03296)
* [45,000+ lines of Rust code later: An update on the Record & Debug Tool (rd)](https://github.com/sidkshatriya/me/blob/master/003-Rd-makes-significant-advances.md)
* [Cloning A Reference and Method Call Syntax in Rust](https://www.fpcomplete.com/blog/cloning-reference-method-calls/)
* [Executable PNGs](https://djharper.dev/post/2020/12/26/executable-pngs/)
* [Why mongodump is fast](https://windsoilder.github.io/why_mongodump_is_fast.html)

### Rust Walkthroughs
* [Concurrency in modern programming languages: Rust](https://dev.to/deepu105/concurrency-in-modern-programming-languages-rust-19co)
* [Building distributed GraphQL backend using Rust and Apollo Federation](https://dev.to/rkudryashov/building-distributed-graphql-backend-using-rust-and-apollo-federation-50bm)
* [Enhance code quality using `matches` macro! in Rust](https://blog.knoldus.com/enhance-code-quality-using-matches-macro-in-rust/)
* [ClickOnce for Rust Apps](https://taggartsoftware.medium.com/clickonce-for-rust-apps-f96873feb8f1)
* [Closures in Rust](https://zhauniarovich.com/post/2020/2020-12-closures-in-rust/)
* [Don't let failures spread over your suite with process-based tests isolation](https://blog.cyplo.dev/posts/2020/12/fail-and-fork/)
* [Triangle From Scratch](https://rust-tutorials.github.io/triangle-from-scratch/opening_a_window/win32.html)
* [video] [series] [(Live Coding) Advent of Code 2020 in Rust](https://youtube.com/playlist?list=PLoSY6azqHO7BpQo8jWKi4cFIobJo-TCzU)

### Miscellaneous
* [Redox OS 0.6 Released With Many Fixes, Rewritten Kernel Memory Manager](https://www.phoronix.com/scan.php?page=news_item&px=Redox-OS-0.6-Released)
* [The more things change...](https://smallcultfollowing.com/babysteps/blog/2020/12/30/the-more-things-change/)
* [Min const generics stabilization has been merged into master! It will reach stable on March 25, 2021 as part of Rust 1.51](https://www.reddit.com/r/rust/comments/kl1e24/min_const_generics_stabilization_has_been_merged/)

# Crate of the Week

This week's crate is [autograd](https://github.com/raskr/rust-autograd), a library of differentiable operations and tensors for machine learning applications.

Thanks to [Zicklag](https://users.rust-lang.org/t/crate-of-the-week/2704/864) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [withoutboats/heck - kebab case doesn't treat numbers as separate word?](https://github.com/withoutboats/heck/issues/18)
* [jplatte/js_int has several good first issues](https://github.com/jplatte/js_int/issues?q=is:issue+is:open+label:%22good+first+issue%22)

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

275 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2020-12-21..2020-12-28

* [stabilize `min_const_generics`](https://github.com/rust-lang/rust/pull/79135) (Huzzah!)
* [utilize PGO for rustc linux dist builds](https://github.com/rust-lang/rust/pull/80262)
* [suggest fn ptr rather than fn item and suggest to use `Fn` trait bounds rather than the unique closure type](https://github.com/rust-lang/rust/pull/80284)
* [implement a compiler diagnostic for move async mistake](https://github.com/rust-lang/rust/pull/80160)
* [highlight edition-specific keywords correctly in code blocks, accounting for code block edition modifiers](https://github.com/rust-lang/rust/pull/80226)
* [prevent caching normalization results with a cycle](https://github.com/rust-lang/rust/pull/80246)
* [fix ICE when lookup method in trait for type that have bound vars](https://github.com/rust-lang/rust/pull/80170)
* [remove `DefPath` from `Visibility` and calculate it on demand](https://github.com/rust-lang/rust/pull/80099)
* [`rustc_query_system`: reduce dependency graph memory usage](https://github.com/rust-lang/rust/pull/79589)
* [add `impl Div<NonZeroU*> for u*` which cannot panic](https://github.com/rust-lang/rust/pull/79134)
* [deprecate atomic `compare_and_swap` method](https://github.com/rust-lang/rust/pull/79261)
* [stabilize `core::slice::fill`](https://github.com/rust-lang/rust/pull/79213)
* [stabilize `deque_range`](https://github.com/rust-lang/rust/pull/79022)
* [use `clone_from` from `hashbrown::`{`HashMap`, `HashSet`}](https://github.com/rust-lang/rust/pull/80400)
* [futures: perf: pack the state and future of unfolds in the same memory](https://github.com/rust-lang/futures-rs/pull/2283)
* [cargo: stabilize `RUSTC_WORKSPACE_WRAPPER`](https://github.com/rust-lang/cargo/pull/8976)
* [rustdoc: stabilise `--default-theme` command line option](https://github.com/rust-lang/rust/pull/79642)

## Rust Compiler Performance Triage

* [2020-12-24](https://github.com/rust-lang/rustc-perf/blob/master/triage/2020-12-24.md):
3 Regressions, 5 Improvements
Major event this week is landing PGO for rustc (on x86_64-unknown-linux-gnu). We
expect other platforms to follow but further investigation will be needed,
especially for cross-compiled platforms. We expect to add LLVM PGO as well.

Triage done by @simulacrum.

See the [full report](https://github.com/rust-lang/rustc-perf/blob/master/triage/2020-12-24.md) for more.

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

*No RFCs were approved this week.*

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

*No RFCs are currently in the final comment period.*

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [Stabilize slice::strip_prefix and slice::strip_suffix](https://github.com/rust-lang/rust/pull/77853)
* [Tracking issue for stable SIMD in Rust](https://github.com/rust-lang/rust/issues/48556)

## New RFCs

* [New trait: core::convert::IntoUnderlying](https://github.com/rust-lang/rfcs/pull/3046)
* [#[target_feature(..)] In Trait Methods](https://github.com/rust-lang/rfcs/pull/3042)

# Upcoming Events

### Online
* [January 5, Buffalo, NY, US - Buffalo Rust User Group](https://www.meetup.com/Buffalo-Rust-Meetup/events/274936687/)
* [January 6, Johannesburg, ZA - Monthly Joburg Rust Chat - Johannesburg Rust Meetup](https://www.meetup.com/Johannesburg-Rust-Meetup/events/275424876/)
* [January 6, Indianapolis, IN, US - Indy.rs - with Social Distancing - Indy Rust](https://www.meetup.com/indyrs/events/jhfstrycccbjb/)
* [January 7, Berlin, DE - Rust Hack and Learn - Berline.rs](https://www.meetup.com/opentechschool-berlin/events/txcprrycccbkb/)
* [January 12, Seattle, WA, US - Monthly Meetup - Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksrycccbqb/)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Rust Software Engineer at CEMS (Amsterdam, NL and Delft, NL)](https://cemsbv.nl/jobs/rust-software-engineer)

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> This is a common theme in Rust’s design: To reduce breakage as code evolves, you’re only allowed to rely on features that have been intentionally declared by the author.

– [2e71828 on rust-users](https://users.rust-lang.org/t/why-explicit-const-fn-token-needed/53006/2)

Thanks to [Kornel](https://users.rust-lang.org/t/twir-quote-of-the-week/328/980) for the suggestion.

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), and [cdmistman](https://github.com/cdmistman).*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/knhni9/this_week_in_rust_371/)</small>
