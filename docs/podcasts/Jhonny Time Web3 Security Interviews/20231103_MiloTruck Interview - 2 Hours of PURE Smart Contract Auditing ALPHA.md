# MiloTruck Interview - 2 Hours of PURE Smart Contract Auditing ALPHA

*Upload Date: 20231103*

*Source: [https://www.youtube.com/watch?v=g5Obbl0cAwk](https://www.youtube.com/watch?v=g5Obbl0cAwk)*

Okay, here's the interview summary in a Q&A format, from my perspective as MiloTruck, diving deep into the Web3 security space:

**MiloTruck Interview: 2 Hours of PURE Smart Contract Auditing ALPHA**

**Introductions**

**Q:** Brandon (MiloTrack), welcome to the show! Can you tell us about your background and how you got into computer science and hacking?

**A:**   Glad to be here!  It's my first interview.  My introduction to security wasn't web3, but Capture the Flag (CTF) challenges.  I got into it through a senior in high school.  It was a cool thing to possibly earn money while still a student.  I specialized in binary exploitation and reversing – finding bugs in binaries by reversing compiled code.  I did CTFs all through high school, and that's how I got started in security.

**Diving into CTFs**

**Q:** You mentioned binary exploitation and buffer overflows in high school, that sounds pretty hardcore. Did you learn those skills beforehand, either at school or online?

**A:** In secondary school (high school) I did take computer science, but it was very basic. My senior introduced me to the CTF community. The Singapore CTF community is quite active. I spent a lot of time grinding online, learning from write-ups. I actually learned C through reading decompiled code. It was horrible at the beginning, when de compilers don't give nice codes.

**Early Career**

**Q:** Okay, so where did you go from there?

**A:** After junior college(High school) I interned at StarLabs, a Singapore security firm, doing traditional cyber security research—Windows fuzzing. Not hugely successful, but it introduced me to finding bugs in real software, not just constructed CTF challenges. Then I had to do my Mandatory Military Enlistment. They sent me a C4 link. So during my time in the Air Force and I was doing Kod Arena, which was real bags. This was in 2021 during bull market season. Smart contracts and web tre were booming.

**Web2 vs. Web3 Security**

**Q:** You've got a lot of experience in traditional cyber security. Do you think it gives you an advantage in web3 and Auditing Contest?

**A:** Initially, I didn't think so because it's totally different. Web2 is memory correction, while Solidity is memory safe. Over time, seeing people like H discovered, I think it *does* help. It's more a mindset thing. You are familiar with the idea of sitting down and finding bugs, Being able to keep looking untill you find the vulnerability. If you looking for a check you are looking to how the check works great!, but when you're looking for security you understand and look at how the can be bypassed. When doing x86 assembly there is a similarity in VML so the stack memory concepts are the same. Although they are different they are similar concepts . This idea carriers on ever when you change from web 2 to web 3. 
    
**Learning Web3**

**Q:** What was your process to learn Web3 security and solidity?

**A:** I started with CryptoZombies to learn basic DeFi concepts like ERC20s and NFTs. Then I did three CTFs: Capture the Ether, Ethernaut, and Damn Vulnerable DeFi. Damn Vulnerable DeFi is very good, as it teaches you real world exploits. Back then there weren't courses so I just did codarina contest directly.

**First Contest Strategies**

**Q:** Did you jump right into CodeArena contest or did you do some research?

**A:** I jumped right into contest by a process of: read code, look up similar past protocols and apply knowledge from audits reports to current audit, and filter all the reports. Applying the filter knowledge instantly to contest or a current audit makes it more effective. So I don't recommend just studying without applying it in contests, and that's not something I recomend. Just going to a conest is what I recomend.

**First Contest and Early Results**

**Q:** Where was it something that you did like part time and from some point do you really like really improve from making 200 bucks and being in like 13 in the list?

**A:** I think my first decent thing was in Chain Link, around June this year. So from military to Chain Link there was one year.

**Q:** How were the results of your first contest?

**A:** The payout was low, maybe $100-$200. I remember getting $250 , but this good as I was making $700 per month in the army.  I mostly focused on the findings themselves anyway.

**Q:** Okay, what did you do after the contest to get better?
**A:**  Mainly look for previous report. I didn't look through back stage back then, maybe I'll suggest it now, but I did back then.

**The Turning Point**

**Q:** You leveled up! Can you explain how you improved so dramatically??

**A:** I'm looking at the history here.. It took like one year and few months. For example, I did a contest in August Leo where where they did the unchecked plus plus. After Franken Coin I went on holidays.

My shift was from May june. After like half a month I told myself, after chain ling ccip contest I'm gonna sit down and find every bug. It helps me to get a decent place. With that I understood the entire protocol.

**Auditing Methodology: Three Phases**

**Q:** Awesome. What did you learn from ChainLink that you applied afterward? You conquered lou and Lance protocol how did you do it?

**A:** Then ccip did show me That understanding protocol is crucial before you start to find bags.

I tell auditor is three phases:
1.  **Understanding the product thoroughly:** go through every single line of code and to understand how the protocol works. Even if you are looking and you have some ideas you just write a audit tag.
2.  **Ideating or attacking:** to think and to try to find potential bugs in functions or identify comlicated areas that increase the chanches of bugs.
3.  **Reporting:** An under discussed finding; write more high quality reports or as high quality as possible, not only to me but also for the judges and for the ones who get a private audit

This really makes sense.

**Reporting is Key**

**Q:** Why is the reporting phase so important? 
**A:** Everyone just doesn't include good reports and does a lot of code snippers from the web. There are few sentences to that are bugs. When a judge these kinds of reports I invalidate the findings as insufficient proof. When u write this PC helps a lot when you understand by all of the coaches sell

Writing good quality reports also does help you build your portfolio a lot better because when you are looking at clients. The reason you should write is to show case and show your skill set in terms of skill set is not bug fighting, but explaining them clients which is what is important to demonstrate to clients and you have to write out high quality reports as high

**The Role of Proofs of Concept (POCs)**

**Q:** Do you attach POCs for every high or medium risk finding? Is it mandatory?

**A:** Mandatory? No, it is coding is not mendatory. Previously, if you find a high risk you has to provide the PC to prove it that you know what you are taking about. Unless, I cannot write a PC it has to be super obvious or just simple, or that I don't write that one. Some things that might look obvious to you and as a as an auditor not obvious to a judge protocol team because they are looking at code from a different stand. All of these reasons are reasons to include PC's.

**Has static analyzers for to find backs automatally, but then you decided to leave that and can you tell us a beat about it

I used to write static analyzers. I run it on every contest and got 100 or 200 this is when to find back

**Manual Auditing vs. Automation**

**Q:** Do you believe that static analyzers will uncover more advaced bugs?
**A:** Not always. Static analysize is a multiplier, it's not a complete replacement. I could have used it for for human effort is more like a black and how is this automated in the web to where this is the where value Static analyze Fussy because it increases

**Q:** You said you currently working on a wildcat protocol where you are writing tests.
**A:** I would fast all the math functions individually to make sure to confirm that what I am seeing and what my ideas of the function is correct to assemble.

**Advice for New Auditors**

**Q:** If you can give three pieces of advice to someone starting out in audit contest, what would they be?
**A:**
1.  **Focus on one contest at a time** for as long can. Because because the formula prioritizes rare bugs and it is statistically unlikely a single auditor will find everything in a single code base, focus on a contest in it's entire to try find and to commit time.
2.  **Always think that there is a bug to to be found, and that code isn't bug free:** The idea is you should always think that there is back it to to be found how do you you think that if there is you can find something and you will always keep searching searching in there will also make the increase of the chance that you will actually something by based on psychology
3.   **Be Patience:** Because you also need to actually improve everyday because you don't just grind grind because other people will will keep posting things that make me think that you don't know how to prove to make that.

**Immunifi and Bug Bounties**

**Q:** Do you have any experience with immunify or buck bounties but what are you mostly doing now
**A:** A lot of my time for a contest in c4 and head but I am due to buck bounties on the side when I have small gaps of time in between AIT contest so I I do a lot for this in but that is okay I have one hide that I was paid from the rust are like mediums are there the rest a lot so i would say 5050% I did it downgrade validated but I didn't get downgraded. I never wanted to immunifi anymore, I did it as often as possible and then they just want everyone.

**Q:** What do you get what's your thoughts?
**A:** With the high-risk that that you will get paid and by is that when you follow get through the first outcome is that you get except but the second outcome is that you report that but the severity gets denied and a third out come is the worse part about of all of it

**Selecting Contest and Bug Bounty Targets**

**Q:** Did you have did how do you pick with and did you choose to go to AIT contest in and do you pick the projects that you're going to back bonus.
**A:**
1.  **Focus on where you are strong:** the protocols more for business for something novel the chances are that there is many competition and also because you want the audit is that can go to something that will give the less come back to you so what what you wanted you should look as all the test and then you see which one seems to seems that they will have less contention.
2.  **Back Bounties:** B back but I am more the more logic that goes with business and logic things that do will be involved in also what the does the audit report the the previous audit to see like how heavily are they audited I do a lot of research

**Auditing Firm Job Offers**

**Q:** Did you get any job offers from Auditing firms obviously you know the tell that you drag attention I soon you got some office I think
**A:** A lot of people say oh I see no a but I soon got the skill. But it is still so hard right now. But mainly because I didn't find the I couldn't fit the right. I can't really work full time forever and then.

**Freelancing vs. Full-Time Employment**

**Q:** Do you even get any offers from Auditing firms?
**A:** The constant consideration with always comes, that if you are a firm that is a contract obligated to the.

**Q:** What would you prefer to do in those conditions?
**A:** But as a freelance is that a chance that you can are in high you you also make a million dollar and if anything that is in the market this you get hired quicker if anything.

**Contacting You**

**Q:** One what way do people reach out to you through Twitter telegram do

The best to do on Twitter to reach out questions what you are that can make and I also saw what the what what what I thought that maybe what I am doing maybe you are going to get high quick.