# 28 Ways To Miss Vulnerabilities In A Smart Contract Audit

*Upload Date: 20230326*

*Source: [https://www.youtube.com/watch?v=f--w08g7lyU](https://www.youtube.com/watch?v=f--w08g7lyU)*

# 28 Ways to Miss Vulnerabilities in a Smart Contract Audit

Hey everyone,

I'm really excited to share this thread on 28 ways to miss vulnerabilities in a smart contract audit.  It's been a while since I put this together, and people really liked it.  This thread is designed to often give you a bunch of tips on how to actually find vulnerabilities in an audit, of course, but it's not often that you hear about how to miss them.

## 1. Main Points

* **Detailed code review is paramount:**  Lack of thoroughness in code analysis is a major way people miss critical issues.
* **Missing edge cases:** Auditors often focus on the straightforward path, forgetting rare or unusual inputs/conditions that trigger bugs.
* **Blindly trusting external calls:** Failing to validate external calls and ensuring they are safe is a major risk.
* **Neglecting test cases:** Omitting or inadequately testing edge cases in your test suites.
* **Not utilizing existing documentation:** Missing out on crucial information that the code's documentation may provide.
* **Incomplete dependency checks:**  Potential issues in smart contracts' dependencies are not thoroughly explored.
* **Problems with tokenomics:**  Issues regarding token distribution, minting, and transfer mechanisms are often overlooked.
* **Inattention to specific token types (ERC-20, ERC-777):** Failure to account for the unique behaviors of different token standards can be disastrous, especially with wrapped tokens.
* **Ignoring gas optimizations:** Underestimating the significance of gas optimizations and their relation to the protocol's security when auditing.
* **Insufficient testing of variable interactions:** Incorrect or insufficient handling of interaction between variables to trigger unexpected behavior.
* **Missing validation mechanisms:** Overlooking critical validation points (e.g., checking against limits) to anticipate attacker exploits.
* **Lack of collaboration:** Auditors who operate in isolation may miss crucial viewpoints or different attack factors.
* **Incorrect assumption(s):**  It's easy to make unproven assumptions about how the code works or what is expected to happen.
* **Not considering other aspects of the overall system:** A failure to understand how the smart contract fits into the wider protocol or system.
* **Missing re-entrancy checks:** Underestimating the danger of re-entrancy exploits resulting from external calls.
* **Incorrect scrutiny for edge cases:** Ignoring seemingly minor issues that when combined could lead to a major exploit.
* **Lack of careful reading of comments:** Ignoring seemingly unimportant comments which can contain crucial context about the code or assumptions.
* **Overlooking special cases:** Failure to test unusual scenarios.
* **Insufficient testing of the incentive structure (governance, rewards):**  Neglecting to account for the incentive structure (both for attackers and developers) and potential misalignment of goals, possibly leading to exploitation.


## 2. Key Insights

Each of these 28 points is a common, yet subtle, way auditors can miss crucial aspects of a smart contract's security.  The real insights are in understanding the *why* behind these errors.  It's not just about the technical specifics, but the mindset an auditor brings to the task.  Are they actively looking for vulnerabilities, or are they just trying to find one or two and go home?  A good audit needs a mindset to really dig in and understand the code from all angles, to understand the potential exploit paths.  It's about meticulousness and critical thinking, and often the best auditing is a team effort, bringing different perspectives and challenging assumptions. This list isn't exhaustive, but it represents some of the pitfalls to consider.

## 3. Practical Takeaways

* **Thoroughly review the smart contract code:**  Take your time, focus on every line, don't gloss over anything.
* **Identify edge cases and boundary conditions:**  Develop thorough test cases that cover every possible input combination.
* **Carefully validate external calls:** Actively look for re-entrancy vulnerabilities and verify external calls handle errors effectively.
* **Incorporate different perspectives:**  Collaborate with colleagues, have peer review, have another set of eyes.
* **Challenge existing assumptions:**  Don't just accept what is stated without verification.  Ask "why?" for every design decision.
* **Read documentation and comments:**  These are important sources of context, assumptions, and expected behavior.
* **Understand the complete system:**  Don't just look at the contract; understand its role and interactions with other parts of the protocol/system.
* **Use comprehensive testing methods:**  Fuzz testing and penetration testing can be valuable tools in digging into a system's behavior from an adversary perspective.


## 4. Additional Notes


This list is not exhaustive but is meant to stimulate thought.  The core lessons here are: smart contract auditing requires diligent care, questioning assumptions, and collaboration. A deep understanding of the code from all angles is critical. Be comprehensive in your review approach. This can avoid missing significant vulnerabilities.  You won't always find every single one, but these points will increase your chances of high-impact ones.