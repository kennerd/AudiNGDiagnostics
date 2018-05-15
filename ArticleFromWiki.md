### Blinkcode (NG)
* Taken from: [Wikipedia Article (15. May 2018)](http://www.audi-80-wiki.de/index.php?title=Blinkcode_(NG))

## Wichtige Informationen vor dem Auslesen des Fehlerspeichers
* Das Auslesen des Fehlerspeichers über den Blinkcode gilt ausschließlich für Motoren mit dem Motorkennbuchstaben NG!
* Vor dem Auslesen des Fehlerspeichers ist das Fahrzeug in möglichst allen Last- und Drehzahlbereichen zu fahren. Der Motor darf nicht abgestellt werden, da nach dem Abstellen der Fehlerspeicher geleert wird. Es sind alle Verbraucher auszuschalten.

## Fehlerspeicher auslesen
* Anklemmen der Prüflampe an Plus (+) des schwarzen Steckers und an "L" des weißen Steckers
 * Die Prüflampe leuchtet nicht auf
* Bildung einer Drahtbrücke zwischen Minus (-) des schwarzen Steckers und "L" des weißen Steckers
 * Die Prüflampe leuchtet auf
 * Drahtbrücke für ca. 5 Sekunden beibehalten, danach entfernen
* Nach dem Entfernen der Drahtbrücke wird ein Blinkcode ausgegeben
 * Die Blinkfolge beginnt mit einem 2,5-sekündigen Startzeichen und einer 2,5-sekündigen Pause
 * Es werden anschließend 4 Blöcke ausgegeben, wobei jeder Block eine Zahl bildet
 * Das Ende wird durch eine 2,5-sekündige Pause und ein 2,5-sekündiges Endezeichen signalisiert
 * Die Ausgabe wiederholt sich
* Auslesen weiterer Fehler
 * Erneutes Setzen der Drahtbrücke zwischen Minus (-) des schwarzen Steckers und "L" des weißen Steckers für 5 Sekunden
 * Entfernen der Drahtbrücke
 * Auslesen des nächsten Fehlers (beschrieben in Punkt 3)
* Wird der der Block 4-4-4-4 ausgegeben sind keine weiteren Fehler auf dem Steuergerät abgelegt

## Zusatzinformationen
* Das Motorsteuergerät (für KE-III-Jetronic) und das Zündsteuergerät (VEZ-K) legen ihre Fehler getrennt ab. Das Zündsteuergerät beginnt mit der Ausgabe der Fehlercodes.

## Blinkcodetabelle

|Code   | Fehler
|-------|------- 
|0000   | Ausgabe Ende
|1111   | Zünd- oder Motorsteuergerät defekt
|1231   | Geber für Fahrgeschwindigkeit G68
|2121   | Leerlaufschalter F60
|2122   | Drehzahlinformation fehlt
|2123   | Volllastschalter F81
|2132   | Datenleitung defekt
|2141   | Erste Klopfregelung
|2142   | Klopfsensor I G61
|2223   | Höhengeber F96
|-------|------- 
|232    | Luftmengenmesser G19/G70
|233    | Luftmengenmesser Referenzspannung G70
|312    | Kühlmittleltemperaturgeber G62
|341    | Lambdaregelung
|342    | Lambdasonde G39 mit Heizung
|431    | Ventil für Leerlaufstabilisierung
|444    | Kein Fehler im Fehlerspeicher
|-------|-------
