# Awesome Source Auditing [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)

🚧 Work in Progress 🚧

> A curated list of source auditing resources.

- [Introduction](#introduction)
  - [Guides](#guides)
- [Manual Reference](#manual-reference)
  - [Cheatsheets](#cheatsheets)
    - [Sanity Checks](#sanity-checks)
    - [Comprehensive Lists](#comprehensive-lists)
    - [Tool Suggestions](#tool-suggestions)
  - [Best Practices](#best-practices)
  - [Vulnerability Lists](#vulnerability-lists)
- [Automation](#automation)
  - [Automated Searching](#automated-searching)
  - [Static Analysis Tools](#static-analysis-tools)
  - [Simple Fuzzers](#simple-fuzzers)
- [Practice](#practice)
  - [War Games / CTFs](#war-games--ctfs)
- [Other Awesome Lists](#other-awesome-lists)
- [Thanks](#thanks)
- [Contribute](#contribute)

## Introduction

### Guides

- [CTF Field Guide - Auditing Source Code](https://trailofbits.github.io/ctf/vulnerabilities/source.html) - this was my first introduction to source auditing, I highly recommend watching the lectures.
- [OWASP Code Review Guide](https://owasp.org/www-project-code-review-guide/) - this guide is quite large but it might be helpful to mentally index it and keep the link handy.

## Manual Reference

### Cheatsheets

#### Sanity Checks

- [Kudelski Security's Auditing code for crypto flaws: the first 30 minutes](https://research.kudelskisecurity.com/2017/04/24/auditing-code-for-crypto-flaws-the-first-30-minutes/)
- [Kudelski Security's Auditing Rust Crypto: The First Hours](https://research.kudelskisecurity.com/2019/02/07/auditing-rust-crypto-the-first-hours/)

#### Comprehensive Lists

- [iSECPartners LibTech-Auditing-Cheatsheet](https://github.com/iSECPartners/LibTech-Auditing-Cheatsheet) - awesome checklist, albeit slightly outdated (I forked it with the intention of modernizing it, feel free to chime in with your thoughts [here](https://github.com/sgmenda/LibTech-Auditing-Cheatsheet/issues).)

#### Tool Suggestions

- [Security assessment techniques for Go projects](https://blog.trailofbits.com/2019/11/07/attacking-go-vr-ttps/) - awesome blog post, so good that this is the only Go resource on this page!

### Best Practices

- [Pornin's Constant-Time Crypto](https://bearssl.org/constanttime.html) - the definitive source for constant-time crypto.
- [veorq's Cryptocoding](https://github.com/veorq/cryptocoding) - the definitive source cryptocoding recommendations.

### Vulnerability Lists

- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)
- [2020 CWE Top 25](https://cwe.mitre.org/top25/archive/2020/2020_cwe_top25.html)
- CWE Views:
  - [CWE VIEW: Weaknesses Introduced During Design](https://cwe.mitre.org/data/definitions/701.html)
  - [CWE VIEW: Weaknesses Introduced During Implementation](https://cwe.mitre.org/data/definitions/702.html)
  - [CWE VIEW: Weaknesses in Software Written in C](https://cwe.mitre.org/data/definitions/658.html)
  - [CWE VIEW: Weaknesses in Software Written in C++](https://cwe.mitre.org/data/definitions/659.html)
  - [CWE VIEW: Weaknesses in Software Written in Java](https://cwe.mitre.org/data/definitions/660.html)
- [Bugs You'll Probably Only Have in Rust](https://gankra.github.io/blah/only-in-rust/)

## Automation

### Automated Searching

- [Sourcetrail](https://github.com/CoatiSoftware/Sourcetrail) - source explorer that makes it easy to understand and navigate large code bases.
- [Semgrep](https://github.com/returntocorp/semgrep) - static analysis tool that makes it really easy to search code.
- [CodeQL](https://securitylab.github.com/tools/codeql) - static analysis tool that is much more powerful than semgrep, but also harder to use.
- [Joern](https://github.com/ShiftLeftSecurity/joern) - looks like an open-source alternative to CodeQL (I haven't had a chance to play with it yet).

### Static Analysis Tools

- Basic Sanitizers:
  - [AddressSanitizer​](https://clang.llvm.org/docs/AddressSanitizer.html)
  - [MemorySanitizer](https://clang.llvm.org/docs/MemorySanitizer.html)
  - [UndefinedBehaviorSanitizer](https://clang.llvm.org/docs/UndefinedBehaviorSanitizer.html)
  - [ThreadSanitizer](https://clang.llvm.org/docs/ThreadSanitizer.html)
- [clang static analyzer](https://clang-analyzer.llvm.org/scan-build.html) - easy to use, and might be a good second step after the sanitizers.
- [cppcheck](https://github.com/danmar/cppcheck) - simple static analysis tool for C/C++.
- [RATS](https://github.com/andrew-d/rough-auditing-tool-for-security) - seems a outdated but you might still be able to get something out of it (I haven't even compiled it, so no warranties here.)
- [slither](https://github.com/crytic/slither) - the goto static analysis tool for solidity.
- [Creating an LLVM Sanitizer from Hopes and Dreams](https://blog.trailofbits.com/2019/06/25/creating-an-llvm-sanitizer-from-hopes-and-dreams/) - tutorial on how to write a new LLVM sanitizer.

### Simple Fuzzers

- clang [libfuzzer](https://llvm.org/docs/LibFuzzer.html) - a standard no-frills fuzzing engine
- [AFL](https://github.com/google/AFL) - a standard no-frills fuzzing engine
- [Rust Fuzz Book](https://rust-fuzz.github.io/book/introduction.html) - instructions on how to fuzz rust projects.

## Practice

### War Games / CTFs

- [The Ethernaut](https://ethernaut.openzeppelin.com/)
- [Cryptopals](https://cryptopals.com/)
- [exploit.education](https://exploit.education/)

## Other Awesome Lists

- [Awesome Security](https://github.com/sbilly/awesome-security/)

## Thanks

- I used [dar5hak/generator-awesome-list](https://github.com/dar5hak/generator-awesome-list) to generate the template for this repo.

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
