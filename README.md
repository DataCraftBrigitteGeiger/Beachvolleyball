# Beachvolleyball

Beachvolleyball-Strategie

Aufgabe:
Entwickle ein Programm (einen Simulator), welches für die individuelle Spielstärke einer Mannschaft und die individuelle Spielstärke ihrer Gegnermannschaft die optimale Risikostrategie berechnet. Konkret: Welche Mannschaft sollte wieviel Risiko [0-10] fahren/benutzen, um langfristig (in z.B. 1000 Spielen) eine möglichst hohe Sieg-Anzahl zu schaffen (zu erwarten)? Die Strategie darf in Abhängigkeit vom Spielstand verändert werden.

Beispiel:
Mannschaft A hat Spielstärke 6, Mannschaft B hat Spielstärke 8 (Eingabe/Benutzerinput).
Niedriges Risiko bedeutet, dass jeder Ballwechsel mit einer Wahrscheinlichkeit entsprechend den beiden Spielstärken erfolgreich oder nicht erfolgreich ausgeht. Hohes Risiko bedeutet, dass die Erfolgschance eines Ballwechsels weit von der jeweiligen Spielstärke einer Mannschaft abweichen kann.
Wieviel Risko sollte Mannschaft A benutzen, um gegen Mannschaft B auf 1000 Spiele hin gesehen möglichst oft gewinnt?
Infos:
-	Ein Match (Spiel) besteht aus nur einem Satz (Vereinfachung).
-	Ein Satz endet bei 21 Punkten. Gewinner brauchen 2 Punkte Vorsprung, d.h. der Satz geht evtl. in die Verlängerung, solange bis 2 Punkte Vorsprung erreicht wurden.
-	Jeder Ballwechsel (=Rallye, z.B. 6x hin/her über das Netz) endet als Punkt für eine der beiden Mannschaften (Zufallsexperiment basierend auf Spielstärken und Risikowahl der beiden Mannschaften).
-	Relevant für die Aufgabenstellung ist immer nur der letzte von maximal drei möglichen Ballkontakten (wie Tennis). Berücksichtigung/Differenzierung von unterschiedlich vielen Ballkontakten nur falls noch Bearbeitungszeit übrig ist.
-	Spielstärke [0-10] drückt sich hier aus als durchschnittliche Return-Frequenz (erfolgreich zurückgespielte Bälle): Ein Team mit Spielstärke 9 spielt bei mittlerem Risiko durchschnittlich 90 % aller angenommenen Bälle mit spätestens dem dritten Kontakt erfolgreich ins gegnerische Feld zurück.
-	Risiko [0-10] drückt sich hier aus als Bereitschaft, von der aktuellen Spielstärke abzuweichen (Zufallsexperiment, kann zu Schwankung nach oben oder nach unten führen), d.h. den aktuellen Ballwechsel mit einer Erfolgschance zu beenden, die um die Spielstärke streut. 
Anforderungen:
-	Benutzeroberfläche mit Bedienelementen (Buttons, Menüs, Infoboxen, Eingabemasken…)
-	Funktionen, die die Eingaben des Benutzers/der Benutzerin erfassen und in die Strategieempfehlung mit einbeziehen:
o	Spielstärke des Benutzers [0-10]
o	Spielstärke der Gegner [0-10]
Methoden/Werkzeuge, die benutzt werden müssen:
-	Numpy
-	Pandas
-	Verteilungen (numpy.random…..)
-	Benutzeroberfläche mit tkinter
-	Git
