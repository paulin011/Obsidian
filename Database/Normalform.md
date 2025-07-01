1 NF: • all attributes of the relation have an atomic value.  einfach nicht mehrere werte in 


2 NF: • it is in 1NF • all non-key attributes are fully functional dependent on the primary key 

→Werte müssen atomar sein (wie 1. NF) und → Jedes Nicht-Schlüsselattribut muss von jedem Schlüsselkandidaten voll funktional abhängig sein (ist immer erfüllt, wenn Schlüsselkandidat nur ein Attribut ist) 

Abhängigkeiten so klein wie möglich

![[Pasted image 20250130151925.png]]


3 NF • it is in 2NF • there is no transitive dependency 
BCNF • it is in 3NF • for every Functional Dependency a->b, a is the super key

One reason to use 3NF over BCNF is that BCNF is not always dependency preserving. 3NF is always dependency preserving and does not result in any redundancies False. There are some situations where BCNF is not dependency preserving, and efficient checking for FD violations on updates is important, that part is true. However, 3NF allows some redundancy!! But is also dependency preserving.