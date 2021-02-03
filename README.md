# `redpkt2021` - "The IDA Case"

*The Red Envelope Puzzle for new year 2021, made for the r00team with much love.*

English | [简体中文](README.zh-CN.md)

## Briefing

> Hello, EZForever speaking:
> 
> You might already know that I've spent tons of time last year digging into Hex-Rays' anti-piracy approaches, but with little to no success. I hereby provide you a chance (challenge?) to try the cracking by yourself and get a hands-on experience of what the cracking communities be struggling to do for years.

**Challenge type:** Misc / Reverse / Crypto / Internet / Whatever

**Estimated difficulty:** Medium to Hard

## Goal

There is a "leaked" copy of *Not IDA 7.0* (I know it sounds stupid but bear with me) installer package available for download on the [Releases](https://github.com/ezforever/redpkt2021/releases) page. Of course, the installation password of which is not leaked thus unknown.

Your mission is to crack this package open and find the flag embedded in somewhere. The flag in this challenge follows an irregular format of `/r00t/[0-9a-zA-Z+]+/`. You will almost certainly need to search on the Internet for relevant information, and definitely will need to code for the flag.

Best of luck.

## Rewards

Flag submission is open for 5 days after this repo went public. The first competitor to submit the correct flag wins a 100 CNY worth of "red packet". DM me for flag submission and other details.

To make this challenge not too boring, new hints are given on this repo every day until someone wins or day 5 has passed.

Also, as always, there are easter eggs scattered throughout this challenge; be the first ~~three~~ five competitors to find at least 5 *Bubble Tea Tokens* and win a cup of bubble tea from me. ("What is a Bubble Tea Token?", you might ask. Well, you'll know once you've found one.) For the sake of funniness, this egg-spotting activity will continue until this winter vacation ends.

*P.S. The rewards are only for students of Donghua University. If you're not, feel free still to submit the flag and tokens. Maybe I'll give you a hug instead after the pandemic ends?*

*P.P.S. All Bubble Tea Tokens are the same in appearance; so to prove you've found enough tokens, you need to provide descriptions or at least screenshots on how you find them.*

[//]: # (*P.P.P.S. The first Bubble Tea Token, so you know what they look like: `0x91779111`. Time to get your hands dirty. Not with real eggs though, that's gross.*)

## Hints

0. As written on the Releases page, you need to extract the contents (at least `ida.key`) from the given package, either by cracking the password or bypass it.
1. You don't need any previous knowledge from IDA cracking (namely, the leaked password generation algorithm for IDA <= 7.0) to solve the challenge. However, do keep a copy of IDA 7.0 at hand for convenience.
2. The Inno Setup compiler used for generating the given package is modded (for obvious reasons), effectively removed a security feature.
3. To save some guessing, the compression algorithm this installer is using internally is zlib with compression level 7. Note that the compression result is only reproducible with small files. [This chart](https://stackoverflow.com/a/54915442) might come in handy.
4. *Coming soon*

