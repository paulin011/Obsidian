---
cards-deck: it sicherheit
---

Smart Cards: Beispiele für Implementierungen in Deutschland #card
▪ SIM-Karte ▪ Hotel-Zutrittskarten ▪ GeldKarte ▪ EC-/Debit-Karte ▪ Elektronische Gesundheitskarte ▪ Elektronischer Reisepass (ePass) ▪ Elektronischer Personalausweis (nPA) − Qualifizierte Signatur ▪ … ▪ Komunikation − Drahtlos (RFID/NFC) − Über Chip-Kontakte
^1741192369296


---

**U2F (Universal 2nd Factor)** #card
U2F ist ein offener, standardisierter Zwei-Faktor-Authentifizierungsmechanismus, der von der FIDO-Allianz entwickelt wurde. Er ermöglicht eine sichere Anmeldung durch einen **physischen Sicherheitsschlüssel** (z. B. USB-, NFC- oder Bluetooth-Token) und schützt vor Phishing- sowie Man-in-the-Middle-Angriffen.
**Funktionsweise:**
1. Der Benutzer meldet sich mit Benutzername und Passwort an.
2. Der Server sendet eine Challenge an den U2F-Sicherheitsschlüssel.
3. Der Sicherheitsschlüssel signiert die Challenge mit seinem privaten Schlüssel und sendet sie zurück.
4. Der Server verifiziert die Signatur mit dem öffentlichen Schlüssel des U2F-Tokens.
**Vorteile:**
- **Phishing-Schutz:** U2F ist domänengebunden – ein Angriff auf eine gefälschte Seite schlägt fehl.
- **Kein Geheimnis auf dem Server:** Der private Schlüssel bleibt auf dem Hardware-Token gespeichert.
- **Schnelle Authentifizierung:** Kein manuelles Eingeben von Codes erforderlich.
- **Unterstützung durch Browser & Dienste:** Chrome, Firefox, Edge und Dienste wie Google, GitHub und Dropbox unterstützen U2F.
**Nachfolger:**  
U2F wurde durch **FIDO2/WebAuthn** weiterentwickelt, das zusätzlich passwortlose Authentifizierung ermöglicht.
^1741192369345

---

**Discretionary Access Control (DAC)** #card
DAC ist eine **benutzerbestimmte Zugriffskontrolle**, bei der der **Eigentümer** eines Objekts entscheidet, wer darauf zugreifen darf und welche Berechtigungen vergeben werden.
**Merkmale:**
- **Objekteigentümer verwaltet Zugriffsrechte** (z. B. Dateien, Ordner).
- **Zugriffskontrolllisten (ACLs)** legen Berechtigungen für Benutzer fest.
- **Flexibel, aber anfällig für Fehler** (z. B. ungewollte Weitergabe von Rechten).
**Beispiel:**
- Ein Benutzer unter Windows oder Linux kann entscheiden, wer seine Dateien lesen oder ändern darf.
**Nachteil:**
- Schwierig in großen Systemen zu verwalten, da Benutzer Berechtigungen weitergeben können.
^1741192369353

---

**Mandatory Access Control (MAC)** #card
MAC ist eine **systembestimmte Zugriffskontrolle**, bei der der **Zugriff durch zentrale Sicherheitsrichtlinien geregelt** wird. Benutzer können ihre Rechte nicht selbst ändern.
**Merkmale:**
- **Sicherheitsstufen (z. B. Geheim, Vertraulich, Öffentlich)** steuern den Zugriff.
- **Keine Weitergabe von Berechtigungen** durch Benutzer möglich.
- **Strenge Kontrolle, geeignet für Hochsicherheitsbereiche (Militär, Regierung).**
**Beispiel:**
- Ein Dokument mit der Klassifikation „Geheim“ kann nur von Benutzern mit entsprechender Sicherheitsfreigabe gelesen werden.
**Nachteil:**
- Unflexibel, erfordert eine zentrale Verwaltung und kann den Arbeitsfluss einschränken.
---
**Role-Based Access Control (RBAC)** #card
RBAC ist eine **rollenbasierte Zugriffskontrolle**, bei der Berechtigungen nicht individuell, sondern über **Rollen** zugewiesen werden.
**Merkmale:**
- **Zugriffsrechte basieren auf vordefinierten Rollen** (z. B. „Administrator“, „Mitarbeiter“).
- **Erhöht die Sicherheit und Skalierbarkeit** in großen Organisationen.
- **Erleichtert die Verwaltung**, da Änderungen an Rollen statt an einzelnen Benutzern vorgenommen werden.
**Beispiel:**
- Ein „Mitarbeiter“ hat automatisch Zugriff auf interne Dokumente, aber kein Schreibrecht auf Unternehmensrichtlinien.
**Nachteil:**
- **Komplexe Einrichtung**, da Rollen und Berechtigungen genau definiert werden müssen.
^1741192369361

---

**Attribute-Based Access Control (ABAC)** #card
ABAC ist eine **attributbasierte Zugriffskontrolle**, bei der der Zugriff auf Basis mehrerer Attribute entschieden wird.
**Merkmale:**
- **Dynamische Regeln basierend auf Benutzer-, Objekt- und Umgebungseigenschaften.**
- **Flexibler als RBAC**, da Regeln nicht nur von Rollen abhängen.
- **Kann Kontextinformationen berücksichtigen** (z. B. Uhrzeit, Standort, Gerätetyp).
**Beispiel:**
- Ein Mitarbeiter kann **nur von einem Firmen-Laptop** aus auf vertrauliche Daten zugreifen, nicht von einem privaten Gerät.
**Nachteil:**
- **Höhere Komplexität**, da viele Attribute definiert und verwaltet werden müssen.
^1741192369369

---

**Rule-Based Access Control (RuBAC)** #card
RuBAC ist eine **regelbasierte Zugriffskontrolle**, die auf **vordefinierten Regeln** basiert, unabhängig von Benutzerrollen.
**Merkmale:**
- **Zugriff wird durch allgemeine Regeln gewährt oder verweigert.**
- **Oft als Ergänzung zu anderen Modellen (RBAC, MAC) genutzt.**
- **Kann Zeit-, Standort- oder Aktivitätsbedingungen enthalten.**
**Beispiel:**
- Ein System erlaubt den Zugriff nur **während der Geschäftszeiten (8:00 - 18:00 Uhr).**
**Nachteil:**
- **Weniger flexibel für individuelle Benutzeranforderungen.**
^1741192369378
