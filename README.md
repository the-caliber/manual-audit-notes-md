# manual audit notes markdown file.
While doing full time manual reviews I encountered the need of noting multiple things, this repo shows the md file I use to effectively note multiple things, including found issues, doubts, questions, progress and more while doing full time manual reviews. This literally works as your brain while auditing and gives you more context about your entire project and progress.

The same [manual-audit-notes.md](manual-audit-notes.md) in this repository is shown below:
1. The line with **[revisit]** prepended shows something that should be visited again or later, it can be something that you think can create a problem if some specific conditions are met after the devs fix specific issue or implementing given suggested in specific way.
2. The line with **[test]** prepended shows the point or the test that I actually want to test. It can be a edge or a POC for a confirmed vulnerability, or something that is not already covered.

```markdown
# Project Name
## Scope:  
GH link:  
Commit hash:  
 
## Flow:
1. Manual review
2. Functional testing:
    - Unit testing
    - Edge case testing
3. Automated testing:
    - ...
4. ...
 
## Resources:
1. Specification doc:
2. Whitepaper:
3. Any other documentation and links.
 
## ToDo:
*Things to do/ remaining things.*   
1. High level things about audit 
2. Developer project walk-through.
3. ...
 
## Common/Doubts/Research:
1. Relearn about specific cross chain service/protocol that's getting used.
 
## ContractName.sol
*This contains doubts/points/research/potential bugs regarding the ContractName.sol*
1. Confirmed issue 1.
2. Confirmed issue 2.
    ### Doubts/Research:
    1. Checking specific formulas.
    2. Checking specific doubt.
    3. Check the subtraction on L453 can be a problem.
    4. [revisit] Revisit something based on the suggestion given.
    * Testcases:  
        1. [test] User should be able to stake.
        2. [test] Multiple users should be able to stake.
        3. [test] ...
 
## ContractName2.sol
*This contains doubts/points/research/potential bugs regarding the ContractName2.sol*
...
 
---
## Questions for developers:
1. Explanation for formulas.
2. Questions about intended logic.
3. ...

```
