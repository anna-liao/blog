---
date: "2017-11-02"
publishdate: "2017-11-02"
lastmod: "2017-11-02"
draft: false
title: "Increasing Rust’s Reach: Porting a Python application to Rust"
tags: ["Rust", "Python"]
categories: ["Rust"]
img: "images/blog/2017/rustbridge.jpg"
toc: true
summary: "My project to learn Rust and write a Rust script while referring to a Python library."
---

I participated in the [Increasing Rust’s Reach](https://blog.rust-lang.org/2017/06/27/Increasing-Rusts-Reach.html) program from August to November 2017. My project was **#7 Finding Missing Pieces in the Crates Ecosystem with Andrew Gallant**. I quickly learned that Andrew, aka @[burntsushi](https://github.com/BurntSushi), is well known in the Rust community for developing [`ripgrep`](https://blog.burntsushi.net/ripgrep/), a command line search tool that is faster than the Silver Searcher and `grep`. Just a web search on `ripgrep` will show you how often it is mentioned by others. Visual Studio search is powered by `ripgrep`. I was in awe that I was selected to work with Andrew, AND he is a really nice and knowledgeable guy to work with.

The plan for my project was to take a small application in Python and port it to Rust. Andrew is a member of the [Rust Libraries team](https://www.rust-lang.org/en-US/team.html) that oversees the Rust standard library, rust-lang crates, conventions, and ecosystem support. The goal is to see how my project could reveal gaps and missing functionality in the Rust library and crates that a new user may encounter. The Library team could then consider how to make the library more usable.

At my previous job at Lawrence Berkeley National Laboratory (a U.S. Dept of Energy lab), I built systems to monitor energy use in buildings and urban systems for research to inform energy policy. I was primarily using Python and open source libraries for my projects. I became interested in learning a modern systems programming language, such as Go or Rust, to see how it could improve performance in our systems.

---

I decided on writing a Rust application for the Raspberry Pi. I also have the [Sense HAT](https://www.raspberrypi.org/products/sense-hat/) add-on board with LED matrix. I focused on writing out to the LED matrix, for example, this [Python example](https://github.com/RPi-Distro/python-sense-hat/blob/master/examples/rainbow.py) to display a dynamic rainbow pattern.

It essentially comes down to translating the [`set_pixels()`](https://github.com/RPi-Distro/python-sense-hat/blob/master/sense_hat/sense_hat.py#L272) function and supporting function [`_get_fb_device()`](https://github.com/RPi-Distro/python-sense-hat/blob/master/sense_hat/sense_hat.py#L165).

It requires representing the pixel map with the correct type representation, reading a file, composing the path for another file, converting the pixel map to the binary representation, and writing to that file.

This seemingly basic and simple application took me down the journey to learn and discover:

* Types
* `Option`s and `Result`s
* `?` [operator](https://blog.rust-lang.org/2016/11/10/Rust-1.13.html)
* Error handling
* File handling
* `Path` and `PathBuf` types
* Parsing `String` and `&str`
* Bit manipulation and 16-bit RGB565 representation
* `vec` vs arrays, and the `clone` trait. Objects allocated on the heap vs stack.
* You can import some external crates to play.rust-lang.org ([example](https://play.rust-lang.org/?gist=51280e8073b54f85cdf5c79547ea2502&version=stable)) [List of supported crates](https://github.com/integer32llc/rust-playground/blob/master/compiler/base/Cargo.toml)
* “I don’t understand the compiler error. Let me try adding some `mut`s and `&`s and see if it compiles.”
* “Yay, it compiles! I have no idea why that worked! I’m not even sure if it’s actually still correct for the functionality I was working towards or that I just shut up the compiler”
* Debugging Rust with breakpoints, not officially supported. However, you can use gdb/lldb. One option is use gdb/lldb with Visual Studio Code.
* Many times, I was frustrated that I knew exactly how to express what I wanted to code in Python, but was clueless as to how to write it in Rust. Thus, learning a new language :)
* Many times, it really just came down to Andrew telling me exactly what the code snippet should look like. And then of course it worked. :P

Through this project, I learned much of the Rust basics, but made slow progress towards accomplishing the goal I defined at the beginning of the Rust Reach program. It’s ok, as Rust is known to have a steep learning curve, and now I can write Rust code a bit more fluidly without getting stumped every few characters. I plan to continue to stumble along even after the program ends. I am _almost_ to the point of writing out the file in the RPi, but still working out file write error.

---

Big thanks to: Andrew Gallant for volunteering as my mentor for this program; Carol (Nichols || Goulding) for coordinating the Increasing Rust’s Reach program and organizing the [Rust Belt Rust](https://www.rust-belt-rust.com/) conference; and the many other awesome members of the [Rust Team](https://www.rust-lang.org/en-US/team.html) and community for encouragement and advice during my learning process.

I will be giving a [talk](https://www.pycascades.com/talks/raspberrypy-to-rustypi-translating-a-python-api-to/) on this project at PyCascades (Jan 2018) in Vancouver, B.C., Canada. I’m hoping to have made some more progress on it by then!
