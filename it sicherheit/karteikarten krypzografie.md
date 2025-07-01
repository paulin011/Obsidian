---
cards-deck: it sicherheit
---



Was ist Kryptographie? #card  
**Kryptographie** befasst sich mit dem **vertraulichen und integren Austausch** von Informationen. Sie nutzt **mathematische Verfahren**, um Daten so zu verschlüsseln, dass **Unbefugte** sie **nicht lesen** oder **manipulieren** können.  
^1741261124566

Welche Schutzziele verfolgt die Kryptographie? #card  
- **Vertraulichkeit** (nur Befugte können den Klartext lesen)  
- **Integrität** (Daten sind unverändert)  
- **Authentizität** (Absender/Empfänger sind echt)  
- **Nicht-Abstreitbarkeit** (Versender kann Nachricht nicht leugnen)
^1741261124612

Was ist Steganographie? #card  
Die **Steganographie** („versteckte Schrift“) zielt darauf ab, **geheime Botschaften** so zu **verbergen**, dass **niemand** erkennt, dass überhaupt eine **Nachricht** ausgetauscht wird. Häufig wird ein harmlos wirkendes **Trägermedium** (z. B. Bild, Text) um unauffällig Zusatzinformationen einzubetten.
^1741261124618

Worin unterscheiden sich Steganographie und Kryptographie grundsätzlich? #card  
- **Kryptographie**: Verbirgt den **Inhalt** (Chiffretext ist erkennbar, aber unverständlich).  
- **Steganographie**: Verbirgt das **Vorhandensein** einer Nachricht (soll nicht auffallen, dass überhaupt etwas versteckt ist).
^1741261124625

Was ist ein typisches Beispiel für Steganographie? #card  
- **Einbetten** von Daten in **Bilddateien** (Least Significant Bit-Verfahren).  
- **Cardan-Gitter**: Bestimmte **Schablone**, durch die nur bestimmte Zeichen sichtbar werden.  
- Verbergen einer Nachricht in scheinbar harmlosen **Texten** oder **Audiodateien**.
^1741261124632

Was versteht man unter Steganalyse? #card  
**Steganalyse** ist das **Gegenstück** zur Steganographie. Sie versucht, durch **Untersuchung** von Daten oder Dateien **versteckte Informationen** aufzudecken – etwa mithilfe **statistischer Tests**, die Auffälligkeiten im Trägermedium erkennen.
^1741261124638

Wie lassen sich Steganographie und Kryptographie kombinieren? #card  
- Zuerst wird der **Klartext** kryptographisch **verschlüsselt**, dann das **Chiffrat** in einem **Trägermedium** versteckt.  
- Erhöht die **Sicherheit**, weil **Angreifer** weder **merkt**, dass eine Nachricht existiert, noch weiß, **wie** er den Inhalt entschlüsseln kann.
^1741261124647

Was bedeutet Kerckhoffs’ Prinzip in der Kryptographie? #card  
- Die **Sicherheit** eines kryptographischen Verfahrens darf **nicht** von der **Geheimhaltung** des **Algorithmus** abhängen, sondern **nur** von der **Geheimhaltung** des **Schlüssels**.  
- Gegensatz: „Security by Obscurity“ (wird als unsicher angesehen).
^1741261124653

Was bezeichnet man als „Kryptoanalyse“? #card  
- Den **Versuch**, kryptographische Verfahren oder **Chiffrate** zu **brechen**, ohne den Schlüssel zu kennen.  
- Prüft die **Stärke** von Verfahren und offenbart **Schwachstellen**, etwa durch **Brute Force**, **statistische** oder **mathematische** Angriffe.
^1741261124662

Welche Anwendungsbeispiele gibt es heute für Kryptographie? #card  
- **TLS/HTTPS**: Sichere Datenübertragung im Web  
- **VPNs**: Geschützter Fernzugriff auf Netze  
- **E-Mail-Verschlüsselung** (PGP, S/MIME)  
- **Digitale Signaturen** zur Echtheitsprüfung und Integritätssicherung  
^1741261124668



Welche grundsätzlichen Verschlüsselungsmethoden gibt es? #card  
- **Symmetrische Verfahren**: Ein einzelner **geheimer Schlüssel** für Ver- und Entschlüsselung. Beispiele: AES, DES.  
- **Asymmetrische Verfahren** (Public-Key-Kryptographie): **Zwei Schlüssel**, ein **öffentlicher** zum Verschlüsseln, ein **privater** zum Entschlüsseln. Beispiele: RSA, ECC.
^1741261124677

Was versteht man unter Block- und Stromchiffren? #card  
- **Blockchiffren**: Verarbeiten Daten in **festen Blöcken** (z. B. 128 Bit). Häufige Betriebsmodi: ECB, CBC, CTR.  
- **Stromchiffren**: Verarbeiten den Klartext **Zeichen** bzw. **Bit für Bit**. Beispiel: RC4, Trivium.
^1741261124683

Wodurch unterscheiden sich symmetrische und asymmetrische Verfahren? #card  
- **Symmetrisch**: **Ein gemeinsamer** geheimer Schlüssel, sehr schnell, aber Schlüsselverteilung schwierig.  
- **Asymmetrisch**: **Öffentlicher Schlüssel** (Public Key) + **Privater Schlüssel** (Private Key). Einfachere Verteilung, aber meist **langsamer**.
^1741261124689

Was sind typische Beispiele symmetrischer Algorithmen? #card  
- **DES** (veraltet, 56-Bit Schlüssel zu klein)  
- **3DES** (DES dreifach angewendet, noch solide, aber langsam)  
- **AES** (aktueller Standard, verschiedene Schlüssellängen: 128, 192, 256 Bit)
^1741261124697

Was sind typische Beispiele asymmetrischer Algorithmen? #card  
- **RSA** (basierend auf Faktorierung großer Zahlen)  
- **ECC** (Elliptic Curve Cryptography, kürzere Schlüssel, gleiche Sicherheit)  
- **ElGamal** (diskreter Logarithmus in zyklischen Gruppen)
^1741261124704

Welche Grundprinzipien gelten in der Kryptographie? #card  
- **Kerckhoffs’ Prinzip**: Sicherheit beruht nur auf dem **Schlüssel**, nicht auf der Geheimhaltung des Algorithmus.  
- **Konfusion und Diffusion** (nach Shannon): Konfusion verschleiert den Zusammenhang zwischen Schlüssel und Chiffrat, Diffusion verteilt die Redundanz des Klartexts über das Chiffrat.
^1741261124712

Welche Analysemethoden gibt es in der Kryptoanalyse? #card  
1. **Ciphertext-Only-Angriff**: Angreifer hat nur Chiffrate.  
2. **Known-Plaintext-Angriff** (KPA): Angreifer kennt einige Klartext-Chiffrat-Paare.  
3. **Chosen-Plaintext-Angriff** (CPA): Angreifer darf Klartexte wählen und erhält deren Chiffrate.  
4. **Chosen-Ciphertext-Angriff** (CCA): Angreifer darf Chiffrate einschicken und erhält die Klartexte.
^1741261124719

Was sind gängige Angriffstechniken auf verschlüsselte Daten? #card  
- **Brute Force / Exhaustive Search**: Alle möglichen Schlüssel durchprobieren.  
- **Wörterbuchangriff**: Variante des Brute-Force mit einer Liste wahrscheinlicher Passwörter.  
- **Seitenkanalangriff** (Side-Channel): Analyse von **Stromverbrauch, Timing** oder **elektromagnetischen Abstrahlungen**.  
- **Rubber-Hose Cryptanalysis**: Schlüsselgewinnung durch **physische** oder **psychische Zwangsmaßnahmen**.  
- **Kombinationsangriffe** (z. B. statistische Verfahren + Vorwissen).
^1741261124726

Worin besteht der Unterschied zwischen „Sicherheit durch Design“ und „Security by Obscurity“? #card  
- **Sicherheit durch Design**: Verfahren und Mechanismen sind **transparent** geprüft, gut dokumentiert, basieren auf **offenen Standards** (Kerckhoffs’ Prinzip).  
- **Security by Obscurity**: Setzt auf **Geheimhaltung** des Verfahrens/Mechanismus selbst, was als **unsicher** gilt, weil Angreifer es meist dennoch herausfinden.
^1741261124732

Warum wird AES heute oft als sicherer Standard verwendet? #card  
- **Starke Kryptoanalyse**: Bisher keine praktikablen Attacken bekannt, die AES brechen.  
- Flexibel in der **Schlüssellänge** (128/192/256 Bit).  
- **Weit verbreitet**, internationaler Standard, gut überprüft.
^1741261124740



