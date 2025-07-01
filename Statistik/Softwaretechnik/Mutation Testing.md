- Motivation: How do we know if we have tested enough? 
- Idea: Determine the fault detection capability by measuring the number of bugs that are detected by a test suite 
- Approach: Change small parts of the code (randomly), and check if the tests can find the introduced fault.

Mutant: Given a program P, a mutant called P’ is obtained by introducing a syntactic change to P. A mutant is killed if a test fails when executed with the mutant. 

Syntactic Change: A small change in the code that mimics typical human mistakes. Such a small change should make the code still valid, i.e., the code can still compile and run

Assumptions 
• The Competent Programmer Hypothesis: We assume that the program is written by a competent programmer, who creates a program that is either correct, or it differs from a correct program by a combination of simple errors. 
• The Coupling Effect: The coupling effect hypothesis states that simple faults are coupled with more complex faults (i.e., test cases that detect simple faults, will also detect complex faults).

Consequences on Mutant Size 
• Mutants size should be small

![[Statistik/Softwaretechnik/Images/Pasted image 20231211115805.png]]

![[Statistik/Softwaretechnik/Images/Pasted image 20231211115836.png]]


# Conclusion
Challenges 
• Automation is key: Mutants should be created automatically (based on mutation operators). There are tools for that. 
• Some mutants may be impossible to kill (i.e., a mutations score of 100% cannot be reached)
• Mutation testing is computationally expensive. The test suite must be run on every mutant.

Effectiveness 
• Studies about mutation testing have shown that mutants can provide a good indication of a test suite's fault detection capability, if the mutation operators are carefully selected, and the equivalent mutants are removed.
• A study by Just et al. shows that mutant detection is positively correlated with real fault detection. In other words, the more mutants a test suite detects, the more real faults the test suite can detect as well. 
• This correlation is independent of the coverage