---
layout: post
title: "Rust I/O: Seekable File Corruptions"
date: 2016-10-02 04:42:00 +0300
categories: rust file seek corruption
---

Recently I've been implementing different compression algorithms in Rust for educational purposes.

While making an archiving program with file index I ran into a problem:
writing file offsets after `seek()` **sometimes** writes random rubbish.

I didn't post the issue on GitHub 'cause it seems to be tricky to write a minimalistic example for the bug reproduction
(also not sure if this is a bug at all).

If anyone runs into a similar issue---for me `try_clone()` and only then `seek()`/`write()` **probably [fixes the issue](https://github.com/alopatindev/rust-experiments/commit/f8b4ae260bb83f8fae68de172a40295eb754351b#diff-2a6421ea097a516a9c295f078d7a2023R213)**.
