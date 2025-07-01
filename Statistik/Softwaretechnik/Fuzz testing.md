Fuzz Testing

Negative software testing method that feeds
malformed and unexpected input data to a
program, device, or system with the purpose of
finding security-related defects, or any critical
flaws leading to denial of service, degradation of
service, or other undesired behavio

Terms: Fuzzer: Program/ Framework that generates fuzz tests.

Crate test cases that make the System Crach

# How to generate fuzzed inputs?
- Mutation-based Fuzzing: Creates permutations from example inputs (e.g., replacing or appending characters). Since mutation-based fuzzing does not consider the specifications of the input format, the resulting mutants may not always be valid inputs.
- Generation-based Fuzzing: Takes the file format and protocol specification of the SUT into account when generating test cases. Generative fuzzers take a data model as input that specifies the input format