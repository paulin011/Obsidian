---
cards-deck: it sicherheit
---


Was ist die Grundidee von Hashing? #card  
Hashing ist eine Einwegfunktion, die beliebig lange Eingaben auf eine feste Länge abbildet. Es dient als "Fingerabdruck" von Daten und wird häufig in der IT-Forensik und Kryptographie eingesetzt 
^1741263820880
^1741263820894

Welche Sicherheitsanforderungen müssen kryptographische Hashfunktionen erfüllen? #card  
- **Einwegfunktion (Preimage Resistance)**: Es soll nicht möglich sein, den ursprünglichen Eingabewert aus dem Hash zu berechnen.  
- **Schwache Kollisionsresistenz (2nd Preimage Resistance)**: Es soll nicht möglich sein, für einen gegebenen Wert \(m_1\) einen anderen Wert \(m_2\) zu finden, sodass \(H(m_1) = H(m_2)\).  
- **Starke Kollisionsresistenz (Collision Resistance)**: Es soll nicht möglich sein, zwei beliebige unterschiedliche Werte \(m_1\) und \(m_2\) zu finden, die denselben Hashwert erzeugen
^1741263820902
^1741263820908

Was ist ein Problem von einfachem Hashing für Passwortspeicherung? #card  
Ein einfaches Hashing speichert für gleiche Passwörter denselben Hash. Dadurch kann ein Angreifer mit einer ausgelesenen Datenbank erkennen, welche Benutzer dasselbe Passwort verwenden 
^1741263820917
^1741263820924

Wie kann Hashing für Passwörter sicherer gemacht werden? #card  
Durch **Salting**: Ein zufällig generierter Wert (Salt) wird an jedes Passwort angehängt, bevor es gehasht wird. Dies verhindert, dass identische Passwörter denselben Hash ergeben
^1741263820930
^1741263820938

Welche Hash-Algorithmen gelten als unsicher? #card  
- **MD5**: Erste Schwachstellen wurden 1994 entdeckt. Spätere Angriffe haben gezeigt, dass Kollisionen in wenigen Sekunden gefunden werden können.  
- **SHA-1**: Bereits schwach, 2019 wurde gezeigt, dass alle bekannten Angriffe auf MD5 nun auch auf SHA-1 anwendbar sind  
^1741263820946
^1741263820952

Was sind Brute-Force-Angriffe auf Hashwerte? #card  
Ein Angreifer testet systematisch alle möglichen Eingaben, um den ursprünglichen Wert zu einem Hash zu finden. Moderne GPUs können über **1 Milliarde SHA-1-Hashes pro Sekunde** berechnen
^1741263820960
^1741263820967

Welche Methoden können Brute-Force-Angriffe erschweren? #card  
- **PBKDF2, bcrypt, Argon2**: Erhöhen den Rechenaufwand durch iterative Berechnung der Hashwerte.  
- **Lange Passwörter**: Erhöhen den Suchraum für Brute-Force-Angriffe.  
- **Salting**: Erschwert die Nutzung von Rainbow Tables
^1741263820975
^1741263820982
