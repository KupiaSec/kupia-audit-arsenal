# PoP #6 - Vlad Bochok - Casually Finding a bug in OpenZeppelin Library

*Upload Date: 20230909*

*Source: [https://www.youtube.com/watch?v=gtvFhCEYBuQ](https://www.youtube.com/watch?v=gtvFhCEYBuQ)*

Okay, here is a comprehensive Markdown summary of the YouTube video "PoP #6 - Vlad Bochok - Casually Finding a bug in OpenZeppelin Library", following the interview flow and using Q&A format.


## PoP #6 - Vlad Bochok - Casually Finding a bug in OpenZeppelin Library - Summary

### Introduction

*   **Q:** Tell us a bit about yourself and what you do?

*   **A:** Vlad Bochok discusses his background, starting with his interest in mathematics and computer science in school including participating in olympics. Moved on to college to study Applied Mathematics. Now he is working for ziki sync, spending times as a security engineer and building upgrades.

### Journey into Crypto

*   **Q:** How did you get into crypto?

*   **A:** A friend introduced him to Ziki Sync, a small startup in crypto. Everything was mysterious at first. The idea reminded him rocket science from his early school days, where "Trust, don't validate" slogan intrigued him to then become an internee with them. He had an interview which focused on problem solving ability.

### Joining Metro lives (Ziki Sync)

*   **Q:** How did you Join Metro lives?

*   **A:** Job searching right after college, Alex, the CEO gave him an interview.
    Was a different type, very curious during that time about zkSync. and was different kind of interview as didn't have prior year experience but only smart enough. Then it's how I join as my first job. He has been in crypto for three years now.

### Evolution of Roles at Ziki Sync

*   **Q:** What was your evolution in the roles of key sync? When you started and what you do now?

*   **A:** Originally, he was doing rust, specifically writing Zero-knowledge proofs (circuits). There is typescript for the tooling. He was doing mainly server side work and some tooling works, while absolutely nothing in smart contracts. One day he realized it was dangerous due to large amount of funds and his lack of familiarity. Three year career in smart contract so far.

### Focusing on Security

*  **Q:** Now you focus on security. As an internee, what was the transition in roles like security wise?

*   **A:** The task was mainly concatenating code during the first month. Then it was focused a lot on data structures and algorithms he obtained from Mathematics Olympics that was brought to solidity.

* There was an understanding to optimize it very well so it can be used as a production review.

*   **A:** A shift in mindset because when he wrote smart contracts for Ziki (zksync) he was always concerned about security as the codebase will eventually be audited. So he had a motto to break it, even if it's already fine to find loopholes. Then later began to perform security reviews. And then the design review.

*   **B:** Then he has fully switched from writing smart contracts on protocol to the security team. As a result, his role became more on abstract challenging the design or improving the architecture by reporting on security.

### Developing a Security Mindset

*   **Q:** For developers trying to be more security-minded, what advice would you provide?

*   **A:**

1.  Start by understanding how Ethereum works.

    *   Read the Ethereum yellow paper to understand the APIs and SDKs.
    *   Understand the underlying computer science.
2.  Did research on ckt circuits after passing applied mathematics on plan.
3.  Also start doing something more applied instead of theoretical by trying to code smart contract and breaking even while following disclosure.
4.  Understand EVM.
5.  Run Capture the Flag(CTF)
6.  Use Slither

### About ZikiSync Architecture

*  **Q:** Can you tell us about ZikiSync architecture?

*   **A:** The aim is to scale eth, and the base idea is to add advanced cryptography of Zero knowledge proofs(ZKP) to scale Etherium.

*   Zk sync light is like a roll up where funds are deposited on layer 1 to make the cost cheap and transfers are made.

*  **Q:** Tell us about Roll Ups.

*   **A:** Roll Ups are separate blockchains connected to the main Ethereum chain. They enable proving the execution of actions while publishing all data needed to restore the state on the main chain.

* As they are interlinked the cost is low since you will be doing advanced zkp of pure computer science.

### Core ZikiSync

*  **A:** The Zk synch as previously mentioned consist of different architecture so
*   Yeah but the cool future is

*You could do something known as zero knowledge PROOFS but now validally proofs.

*   This is sounds so super cool. So I want to be in. So that's how he interviewed with Alex.

* The key point to make is that trust must not mass validate.
*   and this is super cool

*So if that was going to transition from I

*   so what was your evolution and in the

*   And just like tell is about evolution and started as the keen thing sin that will you do now?

### What zkSync Relies On

A: Relies upon all these different levels instructions yeah it will look like.
   *Can you solve the following problems and like place the all problems in part and keep the problem like in place then solve okay
Okay Alex what talking talking about no you don't have no experience it's find what Alex one point is that you're Smart enough to bigger it out so it's like so wow it's exactly what they want because on all other companies they were saying you need to one year up Java year see what enough is just different type

And yeah it's how I join metal lives on all these community said you had to interview with Alex because I can solve the is the problem and like okay okay um what um just place the problem in so it's like smaller part and another one is Alex was talking about yeah yeah you don't have experience fine

um the only you know important thing is that you're smart enough to figure it out so it's like wow it's exactly what they want because on all other companies they're saying no no I know but you need to have one year of java

one year

she plus plus what not so it was just different type

and yeah that's how I join met lives who is billing the king sin and it's my four years working as yeah three years working in crypto right now

yeap so this jobyeah I think it was so you said it was a small startup at the moment do you have an idea

of exactly what they were trying to do and how the bit it could become what that entailed back then

Not really It's just like uh when they joined

here actually, what reading a lot of books and my you asked that or work was like yeah can you read

Ethereum um you know yellow paper right like can you read about this paper write a bit of

circuits or you know just figure it out what this API and SDK so a lot of um just simple computer

science stuff But also some um

Advanced like CT circuits so I did research on both

area And start doing something on

more applied After plan

so all right cool cool so what was the your evolution and then rules from where when you started as a a

Keysing and what you do now

oh yeah and so it's like money started I wasdoing mostly rustBecause so well we had like as back as then we had um circuits written

on Rust We had A server written in draft

uh, do you can also just so that for tooling And
so what um this was a server side work. Oh, it's like absolution of course absolutely for the smart

contract and back then so it was like oh there's a lot of money inside I don't

need to keep it like I don't want to touch it Because it's so you know

dangerous and you don't have experience.

so no. no I just will do something else I

was doing thrust code and some tooling in transcript.It was really enjoying Because they just try you know you understand what is note on blockchain, do and you try

to understand

what SDK all the level of abstractions Right so

yeah it what very interesting But

I just I think that I spent like one year doing the

job and then there was my first task consolidating so it was kind of big task I spended like one month

make so much over engineering I bring a lot of data structures so everything that

they knew from Olympus. I just bring to solidity Can you I optimize it very well So you can use it in reduction
like on the review, just like people

well, why do you know bring so much complexity back then

it was like no, no, but it's fine Because

I understood what

I'm doing right now.
I was like No, I did not.

It's like uh, it's like yeah,
but so it's like it's my first

task in solidityAnd um, basically I just start from that and afterAfter

this I was working on Smart contracts for Thekissing

era That is currently deployed on my netAnd also

reporting some upgrades for Zeke Yeah, Like so It's a previous version of Ziki Sing

and who specializeIn the security side Of

things Yeah, But it was not always the case so it's like

Um, When I did aJob for protocol, so writing facility contracts, also researching for account abstraction,

message passing between chains and all of this, I was really passionate about security and I was like a bit concerned about every piece of code so it's like When I did review, I'm think that obviously if

you need to code and try you know to break it, It was intentionally uh, idea toto break the code even if it's fine.Sometimes, you can just find something very

suspicious And, You know, you wanna Go deep into it. Just like it was How I started toTo take the

security role They did a bunch of internal review Found a Couple of external bugs andSo after that There was,Yeah, and

I just Understand that it's probably mine and justProbably a month or two
Ago

*  switch from protocol team wherever writing smart contracts to a security team and was there all those that transition um What sort of mindset shift you did you have to make

I don't think that they made that need Set on Mindset Because Because
When I wroteThe smartContracts forThe protocol I was always concerned and about The security Just like

when you write something you need To be Very deep into security As

well Because After That you will have Audit you don't want to be in The Position three critical All right

AndAlso, you just want to to Know if at case You just need to deploy Contract, and without

An external Review it will be fine We all like we Then do is This, But,I impressi,This.That it Will be fine At Least so.

,It's like need

Understand Everything."  And making the Design review as Well But it's a Bit of Different Job when actually You Know Sittin Down Writing.Smart Contracts or you, WillChallenge the Ideas.You

Make reviews

* **Q:** Okay, Let's jump on the smallest bound here and try to understand the protocol, try to be

**A:** from the beginning to you know we've been there in advance.To make it's too.Try, To find it as youRead the disclosure and,
What is Suzuki seen the

*  company You work for
What what it do.Yeah so that key inc. yeah so the basic that

*   to have and with basic To what that means from side Chains

A:Not really it's to make to
All the to be is to

Then to provide all the data for to me so

* **Q:** Then, how was the slogans?

A: The is a Slogan, not Valedictorian So it's like, yeah, it's like, it sounds very cool. So I I want to, uh, to be in. The I have to interview with Alex Our CEO.
In the interview what happened interview solving the problem and yeah, yeah.I don't have experience it's fine

*  Uh to join mid road lives other

### Account Obstruction

*  **A:** I read a lot of books task was like yup can you read ethereum yellow paper or like can you read about it write a bit of circuits, and figure it out. Basically, just simple computer science stuff and also some advanced circuits.so I did research doing something a research on both areas did plans passed. It sounds super cool.
*  **Q:** How did you transition from building side smart contracts for protocol side to security and what do you do now?
*   **A:** So basically started mostly in Ross because so we had as back then we had circuits written on Rust. We have server written in drought.
 * Uh we have typescript, that is for tooling"

### The Oz Bug & Details

*   **Q:** Can you tell us about the OpenZeppelin bug you found?
 I mean tell the story.

*   **A:** So, I write the code for protocol and can only see what happened between other projects
 I just bring through so lidity and say, yeah I am optimizing very well because so, you see it in production is like holy, why do I bring so much complexity back then it was like no no there's fine.
I understand to write this account section message all area to do that yeah was very passionate about that and security and I will concern about every picture of code so I just try make you guys a fine and yeah I didn't know just see a couple of external blog and all they already there.
So a

### What are zeroKnowledge Proves?
*	A: Zero Knkowledge provers to scalling

Then uh reDisclosure Report so and
*It sounds sounds like a ROCKET science is very connected to pure computer science

### Q &A About Specifics Of The Bug

* Can you tell us about specifics please?

*   **A:**

    *   **Context:**  This was during a code review for a client. They were using OpenZeppelin's ERC777 implementation.
    *   **The Bug:** The ERC777 standard has limitations on how tokens can be used in callbacks. OpenZeppelin's implementation had functionality to check if a callback was a contract, but the check was performed *after* the token was transferred.
    *   **Impact:** This meant a malicious actor could create a contract that *didn't* actually implement the callback, but would still receive the tokens. Then, when the callback was attempted, it would fail, potentially leading to a denial of service (DoS) or other unexpected behavior.
    *   **Finding the Bug:**  He found it spontaneously. He was casually reading through a contract for our client, and then he saw the structure. That happened to be so easy to me as a math Olympic person to figure it out. And while doing that there was no big stress on my back
*   **Root Cause** You need to store Funds in which contract and