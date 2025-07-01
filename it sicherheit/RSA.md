# RSA Beispiel mit kleinen Zahlen

In diesem Beispiel wählen wir zwei kleine Primzahlen und demonstrieren Schritt für Schritt, wie der RSA-Algorithmus funktioniert. Dabei werden wir alle nötigen Berechnungen durchführen, sodass sie auch ohne Taschenrechner nachvollziehbar sind.

## 1. Wahl der Primzahlen

Wähle zwei kleine Primzahlen:

$$
p = 3 \quad \text{und} \quad q = 11
$$

## 2. Berechnung von \( n \)

Berechne \( n \) als Produkt der beiden Primzahlen:

$$
n = p \cdot q = 3 \cdot 11 = 33
$$

## 3. Berechnung von \(\varphi(n)\) (Eulersche Phi-Funktion)

Die Eulersche Phi-Funktion für \( n \) ist gegeben durch:

$$
\varphi(n) = (p-1)(q-1)
$$

Berechne:

$$
\varphi(n) = (3-1)(11-1) = 2 \cdot 10 = 20
$$

## 4. Wahl des öffentlichen Exponenten \( e \)

Wähle \( e \) so, dass $( 1 < e < \varphi(n) ) und ( \gcd(e, \varphi(n)) = 1 )$.  
Ein einfacher Kandidat ist:

$$
e = 3
$$

Prüfung:

$$
\gcd(3, 20) = 1
$$

Da 3 und 20 teilerfremd sind, ist \( e = 3 \) zulässig.

## 5. Berechnung des privaten Exponenten \( d \)

\( d \) ist der modulare Inverse von \( e \) modulo $(\varphi(n)\)$. Das heißt, \( d \) muss die Gleichung erfüllen:

$$
e \cdot d \equiv 1 \pmod{\varphi(n)}
$$

Für \( e = 3 \) und $(\varphi(n) = 20)$ suchen wir \( d \), sodass:

$$
3 \cdot d \equiv 1 \pmod{20}
$$

Durch Ausprobieren findet man:

- $( 3 \cdot 7 = 21 ) und ( 21 \mod 20 = 1 )$

Daher ist:

$$
d = 7
$$

## 6. Zusammenfassung des Schlüsselpaares

- **Öffentlicher Schlüssel:** \((n, e) = (33, 3)\)
- **Privater Schlüssel:** \((n, d) = (33, 7)\)

---

# Verschlüsselung und Entschlüsselung

Wir zeigen nun, wie eine Nachricht \( m \) verschlüsselt und wieder entschlüsselt wird. Nehmen wir als Beispiel:

$$
m = 4
$$

## 7. Verschlüsselung

Die Verschlüsselung erfolgt nach der Formel:

$$
c = m^e \mod n
$$

Berechne:

$$
c = 4^3 \mod 33 = 64 \mod 33
$$

Da:

$$
64 = 33 \cdot 1 + 31
$$

ist:

$$
c = 31
$$

## 8. Entschlüsselung

Die Entschlüsselung erfolgt nach der Formel:

$$
m = c^d \mod n
$$

Berechne:

$$
m = 31^7 \mod 33
$$

Ein Trick: Beachte, dass $( 31 \equiv -2 \pmod{33} )$. Damit können wir schreiben:

$$
31^7 \equiv (-2)^7 \pmod{33}
$$

Berechne \( (-2)^7 \):

$$
(-2)^7 = -128
$$

Nun bestimme den Rest bei Division durch 33. Wir suchen \( k \) mit:

$$
-128 + 33k = m
$$

Für \( k = 4 \):

$$
-128 + 33 \cdot 4 = -128 + 132 = 4
$$

Also:

$$
m = 4
$$

Das entspricht genau der ursprünglichen Nachricht.

---

# Zusammenfassung

1. **Primzahlen wählen:** \( p = 3 \), \( q = 11 \)
2. **Berechne \( n \):** \( n = 33 \)
3. **Berechne \(\varphi(n)\):** \( \varphi(n) = 20 \)
4. **Wähle \( e \):** \( e = 3 \)
5. **Berechne \( d \):** \( d = 7 \) (weil \( 3 \cdot 7 \equiv 1 \pmod{20} \))
6. **Verschlüsselung:** Für \( m = 4 \) wird \( c = 4^3 \mod 33 = 31 \)
7. **Entschlüsselung:** \( m = 31^7 \mod 33 = 4 \)

Dieses Beispiel zeigt, wie RSA funktioniert, auch wenn in der Praxis deutlich größere Zahlen verwendet werden, um die Sicherheit zu gewährleisten.
