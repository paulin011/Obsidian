Overplotting reduktion

1. Jitter
	• Jitter fügt random Rauschen in die Daten ein um 
	Overplotting zu vermeiden
	• Besonders nützlich für gerundete Zahlen
	• Nachteile
	• Funktioniert nur wenn genug Platz vorhanden ist
	• Position ist nur noch unscharfe Repräsentation der 
	Werte
2. Anzeige des Überdeckungsgrad
	Heatmap
		• Unterteilung des Raums in Regionen
		• Repräsentation der Dichte durch Farbe 
		• Vorteil: 
		• Kein Overplotting
		• Dichte Objektwertebereiche sichtbar 
		• Skaliert für sehr viele Objekte
	 Nachteil:
		• Details - Werte gehen verloren
![[Pasted image 20241113111149.png]]
3. Lokale verzerrung Lupe oder Fisheye
	+ zeigt Details in wichtigen dichten Regionen 
	-- Lokale Linse benötigt Interaktivität
	![[Pasted image 20241113111700.png]]
4. Globale Verzerrung
	![[Pasted image 20241113112019.png]]
	6/12 da 6 datenpunkte usw und dann clustern
	+ zeigt Details in wichtigen dichten Regionen 
	+ keine Interaktivität notwendig
	- begrenzte Möglichkeit Details zu zeigen
	- Verzerrung vom ganzen Datensatz