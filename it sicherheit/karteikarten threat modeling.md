---
cards-deck: it sicherheit
---



Was ist Threat Modeling im Kontext sicherer Softwareentwicklung? #card  
**Threat Modeling** ist ein strukturierter Prozess, um **mögliche Bedrohungen** für eine Software oder ein System **frühzeitig** zu erkennen und Gegenmaßnahmen zu planen. Dabei werden **Systemkomponenten**, **Datenflüsse** und **Assets** erfasst, um **Angriffsszenarien** zu identifizieren.
^1741260180657

Welche Schritte sind typisch für ein Threat Modeling? #card  
1. **Ziele & Scope festlegen** (Welche Teile der Anwendung betrachten wir?)  
2. **System & Assets definieren** (Komponenten, Daten, Benutzerrollen)  
3. **Datenflüsse und Interaktionen** darstellen (z. B. in einem Datenflussdiagramm)  
4. **Bedrohungen identifizieren** (z. B. mit STRIDE, Attack Trees)  
5. **Risikobewertung** (Einschätzung von Schadensausmaß und Eintrittswahrscheinlichkeit)  
6. **Gegenmaßnahmen** entwickeln und **priorisieren**  
7. **Ergebnisse dokumentieren** und **regelmäßig aktualisieren**.
^1741260180663

Was bedeutet das STRIDE-Modell? #card  
**STRIDE** ist ein **Akronym** für häufige **Bedrohungskategorien** in IT-Systemen:  
- **S**poofing Identity (Identitätsvortäuschung)  
- **T**ampering with Data (Datenmanipulation)  
- **R**epudiation (Abstreitbarkeit)  
- **I**nformation Disclosure (unbefugte Offenlegung)  
- **D**enial of Service (Dienstverweigerung)  
- **E**levation of Privilege (Privilegienerweiterung)
^1741260180669

Wie können Datenflussdiagramme (Data Flow Diagrams, DFD) im Threat Modeling helfen? #card  
- Zeigen **Systemkomponenten**, **Datenquellen** und **Datenflüsse** zwischen ihnen.  
- Machen **Schnittstellen** sichtbar, an denen potenziell **Angriffe** erfolgen können.  
- Hervorheben, **wo** Daten **verarbeitet**, **gespeichert** und **übertragen** werden.  
- Grundlage, um **Bedrohungskategorien** systematisch zuzuordnen.
^1741260180674

Was ist ein „Threat Tree“? #card  
- Visuelle Darstellung, ähnlich einem **Baumdiagramm**, bei dem der **Root** ein **unerwünschtes Ereignis** ist (z. B. „Datenklau“).  
- Jede Ebene zeigt **Ursachen** oder **Wege**, wie dieser Vorfall eintreten kann.  
- Hilft, **konkrete Angriffswege** zu identifizieren und zu **bewerten**.
^1741260180680

Wie bewertet man die gefundenen Bedrohungen? #card  
- Typisch ist eine Einschätzung nach **Eintrittswahrscheinlichkeit** und **Auswirkung** (z. B. Low / Medium / High).  
- Zusammenführen zur **Risiko-Klasse** (z. B. in einer **Risikomatrix**).  
- Entscheidungen zu **Prioritäten** für Gegenmaßnahmen.
^1741260180685

Warum ist die regelmäßige Aktualisierung des Threat Models wichtig? #card  
- **Änderungen** im Code, in **Abhängigkeiten** oder in der **Architektur** können neue Angriffsvektoren öffnen.  
- **Neue Technologien** oder **Frameworks** bringen ggf. andere Risiken mit sich.  
- **Bedrohungslandschaft** verändert sich ständig, wodurch neue Angriffsmethoden entstehen können.
^1741260180691

Was unterscheidet Threat Modeling von einem Penetrationstest? #card  
- **Threat Modeling**: **Frühzeitige** Identifikation von Bedrohungen im **Design** und **Architektur** (präventiv).  
- **Penetrationstest**: **Praktischer Test** des laufenden oder fast fertigen Systems, um **konkrete Lücken** aufzuspüren.  
- Kombiniert ergibt sich ein **umfassendes Sicherheitsbild**.
^1741260180696

Wie unterstützt ein „Mitigation Plan“ das Threat Modeling? #card  
- **Mitigation Plan** listet alle **Identifizierten Bedrohungen** und dazu passende **Sicherheitsmaßnahmen**.  
- Enthält **Umsetzungsdetails**, Priorisierung und ggf. **Verantwortlichkeiten**.  
- Stellt sicher, dass **erkannte Risiken** nicht nur dokumentiert, sondern auch **behoben** werden.
^1741260180701

Welche Vorteile hat ein strukturiertes Threat Modeling? #card  
- **Frühes Erkennen** von Sicherheitsproblemen reduziert spätere **Kosten** und **Aufwand**.  
- Klare **Kommunikation** im Team über **Risiken** und **Maßnahmen**.  
- Hilft, **Design-Entscheidungen** und ihre **Sicherheitsauswirkungen** besser zu verstehen.  
- Fördert **proaktives Denken** aus Sicht eines Angreifers.
^1741260180706
