• inner structure of test object is used
• idea: coverage of structural elements within the test object 
• code translated into control flow graph 
• specific test case (concrete inputs) derived from logical test case (conditions) derived from path in control flow graph
#testing 
[[Statistik/Softwaretechnik/Control Flow Graph]]

# Types
• Function coverage (Funktionsüberdeckung): each function of a program is executed at least once during testing 
• [[Statistik/Softwaretechnik/Statement coverage]] (Anweisungsüberdeckung): each statement (LOC) of a program is executed at least once during testing
• [[Statistik/Softwaretechnik/Branch coverage]] (Zweigüberdeckung): statement coverage plus for each branching statement all branches have been exercised
• [[Statistik/Softwaretechnik/Condition coverage]] (Bedingungsüberdeckung): Every condition in a decision in the program has taken all possible outcomes at least once. 
• [[Statistik/Softwaretechnik/Multiple Condition Coverage]] coverage (Mehrfachbedingungsüberdeckung): all combinations of conditions inside each decision are tested 
• [[Statistik/Softwaretechnik/Path coverage]] (Pfadüberdeckung): each possible path through a program is executed at least once during testing

[[Statistik/Softwaretechnik/Coverage Criteria]]

Meist ist real nicht alle tests möglich ie Path Coverage zb. bei integer. Extrem viele möglichkeiten
