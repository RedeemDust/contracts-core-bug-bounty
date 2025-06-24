find vul in the codebase for immunefi bug bounty program. dont assume bug. every bug should fall into scope and able to write a POC
some how hart hat doesnt support fork so we cna't fork in hard hat can only do blank state most

Haven1 is a REKT-Resistant EVM L1 blockchain meticulously designed to prevent onchain hacks, scams and rug pulls through network-level safety guardrails that connects verified users to verified builders so they can interact with complete peace-of-mind.
https://docs.haven1.org/

Critical
Manipulation of governance voting result deviating from voted outcome and resulting in a direct change from intended effect of original results

Critical
Direct theft of any user funds, whether at-rest or in-motion, other than unclaimed yield

Critical
Direct theft of any user NFTs, whether at-rest or in-motion, other than unclaimed royalties

Critical
Permanent freezing of funds

Critical
Permanent freezing of NFTs

Critical
Unauthorized minting of NFTs

Critical
Predictable or manipulable RNG that results in abuse of the principal or NFT

Critical
Unintended alteration of what the NFT represents (e.g. token URI, payload, artistic content)

Critical
Protocol insolvency

High
Theft of unclaimed yield

High
Theft of unclaimed royalties

High
Permanent freezing of unclaimed yield

High
Permanent freezing of unclaimed royalties

High
Temporary freezing of funds

High
Temporary freezing of NFTs

Medium
Smart contract unable to operate due to lack of token funds

Medium
Block stuffing

Medium
Griefing (e.g. no profit motive for an attacker, but damage to the users or the protocol)

Medium
Theft of gas

Medium
Unbounded gas consumption


Web3 PoC Guidelines: 
Most projects, especially for smart contracts, require a PoC for submissions to be valid and in-scope. Without a PoC, it can sometimes be impossible to tell whether there’s any bug at all, or most importantly, whether there’s any impact. A well-written PoC makes it unambiguous that there’s a bug and that an impact is real. Once a project receives a submission with an excellent PoC, they are able to analyze, respond, and pay out a big bounty much faster. 
The smart contract PoC should always be made by forking the mainnet using tools like Hardhat or Foundry. If forking the mainnet state is not feasible, using the project’s existing test suite is an acceptable alternative. However, the test conditions must accurately reflect the state of the deployed code. If the conditions do not match, the project may request additional PoCs to ensure accuracy.

The PoC should contain runnable code for the exploit demonstration. Screenshots of code are not acceptable. The whitehat can choose any framework or language to write a PoC. The whitehat should mention all the dependencies, configuration files, and environmental variables that are required in order to run that PoC, as any other requirements to run the test.

PoCs should have clear print statements and or comments that detail each step of the attack and display relevant information, such as funds stolen/frozen etc.

The whitehat can upload the PoC containing all the configuration files directly to Google Drive and share the link in the submission on the Immunefi Dashboard.

Alternatively, if the PoC is simple enough that it doesn’t require any configuration files, then it can be shared in the submission itself by pasting out the code in the comment.

Additionally, the whitehat should also ideally determine and provide data on the amount of funds at risk, which can be determined by calculating the total amount of tokens multiplied by the average price of the token at the time of the submission.

Whitehats must comply with any additional guidelines specified by the bug bounty program the whitehat is submitting a bug report to. 
If whitehats do not follow the guidelines, their reports may be closed. 

 

Web3 PoC Rules: 
Do not test on public testnet or mainnet.
If you want to run a DoS attack to prove a vulnerability, you must ask for and receive permission from the project in the Dashboard before doing so.
Do not submit a partial or incomplete PoC.
Violation of any of these rules will, in almost all cases, result in an immediate and permanent ban from the Immunefi platform. 

Example of an excellent web3 PoC: https://github.com/immunefi-team/polygon-transferwithsig

