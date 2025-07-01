Grundlegende Annahme komplexe Probleme sind besser lösbar wenn in Komponenten zerteilt

1. Modellierung der Alternativen
	können gegeben sein oder müssen gesucht/generiert werden
	bei zu vielen alternativen muss man sich beschränken
	wie viel energie/zeit steckt man in die alternativensuche
	|
	Alternativen so simpel wie möglich halten BSP:
	A:	a = (Überstunden), b = (Neueinstellung)
	B:	a = (alles mit Überstunden), b = (keine Überstunden
	und Neueinstellung), c = (Überstunden und Neueinstellung)
	|
	Bei Mehrstufigen alternativen nennt man es "Strategie"
	![[Pasted image 20240611114907.png]]
	(Ausnahme ET-Baum, einstufige Alternative = Strategie)

2. Modellierung der Umwelt
		Unsicherheiten z.b. Wetter,Euro USD kurs
		Entscheidungen unter unsicherheit/Risiko
		Kann meist vernachlässigt werden sollte jedoch stets modelliert werden
		**Wird meist über Wahrschenlichkeiten abgebildet.**
			Wahrscheinlichkeitsaxiome Kolmogoroff
				1. p(si)≥ 0 für alle i.
				2. Σ p(si) = 1 (der sichere Zustand erhält die Wahrscheinlichkeit 1)
				3. p(si oder sj) = p(si) + p(sj) (die Wahrscheinlichkeit, dass irgendeiner von mehreren
				sich gegenseitig ausschließenden Zuständen eintritt, ist der der Summe der
				Wahrscheinlichkeiten der Zustände.
		Bei zusammengesetzten Ereignissen: Szenarien
		 Beispiel „Maschinenplanung“
		• Maschine A є {funktioniert, funktioniert nicht}
		• Maschine B є {funktioniert, funktioniert nicht}
		• Geschultes Personal є {1,2,3}
		• 2 x 2 x 3 = 12 mögliche Szenarien
		|
		