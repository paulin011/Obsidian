

Was ist der Data Encryption Standard (DES)? #card  
- **DES** ist ein **symmetrisches Blockchiffre-Verfahren** mit einer **Blockgröße** von 64 Bit und einem **Schlüssel** von 56 Bit.  
- Entwickelt in den 1970er Jahren, war es lange **US-Standard**, gilt aber heute durch den kleinen Schlüsselraum als **unsicher** (anfällig für Brute-Force).

Was ist die Triple-DES (3DES)-Erweiterung? #card  
- **3DES** ist eine **Verkettung** von drei aufeinanderfolgenden **DES-Verschlüsselungen** (EN-DE-EN oder EN-EN-EN).  
- Bietet mehr Sicherheit als **DES** alleine, ist aber relativ **langsam** und wurde durch **AES** weitgehend ersetzt.

Was ist AES (Advanced Encryption Standard)? #card  
- Aktueller **symmetrischer Standard**-Algorithmus mit **128-Bit-Blöcken**.  
- Unterstützt **Schlüssellängen** von 128, 192 oder 256 Bit.  
- **Sehr effiziente** und **sicher** geltende Blockchiffre, von der US-Regierung als Nachfolger von DES festgelegt (FIPS 197).

Wie funktioniert ein One-Time Pad (OTP)? #card  
- **Beweisbar sicheres** Verfahren, bei dem die **Länge des Schlüssels** mindestens so groß ist wie der **Klartext**.  
- Verschlüsselung durch **XOR** des Klartexts mit einem **zufälligen** und **nur einmal verwendbaren** Schlüssel-Stream.  
- Praktisch aufwendig, da Schlüsseldistribution und -länge sehr groß sein müssen.

Was macht das One-Time Pad so besonders sicher? #card  
- Beweisbar **unmöglich zu brechen**, wenn der Schlüssel **zufällig**, **mindestens so lang** wie der Klartext und **nur einmal** benutzt wird.  
- Jeder mögliche Klartext kann **gleich wahrscheinlich** entstehen, wodurch ein Angreifer keine Informationen erhält.

Was ist die Vigenère-Chiffre? #card  
- Eine **polyalphabetische** **Substitutionschiffre**, bei der ein **Schlüsselwort** wiederholt über den Klartext gelegt wird.  
- Jeder Buchstabe wird um die Anzahl Stellen verschoben, die der jeweilige **Buchstabe** im Schlüsselwort vorgibt.  
- Galt lange als „unbrechbar“, ist aber durch **Kasiski-Test** und **Friedman-Test** angreifbar.

Wie unterscheidet sich die Vigenère-Chiffre von einer einfachen Caesar-Verschiebung? #card  
- **Caesar**: Verschiebt alle Buchstaben **gleich** (monoalphabetisch).  
- **Vigenère**: Wechselt je nach **Buchstaben** im Schlüsselwort zwischen **verschiedenen** Verschiebungen (polyalphabetisch).

Warum ist DES heute nicht mehr als sicher genug eingestuft? #card  
- **56-Bit-Schlüssellänge** ist zu kurz für heutige Rechenkapazitäten – ein **Brute-Force-Angriff** ist realistisch.  
- DES kann daher innerhalb akzeptabler Zeit geknackt werden und wurde durch sicherere Alternativen wie **AES** ersetzt.

Warum ist AES derzeit der empfohlene symmetrische Standard? #card  
- **Ausreichend großer Schlüsselraum** (128–256 Bit).  
- **Effizient** auf moderner Hardware (auch für kleine Geräte).  
- **Weit verbreitet**, gründlich **analysiert** und als **sehr sicher** eingestuft.

Was ist der ECB-Modus bei Blockchiffren? #card  
- **ECB** (Electronic Code Book) ist ein **Betriebsmodus** für Blockchiffren.  
- Jeder **Block** des Klartexts wird **unabhängig** mit demselben Schlüssel verschlüsselt.  
- Einfach, aber **unsicher**, weil **gleiche Klartextblöcke** zu **gleichen Chiffratblöcken** führen und Muster sichtbar bleiben.

Warum ist ECB häufig nicht empfohlen? #card  
- Identische Klartextblöcke erzeugen **identische** Chiffratblöcke.  
- Bestimmte **Strukturen oder Muster** im Klartext bleiben erkennbar.  
- Damit bietet ECB **wenig Vertraulichkeit** im Vergleich zu anderen Modi (CBC, CTR etc.).
