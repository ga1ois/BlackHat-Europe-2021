# BlackHat-Europe-2021

All materials about our Black Hat Europe 2021 presentation will be released here.

From Logic to Memory: Winning the Solitaire in Reparse Points

Abstract

In recent years, two types of reparse points: mount point and symlink are frequently used in file redirection vulnerabilities in Windows system services. Hundreds of logic vulnerabilities (from permanent DoS and info leak to privilege escalation) were discovered under this attack surface. Besides fixing those vulnerabilities, Microsoft also released many mitigations to make this bug class harder and harder to exploit successfully and stably. This presentation shows a 0-day logic vulnerability which bypasses all current mitigations with undisclosed exploit techniques and wins Windows EoP category in Pwn2Own 2021. All details, from finding the bug in one day with a unique vulnerability discovery strategy to winning a seemingly impossible race window stably, will be covered.

But the story does not end here. Microsoft stopped granting bug bounties to that bug class and is releasing more and more mitigations to kill the bug class fully. It seems to be the end of the reparse points era, but things are not always that easy. There are over fifty types of tags in reparse points, mount point and symlink are only two of them. After exploring other tags in reparse points, several memory corruption EoP bugs were found among them. Interestingly, in our findings there is one function containing three kinds of bugs: out of boundary read, out of boundary write and race condition; more interestingly, the same vulnerable function appears in several different Windows components. We reported our findings to Microsoft and fastly got bug bounties from them to reward our new discoveries. Memory corruption EoP bugs in reparse points could lead to the native code execution in Windows system services and escalate the privilege to SYSTEM directly, all previous and future mitigations against logic EoP bugs in reparse points are useless. This presentation unveils this new and less noticed attack surface for memory corruption EoP bugs in reparse points.
