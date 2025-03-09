# 6 Critical Vulnerabilities

*Upload Date: 20231130*

*Source: [https://www.youtube.com/watch?v=B8igzag_7jY](https://www.youtube.com/watch?v=B8igzag_7jY)*

# 6 Critical Vulnerabilities | Build Your Toolbox

Hey everyone,

It's great to be here today. I'm going to outline some critical vulnerabilities I've identified in smart contracts, regardless of the underlying technology.

1. **Main Points:**

*   **Smart contract security research findings:**  I've spent a significant amount of time analyzing smart contracts, leading to crucial findings across various codebases.
*   **Across all codebases:** The  vulnerabilities I've found and their associated patterns likely apply to other systems and protocols.
*   **Niche markets & protocols:**  The video discusses how some specific vulnerabilities can be exploited in niche markets.
*   **Tools and techniques:** Knowledge shared will assist in building a comprehensive security toolkit.


2. **Key Insights:**

*   **Compounding rewards:** There are scenarios where malicious actors can exploit compounding rewards systems.  This is significant because it creates a risk-free, often significant gain for the attacker.
*   **Blacklisted addresses:** Blacklisting addresses can't fully prevent exploits. There are often loopholes in protocols that malicious actors find. This means the protocol itself is often the main vulnerability.
*   **Size Delta and risk-free trades**: In many cases, attackers can increase order size or execution price without an obvious risk to yield an unfair profit.
*   **Gas limits and price impact**: There can be vulnerabilities in a protocol's architecture around transaction limitations which make the exploitable risk-free. 
*   **Transfer vulnerabilities**: Many vulnerabilities centered around transfers not considering address blacklisting or validating the appropriate balances. 


3. **Practical Takeaways:**

*   **Develop a security toolkit**: Build your personal toolkit of findings, analyzing smart contracts for similar patterns in other codebases.  This can help you proactively identify critical vulnerabilities.
*   **Understand the specific exploit mechanism for each case**:  Don't just rely on general knowledge. Dive into the details of how each exploit works to anticipate and prevent future vulnerabilities.
*   **Continuously Learn & adapt**: The threat landscape evolves rapidly, so stay updated on the latest vulnerabilities and adapt your toolbox to identify those challenges.
*   **Understand the risks with each protocol**:  Before engaging with a decentralized protocol or token, it's helpful to analyze its logic and execution environment to understand potential limitations and weaknesses that could lead to exploitation.  The specific implementation details of each protocol have inherent risks, especially given how often the protocol itself holds the greatest vulnerability.

4. **Additional Notes:** My name is Owen.  I founded Guardian Audits, which has uncovered over 100 critical vulnerabilities over the past two years allowing the prevention of those attacks and enabling improvements in security reviews, audits, and process development.


Hopefully, this summary is insightful for all of you security researchers.  Feel free to ask any questions.