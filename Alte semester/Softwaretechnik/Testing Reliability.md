Reliability of the program logic
• How does a system handle unexpected inputs?
• General approach: Use random input values
•  Realism or probability of these input values is
irrelevant

Random testing
• Testing with random and independent inputs from the input domain of a program
•  Random testing can generate probabilistic
guarantees about the failure likelihood of a system (e.g., testing 23,000 random inputs without error
guarantees that a system does not crash more than once in 10,000 runs with a probability of 90%)
•  Challenge: How to define the expected output?
•  [[Alte semester/Softwaretechnik/Fuzz testing]] is a special form of random testing

Reliability of the underlying infrastructure
•  How does a system handle errors in the
underlying infrastructure (e.g., server
crash)?
•  Important for distributed systems (e.g.,
cloud services)
[[Alte semester/Softwaretechnik/Chaos Engeneering]]
