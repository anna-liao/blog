---
date: "2017-11-13"
publishdate: "2017-11-13"
lastmod: "2017-11-13"
draft: false
title: "Learning Rust"
tags: ["Rust"]
categories: ["Rust"]
img: "images/blog/2017/rust.png"
toc: true
summary: "Resources for learning Rust"
---

Welcome, new Rustacean! So you have decided that you want to start learning Rust. You are where I was in summer 2017. I have read a lot of stuff online, tinkered with some byte-sized newbie contributions to the Rust project, and generally just hung out with the Rust community both virtually and in person (at [Rust Belt Rust](https://rust-belt-rust.com/) in Columbus, OH). In case you start feeling a little lost and overwhelmed on where to look, let me give you the Newbie’s Guide of what I found to be super useful. There is still a steep learning curve for Rust and you will need to put in the time and practice. However, certain channels will superboost your initiation into the friendly Rustacean community before you become lost and frustrated.

One thing to note is that the Rust language has rapidly evolved in the past couple years, so some of the posts and examples online from 2015 and earlier may not be considered idiomatic anymore. This post will be point you towards resources that are regularly updated.

# Learning Rust

Most of the [Rust docs](https://doc.rust-lang.org/) are quite intimidating. I would start with the [Rust book](https://doc.rust-lang.org/book/second-edition/) while completing [Rust exercism](http://exercism.io/languages/rust/about) exercises and tinkering with Rust code in [play.rust-lang.org](http://play.rust-lang.org/). You can import some external crates in the Rust Playground. ([Examples](https://play.rust-lang.org/?gist=51280e8073b54f85cdf5c79547ea2502&version=stable) and [list of supported crates](https://github.com/integer32llc/rust-playground/blob/master/compiler/base/Cargo.toml))

It’s important to actually be writing Rust code and running it through the compiler while reading the book. I had read a few chapters of the Rust book and _thought_ I knew Rust, but then realized I didn’t really understand the concepts well when I tried to write code that compiles.

# Checking out the Rust community

Cool! So now you know some Rust and getting an idea of the syntax, semantics and concepts. What next?

Check out [https://users.rust-lang.org/](https://users.rust-lang.org/). One thing that is so cool about the Rust Language project is that it is transparent in how the language evolves. It is fascinating to read the threads and learn about how decisions are made for language development as well as increasing the usage and ergonomics of Rust for everyone. This includes Rust for developers that write production code, hobbyists, embedded systems, IDE support, Rubyists, Pythonistas, “frustrated C++ programmers”, and everyone and anyone that wants to know and learn more about Rust! :D

Look for a local [Rust meetup](https://www.meetup.com/topics/rust/) to meet other Rustaceans in your area.

# Community Updates

* Subscribe to [This Week in Rust](https://this-week-in-rust.org/).
* Look for `easy` and `help wanted` issues to contribute to the Rust projects. You can “watch” this [thread](https://users.rust-lang.org/t/twir-call-for-participation/4821) and get notified about new requests for contributions

# READ

* [https://blog.rust-lang.org/](https://blog.rust-lang.org/) for updates about the language.
* Memory Safety and [Fearless Concurrency](https://blog.rust-lang.org/2015/04/10/Fearless-Concurrency.html) are the foundation of the Rust language
* [Programming Rust](http://shop.oreilly.com/product/0636920040385.do), deep dive into how Rust works

# WATCH

* Rust talks online ([Rust YouTube](https://www.youtube.com/channel/UCaYhcUwRBNscFNUKTjgPFiA) channel). There are 3 conference series: RustConf (West USA), Rust Belt Rust (Rust Belt, Midwest USA), and RustFest (Europe).
* Follow [@RustVideos](https://twitter.com/RustVideos) on Twitter

## Highlights:

* [History of Rust](https://www.youtube.com/watch?v=79PSagCD_AY)
* [RustConf 2016 closing keynote](http://www.youtube.com/watch?v=ftQfpAeyxPo) by Julia Evans. Check out her [website](https://jvns.ca/) for a bunch of great comics explaining technical concepts.
* [Rust screencasts](http://intorust.com/), by Niko of the Rust Core team
* [Rust overview](https://www.youtube.com/playlist?list=PLo3w8EB99pqJ74XIGe72c9hBZWz9Y16cY) from Mozilla team

---

If you are still looking for more links to add to your heap (heaps can grow, stacks not B-)): [https://github.com/rust-unofficial/awesome-rust](https://github.com/rust-unofficial/awesome-rust)

Best of luck in your journey and hope to see you around in the Rust community!