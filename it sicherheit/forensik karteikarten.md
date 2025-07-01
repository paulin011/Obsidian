---
cards-deck: it sicherheit
---

Was versteht man unter **forensischen Datenspuren** in der IT-Forensik? #card  
Forensische Datenspuren sind digitale Spuren, die bei der Nutzung eines Systems entstehen und Hinweise auf Aktivitäten und Ereignisse geben können.
^1741623227853

Wo entstehen **forensische Datenspuren** typischerweise? #card  
- Dateisystem  
- Betriebssystem (z.B. Logdateien)  
- Arbeitsspeicher (RAM)  
- Netzwerkverkehr (Logfiles, Protokolle)  
- Temporäre Dateien und Cache  
- Metadaten von Dateien  
- Bildschirmfotos und Videomitschnitte
^1741623227861

Wann entstehen explizit **keine Datenspuren**? #card  
- Bei Nutzung von vollständig verschlüsselten, temporären oder flüchtigen Speichern  
- Bei bestimmten anonymisierenden Techniken (z. B. RAM-only Betriebssysteme)
^1741623227865

Was passiert mit forensischen Datenspuren, wenn eine virtuelle Maschine (z. B. Kali-VM) gelöscht wird? #card  
- Teile der Spuren (z. B. temporäre Dateien, Snapshots) können unwiederbringlich verloren gehen  
- Andere Spuren könnten auf dem Host-System noch auffindbar bleiben (z. B. Dateifragmente, Logs des Hosts)
^1741623227868

In welche Kategorien kann Forensik-Software eingeteilt werden? #card  
- **Post-mortem Forensik** (Analyse eines nicht laufenden Systems)  
- **Live-Forensik** (Analyse eines laufenden Systems)
^1741623227872

Welche speziellen Daten untersucht **Post-mortem Forensiksoftware**? #card  
- Dateisystem und Betriebssystemdaten  
- Nutzerdateien (z. B. Dokumente, Videos, Bilder)  
- Metadaten von Dateien und Dateiinhalten
^1741623227876

Welche Datenquellen nutzt die **Live-Forensiksoftware**? #card  
- Arbeitsspeicher (RAM)  
- Aktuelle Bildschirmfotos oder Videomitschnitte  
- Laufender Netzwerkdatenverkehr  
- Elektromagnetische Abstrahlung (fortgeschritten)
^1741623227880

Was ist ein **forensisches Festplattenabbild**? #card  
Eine exakte, bitweise Kopie (Image) eines Datenträgers, erstellt z.B. mit dem Linux-Tool `dd`, zur Analyse ohne das Originalmedium zu verändern.
^1741623227884

Wie kann ein forensisches Festplattenabbild in Kali Linux eingebunden werden? #card  
- Minimaler Mount-Befehl:  
  `sudo mount /pfad/zu/festplatte.dd /mnt`  
- Danach Zugriff auf Festplatteninhalt unter `/mnt`
^1741623227889

Welche Software eignet sich besonders zur schnellen Wiederherstellung gelöschter Dateien (**Dateicarving**)? #card  
- **foremost** (Command-line-basiert, schnelle Wiederherstellung gelöschter Dateien anhand von Signaturen)
^1741623227894

Welche Software eignet sich zur gründlichen, GUI-gestützten forensischen Auswertung in Kali Linux? #card  
- **Autopsy** (Open-Source-Forensiksoftware)
^1741623227898

Wie lautet der Prozess, um ein Festplattenabbild in **Autopsy** zu analysieren? #card  
1. `sudo autopsy` im Terminal ausführen  
2. Webbrowser: `http://localhost:9999/autopsy` öffnen  
3. „New Case“ erstellen und Name vergeben  
4. „Add Host“ und anschließend Image File hinzufügen  
5. Analyse über File Analysis durchführen und gelöschte Dateien oder Dateisysteminhalte untersuchen
^1741623227902

Was ist eine typische **Untersuchungsfrage** in einem forensischen Fall? (Beispiel) #card  
- „Der Benutzer john hat ein Bild gelöscht – können Sie das wiederherstellen?“  
- „Wann wurde der Webserver durch eine SQL-Injection gehackt?“
^1741623227906

Wie können Webserver-Zugriffe zur Untersuchung eines SQL-Injection-Angriffs ausgewertet werden? #card  
- Durch Analyse von Webserver-Logdateien  
- Suchen nach auffälligen URL-Parametern (z.B. `debug`)  
- Nutzung von Tools wie `grep`, um Logs gezielt zu durchsuchen
^1741623227910

Welche Kriterien gehören in einen **forensischen Bericht**? (W-Fragen beachten!) #card  
- Was ist passiert? (Sachverhalt)  
- Wann ist es passiert? (Zeitpunkte, Zeiträume)  
- Wo sind die Spuren? (Systeme, Datenquellen)  
- Wie wurde die Untersuchung durchgeführt? (Methodik)  
- Welche Ergebnisse und Erkenntnisse gibt es? (Analyseergebnisse)  
- Warum sind diese Erkenntnisse relevant? (Bewertung)
^1741623227914
