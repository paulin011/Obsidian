---
cards-deck: it sicherheit
---

Was versteht man unter dem Begriff „Web Security“? #card  
Die **Web Security** umfasst alle Maßnahmen und Konzepte, um **Webanwendungen** und deren **Daten** gegen Angriffe und Manipulationen abzusichern. Dabei stehen unter anderem **Vertraulichkeit**, **Integrität** und **Verfügbarkeit** im Fokus.
^1741195498580

Welche Rollen spielen Client und Server bei Webanwendungen? #card  
- **Client** (z. B. ein Browser) sendet **HTTP-Anfragen** (GET, POST etc.) an den Server.  
- **Server** (z. B. ein Webserver) verarbeitet die Anfrage und liefert **HTTP-Antworten** (z. B. HTML-Seiten, JSON-Daten) zurück.
^1741195498627

Was bedeutet Parametermanipulation? #card  
- Veränderung von **GET-/POST-Parametern**, Headern oder Cookies.  
- Angreifer versucht, **unerwartete Werte** an den Server zu senden (z. B. manipulierte Preisangaben in einem Webshop).  
- Ziel ist das Umgehen von **Validierungen** oder das Erzwingen eines abweichenden Verhaltens.
^1741195498631

Was ist Cross-Site Scripting (XSS)? #card  
- **XSS** ist das **Einschleusen von JavaScript** (oder anderem aktiven Code) in eine Webseite.  
- Angriff beruht darauf, dass **Scriptcode** später im Browser eines Opfers **ausgeführt** wird.  
- Gefährlich, weil Angreifer damit **Cookies auslesen**, Benutzeraktionen durchführen oder Inhalte manipulieren kann.
^1741195498635

Welche zwei Hauptvarianten von XSS gibt es? #card  
- **Reflektiertes (reflected) XSS**  
  - Schadcode wird direkt über **URL-Parameter** eingeschleust und sofort in der **Antwort** reflektiert.  
  - Wird aktiv, sobald das Opfer den **präparierten Link** aufruft.  
- **Persistentes (stored) XSS**  
  - Schadcode wird **dauerhaft auf dem Server** gespeichert (z. B. Kommentar, Gästebuch).  
  - Führt bei jedem Aufruf der Seite (z. B. von einem Nutzer oder Admin) zum Ausführen des schädlichen Codes.
^1741195498639

Nenne typische Gegenmaßnahmen gegen XSS. #card  
- **Input-Validierung** und **Ausgabe-Encoding** (z. B. HTML-Escape)  
- Verwenden von Bibliotheken oder Framework-Funktionen, die **Sonderzeichen** sicher handhaben  
- **Content Security Policy (CSP)** im HTTP-Header  
- Vermeiden, dass Benutzer **HTML/JavaScript** unkontrolliert einbringen können.
^1741195498643

Was bedeutet CSRF (Cross-Site Request Forgery)? #card  
- Eine Technik, bei der ein Angreifer das **authentifizierte Browser-Umfeld** eines Opfers missbraucht.  
- Der Browser sendet dabei **ungewollt** (für das Opfer unsichtbar) **gültige Anfragen** an eine Webanwendung, weil er noch **Sitzungscookies** hat.  
- Beispiele: Überweisung im Online-Banking auslösen, ohne dass der legitime Nutzer es bemerkt.
^1741195498648

Wie schützt man sich gegen CSRF-Angriffe? #card  
- **CSRF-Token** (zufällige, einmalige Token) in Formularen oder Links.  
- **SameSite-Cookies** aktivieren, damit Cookies nicht bei fremden Seiten geschickt werden.  
- **Token-Überprüfung** auf Serverseite: Anfrage wird nur akzeptiert, wenn Token gültig ist.
^1741195498652

Was sind Cookies und welche Rolle spielen sie in der Web Security? #card  
- **Cookies** sind kleine **Datenpakete**, die im Browser gespeichert werden.  
- Dienen typischerweise zur **Session-Verwaltung** (z. B. eingeloggter Nutzer).  
- Können ein **Angriffsvektor** sein (z. B. Session-Hijacking), wenn sie nicht sicher verwaltet oder geschützt werden (Secure-/HttpOnly-Flags, SameSite-Attribut).
^1741195498656

Was sind gängige Best Practices, um Webanwendungen abzusichern? #card  
- **Eingaben validieren** (Server- und Client-seitig)  
- **Ausgaben escapen** (HTML, JavaScript, CSS)  
- **HTTPS erzwingen** (TLS/SSL)  
- **Security-Header** verwenden (Content Security Policy, X-Frame-Options, X-XSS-Protection usw.)  
- **Sicheres Session-Management** (sichere Cookies, korrekte Invalidation)  
- **Regelmäßige Code-Reviews und Penetrationstests** durchführen.
^1741195498660

Welche Funktion hat HTTPS in Bezug auf Web Security? #card  
- **HTTPS** ist HTTP über **TLS/SSL** und bietet:  
  - **Verschlüsselung**: Abhörsicherheit  
  - **Integrität**: Schutz vor Manipulation unterwegs  
  - **Authentizität**: Server-Identität durch Zertifikate überprüfbar.
^1741195498664

Was versteht man unter SQL-Injection (SQLi)? #card  
- **Einschleusen von SQL-Befehlen** in Datenbankabfragen durch manipulierte Eingaben.  
- Ermöglicht dem Angreifer z. B. **Daten auszulesen**, zu löschen oder zu verändern.  
- Klassisches Beispiel: Anmeldemaske ohne sichere **Prepared Statements**.
^1741195498668

Welche Maßnahmen helfen gegen SQL-Injection? #card  
- **Prepared Statements** oder **parametrisierte Abfragen** (statt String-Konkatenation)  
- **Whitelisting** von Eingaben (Zahlen-/Zeichen-Filter)  
- **Least Privilege** für Datenbank-User (z. B. Schreibrechte nur wo nötig).
^1741195498673

Was ist ein „Black Box Testing“ im Kontext der Websicherheit? #card  
- Testmethode, bei der ein **externer Tester** ohne Einblick in den Quellcode eine Anwendung überprüft.  
- Greift wie ein **Angreifer von außen** auf die Anwendung zu.  
- Findet oft **praktische Sicherheitslücken**, kann aber tieferliegende Codefehler übersehen.
^1741195498677

Was sollte man bei der Entwicklung sicherer Webanwendungen beachten? #card  
- Sicherheitsaspekte müssen **frühzeitig** eingebunden werden (Security by Design).  
- **Regelmäßige Updates** der verwendeten Frameworks und Bibliotheken.  
- Implementieren von **Logging** und **Monitoring**, um Angriffe zu erkennen.  
- **Penetrationstests** und **Code Reviews** vor dem Release.
^1741195498681
