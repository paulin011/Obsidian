---
cards-deck: it sicherheit
---



**Was versteht man unter IT-Forensik (Digitale Forensik, Computerforensik)?** #card  
Die IT-Forensik umfasst Methoden zur Untersuchung und Beurteilung verdächtiger Vorfälle oder Handlungen in Bezug auf IT-Systeme, basierend auf digitalen Spuren, die erfasst, gesichert, aufbereitet, analysiert und sachverständig beurteilt werden. Ziel ist es, digitale Datenspuren so aufzubereiten, dass diese vor Gericht verwendbar sind.
^1741265891356

---

Was ist das Ziel der **IT-Forensik**? #card

- Erfassung und Sicherung digitaler Spuren.
- Nachvollziehen von Abläufen, Tatbeständen und Tatmustern.
- Klärung der W-Fragen (wer, was, wann, wo, wie).
- Ermittlung von handelnden Personen oder Verantwortlichen.
^1741265891382

---

Was versteht man unter der **Locard’schen Regel** in der IT-Forensik? #card 
Die Locard'sche Regel besagt, dass jeder Kontakt zwischen zwei Objekten (z.B. Täter, Opfer, Tatort) wechselseitige Spuren hinterlässt.  
In der IT bedeutet dies, dass jegliche Aktionen eines Täters auf einem IT-System digitale Spuren hinterlassen (z.B. Log-Dateien, gelöschte Dateien, Dateisystemeinträge).

---

Was ist **Forensic Readiness**? #card 
Forensic Readiness bezeichnet die präventiven Maßnahmen zur Vorbereitung auf IT-forensische Untersuchungen. Ziel ist es, sicherzustellen, dass im Falle eines Sicherheitsvorfalls digitale Beweise schnell und vollständig gesichert werden können.

---

Was sind typische **digitale Datenspuren**, die in der IT-Forensik analysiert werden? #card

- Logdateien
- Temporäre Dateien
- Gelöschte Dateien
- Backups
- E-Mails und deren Anhänge
- Netzwerkverkehrsdaten
- Hauptspeicherinhalte (RAM)
- Browserhistorien
^1741265891392

---

Wie werden **digitale Beweise** üblicherweise gesichert? (Imaging) #card 
Digitale Beweismittel werden meist durch eine blockweise, exakte Kopie (Image) des Datenträgers gesichert. Ein typisches Tool dafür ist `dd` (disk dump) unter Linux. Das Ziel ist die unveränderte Sicherung des Originalzustands.

---

Welche Arten von Daten unterscheidet man hinsichtlich ihrer Volatilität in der IT-Forensik? #card

- **Flüchtige Daten**: Existieren nur temporär (z.B. RAM-Inhalte).
- **Fragile Daten**: Können beim Zugriff verändert werden (z.B. Zeitstempel).
- **Temporär zugreifbare Daten**: Sind nur zeitweise verfügbar (z.B. Netzwerkverbindungen).
^1741265891399

---

Was bedeutet **Post-mortem-Forensik**? #card 
Post-mortem-Forensik bezeichnet die Analyse von Systemen nach deren Abschaltung, also ohne, dass aktive Prozesse laufen. Ziel ist, den Zustand eines Systems nach einem Vorfall rekonstruieren zu können.

---

Was bedeutet **Live-Forensik**? #card 
Live-Forensik umfasst die Untersuchung aktiver Systeme, um laufende Prozesse, Netzwerkverbindungen und temporäre Daten zu erfassen. Diese Vorgehensweise ist komplex, da sie die untersuchten Systeme verändert und gut dokumentiert werden muss.

---

Was umfasst ein gutes **Sachverständigengutachten in der IT-Forensik**? #card 
Ein gutes Gutachten folgt einer festen Struktur vom Formalen (objektive Feststellungen), über daraus abgeleitete Schlüsse, Bewertungen der Ergebnisse bis hin zur abschließenden Meinung und Empfehlungen. Es muss nachvollziehbar, objektiv und umfassend dokumentiert sein.

---

Was versteht man unter einem **Writeblocker** in der IT-Forensik? #card
Ein Writeblocker ist ein Hardware- oder Softwarewerkzeug, das verhindert, dass ein Originaldatenträger bei der Sicherung verändert wird. Dies garantiert die Integrität der digitalen Beweise.

---

Was ist eine **forensische Beweismittelkette (Chain of Custody)**? #card
Die Chain of Custody beschreibt die lückenlose und dokumentierte Nachvollziehbarkeit der Aufbewahrung, Übergabe und Bearbeitung digitaler Beweismittel, um Manipulation auszuschließen und die Verwendbarkeit vor Gericht sicherzustellen.

---

Was sind Beispiele für typische **IT-Incidents**? #card

- Ein Mitarbeiter installiert Malware (z.B. versehentlich durch eine infizierte Bewerbung).
- Vorsätzlicher Datendiebstahl durch Mitarbeiter (z.B. Daten auf USB kopieren).
- Angriff durch Ransomware (Datenverschlüsselung und Lösegeldforderung).
- Unautorisierter Zugriff auf interne Daten durch verlorene Geräte oder offenen Serverzugriff.
^1741265891407

---

Was ist ein **Digitaler Ersthelfer** in der Incident Response? #card 
Ein Digitaler Ersthelfer ist eine speziell geschulte Person, die unmittelbar nach Erkennen eines IT-Vorfalls erste Maßnahmen ergreift (z.B. Trennen vom Netzwerk, Dokumentation des Vorfalls, Benachrichtigung weiterer IT-Experten).

---

Welche **grundlegenden Incident-Klassen** gibt es häufig in der Praxis? #card

- Innentäter (Sabotage, Datendiebstahl)
- Unautorisierter Zugriff auf interne Daten
- Datenverlust und -rettung (technische Defekte, Ransomware)
- Installation nicht-autorisierter Software (z.B. Raubkopien mit Schadsoftware)
^1741265891414

---

Was versteht man unter **Incident Response**? #card 
Incident Response umfasst alle organisatorischen und technischen Maßnahmen zur Erkennung, Behandlung und Behebung von IT-Sicherheitsvorfällen, mit dem Ziel, Schäden zu minimieren und den normalen Betrieb wiederherzustellen.

---

Was sind die **10 goldenen Regeln des Digitalen Ersthelfers** (auszugsweise)? #card

- Ruhe bewahren
- Keine vorschnellen Aktionen durchführen
- Systeme nicht vorschnell abschalten oder verändern
- Dokumentation aller Schritte sicherstellen
- Kommunikation mit geeigneten Personen durchführen
- Vorfall an zuständige Personen melden
- Veränderung und Interaktionen genau dokumentieren
^1741265891421

---

Was ist das **Ziel einer forensischen Untersuchung im Incident-Response-Prozess**? #card 
Ziel ist es, genau zu ermitteln, was passiert ist, wie es passiert ist, und idealerweise wer oder was verantwortlich war. Diese Untersuchung liefert oft eine Basis für weitere juristische oder organisatorische Maßnahmen.

---

Was bedeutet **Incident Response**? #card 
Incident Response bezeichnet das systematische Vorgehen zur Erkennung, Behandlung und Nachbereitung von IT-Sicherheitsvorfällen, einschließlich technischer, organisatorischer und rechtlicher Aspekte.

---

Welche Ebenen umfasst das **Prozessmodell der IT-Forensik** nach BSI-Leitfaden? #card

- Vorfallserkennung
- Sicherung digitaler Beweismittel
- Analyse der Beweismittel
- Präsentation der Ergebnisse (z.B. Sachverständigengutachten)
^1741265891427

---

Was bedeutet „Better safe than sorry“ im Kontext der IT-Forensik und Incident Response? #card  
Lieber einmal zu oft auf einen möglichen Sicherheitsvorfall reagieren (Fehlalarm), als einen echten Sicherheitsvorfall zu übersehen.
^1741265891433
