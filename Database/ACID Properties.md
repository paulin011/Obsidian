§ Atomicity. Either all operations of the transaction are properly reflected in the database or none are. 
§ Consistency. Execution of a transaction in isolation preserves the consistency of the database. 
§ Isolation. Although multiple transactions may execute concurrently, each transaction must be unaware of other concurrently executing transactions. Intermediate transaction results must be hidden from other concurrently executed transactions. 
	§ That is, for every pair of transactions Ti and Tj, it appears to Ti that either Tj, finished execution before Ti started, or Tj started execution after Ti finished. 
§ Durability. After a transaction completes successfully, the changes it has made to the database persist, even if there are system failures.