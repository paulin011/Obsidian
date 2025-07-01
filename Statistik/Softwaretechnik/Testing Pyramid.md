![[Statistik/Softwaretechnik/Images/Pasted image 20231211114409.png]]

[[Statistik/Softwaretechnik/Unit tests]]  : When the component is about an algorithm or a single piece of business logic of the software system. 
[[Statistik/Softwaretechnik/Integration Tests]]: Whenever the component under test interacts with an external component (e.g., a database or a web service) integration tests are appropriate. 
System tests: Use a risk-based approach. What are the absolutely critical parts of the software system under test? 
Manual tests: Should only be used where requirements and specifications are incomplete or, if there is a lack of time.

# Beware of exceptions
• Development of system software (operating systems, database systems,…) may demand more system tests because a lot happens at “low level” (disk I/O, socket communication) 
• Development of Cyber-Physical systems may demand more system tests because the system strongly depends on its physical context (e.g., a water management station)