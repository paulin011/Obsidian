
Welche zwei Hauptvarianten von XSS gibt es? #card
- **Reflektiertes XSS**: Der Schadcode wird direkt über URL-Parameter an den Server übergeben und sofort beim Opfer ausgeführt.
- **Persistentes XSS**: Der Schadcode wird dauerhaft gespeichert (z.B. in Datenbanken) und zu einem späteren Zeitpunkt von Opfern abgerufen.


Wofür steht die Abkürzung **XSS** und was macht diese Angriffe gefährlich? #card  
XSS steht für **Cross-Site Scripting**. Diese Angriffe ermöglichen das Ausführen fremden Codes im Browser, wodurch z.B. Cookies gestohlen, Sessions übernommen oder sensible Informationen abgegriffen werden können.

Was besagt die **Locard‘sche Regel** in der IT-Forensik? #card  
Die Locard'sche Regel besagt, dass bei Kontakt zweier Objekte (z.B. Täter und IT-System) immer wechselseitige Spuren entstehen, z.B. Log-Einträge oder Dateireste nach einer Löschung.


Was versteht man unter einem **fehlertoleranten Computersystem**? #card  
Ein fehlertolerantes Computersystem verwendet redundante Hardware-, Software- oder Stromversorgungskomponenten, um die Systemverfügbarkeit auch bei Fehlern oder Ausfällen sicherzustellen.

Was ist die **Entropie** im Kontext der IT-Sicherheit? #card  
Entropie beschreibt das Maß für Zufälligkeit oder Komplexität, z.B. eines Passwortes. Sie wird verwendet, um die Stärke (Informationsgehalt) eines Passwortes zu bewerten.

Was ist **Security Engineering** nach Ross Anderson? #card  
Security Engineering umfasst den Aufbau von Systemen, die robust gegenüber böswilligen oder unabsichtlichen Fehlern sind. Anderson definiert vier Schlüsselbereiche:

- **Policy** (Schutzziele)
- **Mechanismen** (Techniken zur Sicherung)
- **Assurance** (Grad des Vertrauens in Sicherheitsmechanismen)
- **Incentives** (Motivation von Angreifern und Verteidigern)

---

Nenne drei Kategorien von **Zugriffskontroll-Strategien**. #card

- **Discretionary Access Control (DAC)** (benutzerbestimmt)
- **Mandatory Access Control (MAC)** (systembestimmt)
- **Role-Based Access Control (RBAC)** (rollenbasiert)


Was bedeutet „Security by Obscurity“ und warum ist es problematisch? #card  
„Security by Obscurity“ bedeutet, Sicherheit durch Geheimhaltung interner Strukturen zu erreichen. Problematisch, weil Sicherheit nicht garantiert wird, wenn Details doch bekannt werden („Kerckhoffs’ Prinzip“).


Welche zwei Hauptaufgaben erfüllt **Incident Response**? #card  
Incident Response umfasst:

- **Erkennung** von IT-Sicherheitsvorfällen
- **angemessene Reaktion**, einschließlich Analyse, Eindämmung und Behebung des Vorfalls sowie Wiederherstellung des Normalbetriebs.


Was versteht man unter einer **Einwegfunktion**? Nenne ein Beispiel. #card  
Eine **Einwegfunktion** lässt sich leicht in eine Richtung berechnen, ist aber schwer umkehrbar (z.B. Hash-Funktion SHA-256). Sie wird oft für Passwörter eingesetzt.


Warum ist die **Länge eines Passworts wichtiger als die Komplexität**? #card  
Ein längeres Passwort erhöht die Entropie deutlich mehr als eine Erweiterung des Zeichenvorrats, da die Anzahl möglicher Kombinationen exponentiell mit der Länge wächst.