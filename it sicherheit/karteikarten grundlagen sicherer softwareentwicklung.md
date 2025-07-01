---
cards-deck: it sicherheit
---

Was bedeutet "Security Engineering"? #card  
	**Security Engineering** bedeutet das **konzeptionelle und technische Gestalten** eines Systems, damit es trotz böswilliger Angriffe, Fehler und unvorhergesehener Ereignisse **zuverlässig und sicher** bleibt. Dabei werden **Methoden, Prozesse und Werkzeuge** eingesetzt, um Sicherheitsziele schon in der **Design- und Implementierungsphase** systematisch zu erreichen.
^1741195747532

Welche vier Bereiche umfasst das Framework von Ross Anderson im Security Engineering? #card  
- **Policy**: Festlegung, **was** erreicht werden soll (z. B. Schutzziele).  
- **Mechanism**: **Techniken** und **Algorithmen**, die zum Schutz eingesetzt werden können (z. B. Verschlüsselung, Authentifizierungsverfahren).  
- **Assurance**: **Vertrauensgrad** in die jeweiligen Schutzmechanismen (z. B. formale Überprüfungen, Zertifizierungen).  
- **Incentives**: Motivationen und **Anreize** aller Beteiligten, das System sicher zu betreiben (z. B. Betreiber, Angreifer).
^1741195747577

Warum ist es sinnvoll, Sicherheitsanforderungen früh in der Softwareentwicklung zu berücksichtigen? #card  
- **Änderungen** sind zu einem späteren Zeitpunkt **viel aufwändiger** und teurer.  
- Die **Software-Architektur** kann so von Beginn an sicherheitsrelevante Aspekte integrieren.  
- **Konzeptfehler** in frühen Phasen wirken sich später gravierender auf die Gesamtsicherheit aus.  
- Reduziert das Risiko von **Sicherheitslücken** und **Nachbesserungskosten**.
^1741195747581

Was versteht man unter "Threat Modeling"? #card  
- **Prozess**, bei dem in der **Design-Phase** einer Software mögliche **Bedrohungen** identifiziert werden.  
- Man untersucht Datenflüsse und Ressourcen, um **Angriffsszenarien** (Threat Trees/Fault Trees) aufzuzeigen.  
- Ziel ist, die **Risiken** früh zu erkennen und passende **Gegenmaßnahmen** einzuplanen.
^1741195747585

Was bedeutet "fail-safe" und "fail-secure"? #card  
- **Fail-safe**: Das System geht bei einem Ausfall in einen **Zustand**, der für den Benutzer **ungefährlich** bzw. ungefährdet ist (z. B. Not-Aus, Service verweigert).  
- **Fail-secure**: Das System bleibt bei einem Ausfall **geschützt** und verhindert **unbefugten Zugriff**, auch wenn es dafür evtl. die Funktion einschränkt.
^1741195747588

Was ist "Change Management" im Kontext sicherer Softwareentwicklung? #card  
- Geregelter Prozess, um **Änderungen** (z. B. an Code oder Konfiguration) **nachvollziehbar** zu planen, durchzuführen und zu dokumentieren.  
- Ziel ist, **ungeplante Nebeneffekte** zu minimieren und **Fehlerquellen** zu reduzieren.  
- Wichtig in sicherheitskritischen Umgebungen, da jede Änderung neue **Schwachstellen** einführen kann.
^1741195747592

Welche Arten von Anwendungskontrollen existieren für Software? #card  
- **Eingabekontrollen**: Prüfen, ob **Daten korrekt** und **vollständig** eingegeben werden (z. B. Validierung).  
- **Verarbeitungskontrollen**: Stellen sicher, dass Daten bei der **Verarbeitung** weiterhin korrekt sind (z. B. Plausibilitätsprüfungen).  
- **Ausgabekontrollen**: Überprüfen, dass ausgegebene Daten **korrekt** sind und ggf. an die **richtigen Empfänger** gehen.
^1741195747596

Was sind fehlertolerante Computersysteme? #card  
- Systeme, die **redundante** Hardware-, Software- oder Stromversorgungs-Komponenten nutzen. 
- Ziel: Auch bei **Fehlern** im System läuft die **Kernfunktion** weiter.  
- Erhöht die **Ausfallsicherheit** und kann in sicherheitskritischen Bereichen sehr wichtig sein.
^1741195747600

Was ist "Functional Safety" und wie hängt sie mit sicherer Softwareentwicklung zusammen? #card  
- **Functional Safety** (z. B. nach IEC 61508) bezieht sich darauf, dass sicherheitsrelevante Systeme bei **Ausfällen** oder **Fehlfunktionen** **keine Gefahr** für Menschen oder Sachwerte darstellen.  
- In der Softwareentwicklung bedeutet das, **Risiken** frühzeitig zu analysieren und geeignete **Techniken** zur Vermeidung bzw. Kontrolle von Fehlern einzusetzen.  
- Kommt oft in **Industrie**, **Medizin** und **Automobil** zum Einsatz.
^1741195747605

Warum ist Dokumentation wichtig für sichere Softwareentwicklung? #card  
- **Nachvollziehbarkeit**: Jede Sicherheitsentscheidung sollte dokumentiert sein, damit man bei **Änderungen** versteht, **warum** etwas so umgesetzt wurde.  
- **Qualitätssicherung**: Mit guter Dokumentation lassen sich **Fehlerquellen** schneller erkennen und ausräumen.  
- **Revisionssicherheit**: Hilft bei **Audits** oder in **Haftungsfällen**, zeigen zu können, dass die Sicherheitsvorgaben eingehalten wurden.
^1741195747610

Was versteht man unter „Secure Software Development Lifecycle“ (SSDLC)? #card  
Der **Secure Software Development Lifecycle** integriert **Sicherheitsmaßnahmen** in jeden Abschnitt des **Softwareentwicklungszyklus** – von der **Anforderungsanalyse** über **Design und Implementierung** bis hin zu **Tests, Wartung** und **Rückbau**. Ziel ist, **Sicherheit** von Anfang an und kontinuierlich zu berücksichtigen, statt sie erst am Ende „anzuflanschen“.

Welche Rolle spielt das „Least Privilege“-Prinzip in der Softwareentwicklung? #card  
- Beim **Least Privilege**-Prinzip erhält jede **Komponente** oder jeder **Prozess** nur die **minimal notwendigen Rechte**, um seine Aufgabe zu erfüllen.  
- Verringert das Risiko, dass kompromittierte Teile einer Anwendung weitreichenden Schaden anrichten können.  
- Sollte sowohl auf **Benutzerberechtigungen** als auch auf **interne Software-Komponenten** angewendet werden.

Was ist ein „Design Review“ im Kontext sicherer Softwareentwicklung? #card  
- Eine **Überprüfung** der **Softwarearchitektur** und des **Systemdesigns** im Hinblick auf **mögliche Schwachstellen**.  
- Oft werden **Bedrohungsmodelle** herangezogen, um zu sehen, ob alle Angriffsvektoren adressiert sind.  
- Dient dazu, **teure Korrekturen** spät im Prozess zu vermeiden.

Warum ist „Secure Coding“ wichtig? #card  
- **Fehler im Quellcode** können häufige Angriffsflächen sein (z. B. Pufferüberläufe, SQLi, XSS).  
- Secure Coding fasst **Best Practices** zusammen, damit Code robust und **resistent** gegenüber Standardangriffen ist.  
- Reduziert den **Wartungsaufwand** und erhöht die **Zuverlässigkeit** der Anwendung.

Wie kann ein automatisches „Static Code Analysis Tool“ helfen? #card  
- **Durchsucht** den Quellcode **ohne** ihn auszuführen.  
- Identifiziert **potenzielle Sicherheitslücken** (z. B. unsichere Funktionen, fehlende Input-Validierung).  
- Liefert **Empfehlungen**, die man dann manuell überprüfen und beheben kann.  
- Spart Zeit und erhöht die **Qualität** des Codes.

Was ist der Unterschied zwischen „Static Code Analysis“ und „Dynamic Code Analysis“? #card  
- **Static Code Analysis**: Prüft den **Quellcode**, ohne das Programm **auszuführen** (z. B. auf unsichere Funktionen).  
- **Dynamic Code Analysis**: Untersucht das **laufende Programm** (z. B. Penetrationstest, Fuzzing).  
- Beide Ansätze **ergänzen sich**, weil sie unterschiedliche Perspektiven liefern.

Wofür wird „Fuzzing“ eingesetzt? #card  
- **Automatisches Testverfahren**, bei dem **zufällige** oder **manipulierte Eingaben** an eine Software gesendet werden.  
- Ziel: **Abstürze**, **ungewöhnliches Verhalten** oder **Sicherheitslücken** aufzudecken.  
- Hilft, **schwer reproduzierbare Fehler** zu finden, die bei konventionellen Tests unentdeckt bleiben.

Was ist „Continuous Integration/Continuous Deployment“ (CI/CD) und wie hilft es der Sicherheit? #card  
- **CI/CD** ist ein Ansatz, bei dem Code **kontinuierlich** integriert, getestet und **automatisiert ausgeliefert** wird.  
- In jeder Pipeline-Stufe lassen sich **Sicherheitstests** (z. B. Static Analysis, Unit Tests) integrieren.  
- Dadurch können **Sicherheitsprobleme früh** erkannt werden und das Risiko von **unsicheren Releases** sinkt.

Was ist der Zweck von „Security Testing“ (z. B. Penetration Testing)? #card  
- **Sicherheitsrelevante Schwachstellen** aufdecken, bevor sie ein Angreifer findet.  
- Umfasst **manuelles** oder **automatisiertes Testen** von Angriffsszenarien (SQLi, XSS, etc.).  
- Liefert dem Team **konkrete Empfehlungen**, um die Software **robuster** zu machen.

Wie trägt eine gute „Logging und Monitoring“-Strategie zur sicheren Softwareentwicklung bei? #card  
- **Protokolliert** sicherheitsrelevante Ereignisse (z. B. Login-Versuche, Fehlermeldungen, Zugriffe).  
- Unerwartetes Verhalten (z. B. Häufung von Fehlanmeldungen) kann **schneller erkannt** werden.  
- Erleichtert **Forensik** und **Incident Response**, indem nachvollziehbar wird, **wer**, **wann**, **was** gemacht hat.
