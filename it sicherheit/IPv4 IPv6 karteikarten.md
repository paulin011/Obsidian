---
cards-deck: it sicherheit
---


Was ist das **TCP/IP-Schichtenmodell** und wozu dient es? #card  
Das TCP/IP-Schichtenmodell strukturiert Netzwerke in aufeinander aufbauende Schichten, die der jeweils oberen Schicht Dienste anbieten. Es abstrahiert die physischen Spezifika, ermöglicht Kommunikation über diverse Infrastrukturen und Protokolle und bietet Flexibilität bezüglich Geschwindigkeit und Zuverlässigkeit der Übertragung.
^1741272099547

---

Welche vier Schichten gibt es im **TCP/IP-Schichtenmodell**? #card

- **Anwendungsschicht** (Application)
- **Transportschicht** (TCP/UDP)
- **Internetschicht** (IP)
- **Netzzugangsschicht** (Network Access)
^1741272099550

---

Was ist die Aufgabe der **Internetschicht** im TCP/IP-Modell? #card  
Die Internetschicht leitet Datenpakete mithilfe von IP-Adressen über Netzwerke hinweg weiter (Routing). Dies geschieht verbindungslos („best-effort“), d.h. ohne Erfolgsgarantie oder Kontrolle.
^1741272099554

---

Was versteht man unter dem Begriff **Encapsulation**? #card  
Encapsulation bezeichnet das Prinzip, bei dem jede Netzwerkschicht Daten der höheren Schicht in ein eigenes Protokoll verpackt und zusätzliche Header hinzufügt. Bei Empfang erfolgt Demultiplexing, wobei jede Schicht die Daten auspackt und der jeweils höheren Schicht übergibt.
^1741272099557

---

Was bedeutet die Abkürzung **CIDR**? #card  
CIDR steht für **Classless Inter-Domain Routing** und bezeichnet die klassenlose, flexible Vergabe und Darstellung von IP-Adressen mithilfe variabler Subnetzmasken (z.B. 192.168.1.0/24).
^1741272099560

---

Was ist der Unterschied zwischen **IPv4** und **IPv6**? #card

- **IPv4** verwendet 32-Bit-Adressen (z.B. 192.168.1.1), insgesamt ca. 4,3 Milliarden mögliche Adressen.
- **IPv6** verwendet 128-Bit-Adressen (z.B. 2001:0db8:85a3::8a2e:0370:7334), dadurch nahezu unbegrenzter Adressraum. ^1741272099564
^1741272099566

---

Welche **IP-Adressbereiche** gelten als privat nach RFC1918? #card

- 10.0.0.0 bis 10.255.255.255 (Klasse A)
- 172.16.0.0 bis 172.31.255.255 (Klasse B)
- 192.168.0.0 bis 192.168.255.255 (Klasse C)
^1741272099570

---

Welche vier Typen von Adressen kennt IP? #card

- **Unicast** (ein Empfänger)
- **Multicast** (eine Gruppe von Empfängern)
- **Broadcast** (alle Teilnehmer eines Netzwerks)
- **Anycast** (ein Empfänger aus einer Gruppe)
^1741272099573

---
