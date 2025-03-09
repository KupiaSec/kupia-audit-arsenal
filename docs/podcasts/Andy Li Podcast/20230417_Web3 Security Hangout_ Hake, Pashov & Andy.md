# Web3 Security Hangout: Hake, Pashov & Andy

*Upload Date: 20230417*

*Source: [https://www.youtube.com/watch?v=L1r6ZRnTAWE](https://www.youtube.com/watch?v=L1r6ZRnTAWE)*

Here's a summarization of the YouTube transcript provided, following an interview format and focusing on the core information from the questions and answers.

**Web3 Security Hangout: Hake, Pashov & Andy - Summary**

**Part 1: Audit Company Structure**

Q: How do auditing groups in Web3 have a formal work setup or process?
A: At Sigma Prime, they focus on writing Proofs of Concept (PoCs). The audit is divided into two parts: a comparable part to other firms, and a secondary part where they implement extra test and write PoCs

Q:Is auditing touching one or up to four auditors?
A: For Sigma Prime, it involves multiple auditors working as a team bouncing ideas with each other before additional tasks

**Part 2: Spearbit Auditing Process and Report Format**

Q: Can you share how Sparebit(auditing form), conducts the auditing process. what their auditing report looks like, and how collaborative the report process is?
A: Spearbit's auditing process in GitHub involves code changes within a pull request. Anyone can immediately comment on the pull request
The entire code is present via pull requests in GitHub, so whoever identifies an issue promptly comments on it stating the specific problem with suggested solutions (the changes, all the code is revieweable in github).
It's collaborative, but speed is important because it can be efficient, so the first one finding the most finding the most issues usually 'wins
The auditor finding the most issues does not matter in the end because its team work
They have a tool that will generate automatically a report showing the issues within GitHub itself(from those pull requests)

**Part 3: Public vs. Private Audits and Scaling Audits**

Q: What are your opinions on private audit to public audits?
A: Right now, for private audits, Andy clones code locally vs code on chain. Private pull requests formality can hinder back and forth communication, and collaboration to find solutions

Q: (What about) setting up a structure for private audits?
A: Hake does everything manually, is a solepreneur and has an overhead process so he is focusing on auditing from the command line instead

Q: How does one scale their solo auditing firm and how do you include security researchers in your audits; and pay a share of awards to QA work?
A: He has been doing audits with some real life (web3 friends).
Andy has a model where his friends do the auditing alongside him and "find duplicates". He still pays them the reward of the code4rena reward pot for these audits

Q: What are 2023 goals for your Web3 Security audit company?
A: My point of view is from what I am getting lately because right now I am not actively approaching protocols so i can only show you from my perspective that they are getting too small-budget clients mostly.
Right now the landscape is that while it is passion there are less audits.
NFT budget is increasing so that's a trend"

**Part 4: Projects, Standout Audits, Top Vulnerabilities:**

Q: Can you talk about the types of audits you've been doing?
A: Most recent audit was dealing with NFT games using Layer0
Finding NFT vulnerabilities can be easier because general audiences want to have fun
It has been harder to "rug people" - or do economical stuff due to the "private key issues", with the D5 protocols

Q: What to do from a developer standpoint, to improve a code base, specifically in web 3.0?
A: Validate Chainlink Oracle inputs from attacks such as high severity. Always have a low budget plan and implement it.. There is a lower budget for projects run by solepreneurs, use automated services to get started quickly

**Part 5: Team Auditing Benefits and Collaboration**

Q: Do you think there's benefit from that compounding fact of of just auditing with other auditing goups, just being able to bounce ideas off?
A: The main benefit of team audits is the power of confirmation of findings instead of making the report just after fully fleshing out a vulnerability.
Pull-requests have their benefit in making all members to see it, and also the protocol gets "free value"

**Part 6: Tooling and the future of remote collaboration in web3 security**

Q: Is everyone doing this type of github collaboration setup? In particular, how about making it all on chain?
A: At sparebit it starts manually but everything from report generation is automated as much as possible

**Part 7: Code Arena / Code4Rena and the future of private Security Research**

Q: Do you feel that the current model of doing code4rena are working good enough or the model needs an update? Also a question about the legal side if you can share an opinion
A: Yes all good except with time you get too much exposure to the code and there can come times that one might see a new exploit because of prior knowledge
"I hope to start something similar but for private audits" - he's personally done C4 but not solo

**Part 8: Advice for New Auditors, Important Areas, Future Trends:**

Q: Any advice for new auditors?
A: Yeah be methodical create a check list and make sure USDT and USDC tokens with multiple implementations on all implementations are tracked

Q: About this final part (of the stream), do you have in mind what should this contain from the technical aspect and what do people want to know?
A: A private key compromise is probably has been the biggest one in the past. so you can add security, and even all these things you can do to try to get your staff sorted" -

With so many chain links available to take away smoking signals that was kind of our biggest things that that were helpful and useful.

Q: Final comments?
A: ""we kind of get into the details
well the whole year will be web.3 there still provide it
we started really well"
it has become a very complex D5 logic" --  - "so all of the best there are so many protocols is
it important I know a lot of people
that is what's important to me this collaborative mean"  - well the end product what's
what's important -- It will be automatic report. This will give 4x. I feel
Like in that report from GitHub is very nice there is some good points.
It has been just to the Sigma
All right so I do think that if there are all these changes and codes. so let's go"