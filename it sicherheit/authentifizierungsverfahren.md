---
cards-deck: it sicherheit
---


**Authentifikation mittels Wissen** #card  
Die Authentifikation erfolgt durch den Nachweis eines Geheimnisses, das nur dem Benutzer bekannt ist. Beispiele: Passwörter, PINs, Sicherheitsfragen. Vorteile: Einfach in der Implementierung und kostengünstig. Nachteile: Anfällig für Phishing, Shoulder Surfing und Brute-Force-Angriffe.
^1741177751424

---

**Authentifikation mittels Besitz** #card
Hierbei wird ein physisches oder digitales Objekt zur Identitätsbestätigung verwendet. Beispiele: Smartcards, Security Tokens, Einmalpasswort-Generatoren. Vorteile: Schwierig zu fälschen. Nachteile: Verlust oder Diebstahl kann zu Sicherheitsproblemen führen.
^1741177751430

---

**Authentifikation mittels biometrischer Merkmale** #card 
Identitätsnachweis anhand individueller körperlicher oder verhaltensbasierter Merkmale. Beispiele: Fingerabdruckscanner, Gesichtserkennung, Iris-Scan. Vorteile: Hohe Sicherheit, schwer fälschbar. Nachteile: Datenschutzprobleme, mögliche Fehlerraten (False Acceptance, False Rejection).
^1741177751433

---

**Mehrfaktor-Authentifikation (MFA)** #card
Kombination mehrerer Authentifikationsverfahren zur Erhöhung der Sicherheit. Typische Kombinationen: Wissen + Besitz (z.B. Passwort + SMS-Code). Vorteile: Höhere Sicherheit als Einzelfaktoren. Nachteile: Erhöhter Verwaltungsaufwand und Usability-Herausforderungen.
^1741177751438

---

**Einmalpasswörter (OTP)** #card  
Passwörter, die nur einmalig für eine Anmeldung gültig sind, oft per SMS oder Authenticator-App generiert. Vorteile: Keine Wiederverwendung von Passwörtern möglich. Nachteile: Abhängigkeit von einer sicheren Übertragungsmethode.
^1741177751442

---

**Public-Key-Authentifikation** #card
Nutzung asymmetrischer Kryptographie zur Authentifikation, oft in SSH- oder PGP-Umgebungen. Vorteile: Hohe Sicherheit, da keine Passwörter übermittelt werden. Nachteile: Verwaltung von Schlüsselpaaren kann komplex sein. 
^1741177751445

**Vier-Augen-Prinzip** #card  
Das Vier-Augen-Prinzip ist ein Sicherheitsmechanismus, bei dem eine Aktion oder Entscheidung von mindestens zwei unabhängigen Personen überprüft werden muss. Dies dient der Fehlervermeidung und Betrugsprävention. Es wird häufig in sicherheitskritischen Bereichen wie der IT-Sicherheit, dem Finanzwesen und der Verwaltung sensibler Daten eingesetzt.
^1741177751449

**Challenge-Response-Verfahren** #card  
Das Challenge-Response-Verfahren ist ein Authentifizierungsmechanismus, bei dem eine Partei (z. B. ein Server) eine zufällige Herausforderung (Challenge) sendet, die von der anderen Partei (z. B. einem Client) mit einer vorher definierten Antwort (Response) beantwortet werden muss. Diese Antwort basiert auf einem geheimen Schlüssel oder kryptografischen Algorithmus. Ziel ist es, die Identität sicherzustellen, ohne das geheime Passwort direkt zu übertragen.
^1741177751453

**RADIUS (Remote Authentication Dial-In User Service)** #card  
RADIUS ist ein zentrales Authentifizierungs-, Autorisierungs- und Accounting-Protokoll (AAA) für Netzwerkzugriffe. Es wird häufig für VPNs, WLANs, Einwahlzugänge und Unternehmensnetzwerke genutzt.
- **Authentifizierung:** Ein Client (z. B. ein WLAN-Router oder VPN-Server) leitet Benutzeranmeldedaten (Benutzername, Passwort oder Zertifikat) an den RADIUS-Server weiter. Dieser prüft die Anmeldedaten gegen eine Datenbank (z. B. Active Directory, LDAP, SQL-Datenbank).
- **Autorisierung:** Nach erfolgreicher Authentifizierung legt der RADIUS-Server fest, welche Dienste und Ressourcen der Benutzer nutzen darf.
- **Accounting:** Der RADIUS-Server kann Sitzungsinformationen wie Verbindungsdauer, genutzte Bandbreite und IP-Adressen protokollieren.
**Ablauf einer RADIUS-Anfrage:**
1. Der Benutzer sendet Anmeldeinformationen an einen Netzwerk-Access-Server (NAS, z. B. WLAN-AP, VPN-Gateway).
2. Der NAS leitet die Anfrage als RADIUS-Request an den RADIUS-Server weiter.
3. Der RADIUS-Server überprüft die Zugangsdaten mit einer Benutzerdatenbank.
4. Falls erfolgreich, sendet der RADIUS-Server eine "Access-Accept"-Nachricht zurück, ggf. mit spezifischen Zugriffsrechten. Falls fehlerhaft, wird ein "Access-Reject" gesendet.
5. Während der Sitzung kann der RADIUS-Server weitere Abfragen oder Logging-Informationen für Abrechnung und Kontrolle speichern.
**Sicherheit:** RADIUS verwendet das UDP-Protokoll und MD5-basierte Verschlüsselung für Passwörter, ist aber anfällig für Man-in-the-Middle-Angriffe. Eine sicherere Alternative ist **RadSec**, eine TLS-verschlüsselte Version von RADIUS.
^1741177751457

---

**Kerberos** #card  
Kerberos ist ein sicheres, netzwerkbasiertes Authentifizierungsprotokoll, das auf symmetrischer Kryptographie und einem zentralen Ticket-System basiert. Es ermöglicht Single Sign-On (SSO) und wird häufig in Unternehmensnetzwerken mit Windows Active Directory genutzt.
**Hauptkomponenten:**
- **Key Distribution Center (KDC):** Zentraler Server mit zwei Diensten:
    - **Authentication Server (AS):** Prüft Benutzeridentitäten und stellt ein Ticket Granting Ticket (TGT) aus.
    - **Ticket Granting Server (TGS):** Erteilt Dienst-Tickets (Service Tickets) für verschiedene Netzwerkdienste.
- **Client:** Ein Benutzer oder eine Maschine, die sich im Netzwerk authentifizieren möchte.
- **Service (Server):** Ein Server oder Dienst, auf den der Client zugreifen möchte (z. B. Dateifreigaben, E-Mail, Drucker).
**Ablauf einer Kerberos-Authentifizierung:**
1. **Anfrage beim AS:** Der Benutzer meldet sich mit seinem Benutzernamen an. Das Passwort wird nicht direkt übertragen, sondern als Hash verwendet.
2. **TGT-Erhalt:** Der AS überprüft den Benutzer und gibt ein verschlüsseltes Ticket Granting Ticket (TGT) zurück, das nur für eine begrenzte Zeit gültig ist.
3. **Anfrage beim TGS:** Der Client sendet das TGT an den TGS, um ein Service Ticket für einen bestimmten Dienst zu erhalten.
4. **Service Ticket-Erhalt:** Der TGS sendet das Dienst-Ticket zurück.
5. **Zugriff auf den Dienst:** Der Client sendet das Service Ticket an den Server des gewünschten Dienstes. Falls gültig, wird der Zugriff gewährt.
**Sicherheitsmerkmale:**
- **Symmetrische Verschlüsselung (AES, RC4):** Passwort wird nie direkt über das Netzwerk gesendet.
- **Zeitstempelbasierte Authentifizierung:** Verhindert Replay-Angriffe.
- **Single Sign-On (SSO):** Ein Benutzer meldet sich einmal an und kann auf mehrere Dienste zugreifen, ohne erneut Login-Daten einzugeben.
- **Erhöhte Sicherheit durch Mutual Authentication:** Client und Server authentifizieren sich gegenseitig.
**Schwachstellen & Herausforderungen:**
- **KDC als Single Point of Failure:** Bei einem Ausfall können sich Benutzer nicht mehr authentifizieren.
- **Uhrzeitsynchronisation erforderlich:** Kerberos verwendet Zeitstempel, weshalb Server und Clients synchronisierte Uhren benötigen (max. Zeitabweichung typischerweise 5 Minuten).
- **Pass-the-Ticket-Angriffe:** Angreifer können gestohlene Tickets für illegitime Authentifizierung nutzen.
^1741177751460


**Klartextspeicherung von Passwörtern** #card  
Die Speicherung von Passwörtern im Klartext ist ein schwerwiegendes Sicherheitsrisiko, da kompromittierte Datenbanken sofort die Anmeldeinformationen aller Benutzer offenlegen. Falls ein Angreifer Zugriff auf die Datenbank erhält, kann er die Passwörter direkt missbrauchen oder für weitere Angriffe (Credential Stuffing) verwenden.  
**Warum ist Klartextspeicherung unsicher?**
- **Kein Schutz vor Datenlecks:** Ein Hackerangriff kann alle Passwörter sofort offenlegen.
- **Interne Bedrohungen:** Administratoren oder Insider könnten Passwörter missbrauchen.
- **Wiederverwendung von Passwörtern:** Nutzer verwenden oft dieselben Passwörter für mehrere Dienste.
Um Klartextspeicherung zu vermeiden, sollten Passwörter **gehasht** und mit **Salt** geschützt werden.

---

**Salting von Passwörtern** #card  
Salting ist eine Technik zur Erhöhung der Sicherheit von gehashten Passwörtern, indem ein zufälliger Wert (Salt) zum Passwort hinzugefügt wird, bevor es gehasht wird. Dies verhindert, dass Angreifer vorgefertigte Hash-Werte aus **Rainbow Tables** nutzen.  
**Funktionsweise:**
1. Ein zufälliger **Salt** (z. B. 16 Byte) wird für jedes Passwort generiert.
2. Das Salt wird mit dem Passwort kombiniert (z. B. `Salt + Passwort`).
3. Das kombinierte Ergebnis wird mit einer sicheren Hash-Funktion (z. B. SHA-256, bcrypt) gehasht.
4. Der Hash und der Salt werden gemeinsam gespeichert.
**Vorteile:**
- **Schutz gegen Rainbow Tables:** Vorgefertigte Hash-Tabellen sind nutzlos, da jedes Passwort durch den individuellen Salt einzigartig wird.
- **Erhöhte Entropie:** Selbst identische Passwörter erhalten durch den Salt unterschiedliche Hashes.
- **Erhöhung des Rechenaufwands für Angreifer:** Wörterbuch- und Brute-Force-Angriffe werden erschwert.
**Best Practices:**
- **Jeder Benutzer sollte einen eigenen Salt haben.**
- **Salts sollten lang genug sein (mindestens 16 Byte).**
- **Zusätzliche Iterationen (Key Stretching) sollten genutzt werden, z. B. durch PBKDF2 oder Argon2.**

---

**PBKDF2 (Password-Based Key Derivation Function 2)** #card  
PBKDF2 ist eine Schlüsselableitungsfunktion, die verwendet wird, um Passwörter durch wiederholtes Hashing widerstandsfähiger gegen Brute-Force- und Wörterbuchangriffe zu machen. Es gehört zur Kategorie des **Key Stretching** und ist in vielen kryptografischen Anwendungen und Protokollen (z. B. WPA2, PKCS#5) verbreitet.  
**Funktionsweise:**
1. Das Passwort wird mit einem zufälligen **Salt** kombiniert.
2. Der Hashing-Algorithmus (z. B. HMAC-SHA256) wird mehrfach iterativ angewendet (z. B. 100.000 Iterationen).
3. Das finale Ergebnis dient als sicherer Hash oder als Schlüssel für kryptografische Anwendungen.
**Vorteile:**
- **Verlangsamt Brute-Force-Angriffe**, indem das Hashing viele Iterationen durchläuft.
- **Kann mit verschiedenen Hash-Funktionen kombiniert werden**, um die Sicherheit anzupassen.
- **Standardisiert (RFC 8018)** und in vielen Systemen integriert.
**Parameter von PBKDF2:**
- **Passwort:** Das zu schützende Passwort.
- **Salt:** Ein zufälliger Wert zur Vermeidung von Rainbow-Table-Angriffen.
- **Iterationsanzahl:** Anzahl der Wiederholungen (empfohlen mindestens 100.000).
- **Hash-Funktion:** HMAC mit SHA-256 oder SHA-512.
- **Schlüssellänge:** Länge des erzeugten Hashes (z. B. 256 Bit).
**Alternativen zu PBKDF2:**
- **bcrypt:** Speichert den Salt im Hash, begrenzt parallele Berechnungen durch seinen adaptiven Kostenfaktor.
- **Argon2:** Gewinner des "Password Hashing Competition", bietet Schutz gegen GPU-optimierte Angriffe und hohe Anpassbarkeit.
PBKDF2 ist besonders nützlich in **Legacy-Systemen**, während **bcrypt und Argon2** als moderner und sicherer gelten.

---

