---
cards-deck: it sicherheit
---



Was ist eine elektronische Signatur? #card  
Eine elektronische Signatur ist ein digitaler Code, der einer elektronisch übertragenen Nachricht hinzugefügt wird, um ihren Inhalt und den Sender eindeutig zu identifizieren​oaicite:0.
^1741264138840

Welche Anforderungen müssen digitale Signaturen erfüllen? #card

- **Identifikation**: Die Signatur muss die Identität des Unterzeichners eindeutig erkennen lassen.
- **Echtheit**: Der Unterzeichner muss das Dokument gesehen und anerkannt haben.
- **Abschluss**: Der Unterzeichner muss inhaltlich zustimmen.
- **Warnung**: Die Unterzeichnung ist eine bewusste Handlung und macht dem Unterzeichner so dessen Bedeutung klar
^1741264138850

Wie funktionieren digitale Signaturen technisch? #card

1. Es wird ein Hash des zu signierenden Dokuments erstellt.
2. Der Hash wird mit dem privaten Schlüssel des Unterzeichners signiert.
3. Die Signatur kann mit dem öffentlichen Schlüssel verifiziert werden​oaicite:2.
^1741264138858

Welche Algorithmen werden für digitale Signaturen verwendet? #card

- **RSA**
- **Digital Signature Algorithm (DSA)**
- **Elliptic Curve Digital Signature Algorithm (ECDSA)**​oaicite:3.
^1741264138864

Wie wird eine digitale Signatur zur Authentifizierung verwendet? #card

4. Der Server sendet eine Zufallszahl an den Client.
5. Der Client signiert diese Zufallszahl mit seinem privaten Schlüssel.
6. Der Server überprüft die Signatur mit dem öffentlichen Schlüssel des Clients​oaicite:4.
^1741264138871

Was ist eine Public-Key-Infrastruktur (PKI)? #card  
Eine PKI ermöglicht die Verwaltung von digitalen Zertifikaten und Schlüsselpaaren durch eine vertrauenswürdige Zertifizierungsstelle (CA). Diese CAs stellen Zertifikate aus, die die Authentizität öffentlicher Schlüssel bestätigen​oaicite:5.
^1741264138878

Was ist eine Zertifikatssperrliste (CRL)? #card  
Eine Zertifikatssperrliste enthält Zertifikate, die als ungültig erklärt wurden, z. B. weil der zugehörige private Schlüssel kompromittiert wurde​oaicite:6
^1741264138885
