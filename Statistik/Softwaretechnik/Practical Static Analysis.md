The tool analyzing the source code via [[Statistik/Softwaretechnik/Static Analysis]] can fail in 2 ways
![[Pasted image 20231213161832.png]]
If the tool is an overapproximate (sound) analysis then it will never miss violations but may say that it violates even though it does not

If the tool is underapproximate then it will never report a false positive however it will miss real violations of the property being checked