Analysis of all possible paths in the [[Alte semester/Softwaretechnik/Control Flow Graph]]
Checking properties at each program points

Abstraction that define an abstract domain that considers only the values/states relevant to the property
Testing the Abstract statet instead of any concrete values in all possible paths of the program.

Program Points Every edge in a control flow graph denotes a program point. 
Program points characterize the possible conditions that hold before entering and after leaving a node in the [[Alte semester/Softwaretechnik/Control Flow Graph]].

For every node in the [[Alte semester/Softwaretechnik/Control Flow Graph]]: 
• Evaluate the state before entering the node 
• What is the possible state after leaving the node (apply the transfer function)? 
Iterate over all successor nodes in the [[Alte semester/Softwaretechnik/Control Flow Graph]] until no program point’s state changes anymore.
Result: A state in every program point
![[Pasted image 20231213163641.png]]
![[Pasted image 20231213163720.png]]
![[Pasted image 20231213163745.png]]
CFG = [[Alte semester/Softwaretechnik/Control Flow Graph]]