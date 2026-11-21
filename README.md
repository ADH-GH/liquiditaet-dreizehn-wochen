# Liquiditätsvorschau über dreizehn Wochen

Die Seite legt offene Forderungen, offene Rechnungen, feste Zahlungen und Planwerte auf
dreizehn Wochen und zeigt je Woche Einzahlungen, Auszahlungen und den Stand am Ende gegen die
Kreditlinie. Forderungen rechnet sie mit Fälligkeit plus dem Abstand, mit dem der jeweilige
Kunde bisher gezahlt hat. Reicht die Linie nicht, arbeitet das Team an der Woche: Zusage vom
Kunden, Verschiebung einer Lieferantenzahlung mit Freigabe, und jede Woche wird die Vorschau
vorgelegt und freigegeben.

Zur Lösung gehört kein Agent. Deshalb liegt in diesem Repo nur die HTML-Datei.

**Das Video zeigt die Lösung:** [demo.mp4](docs/demo.mp4), etwa 2 Minuten. Dieses Repo enthält die
Grundlage dazu. Showroom ADH, Stand 04.12.2026. Firma, Personen und Zahlen im Beispiel sind erfunden.

## Ausprobieren

`index.html` per Doppelklick öffnen. Kein Build, kein Server, keine Installation. Alle Eingaben
bleiben im Browserfenster.

1. `index.html` öffnen. Kontostand 182.000 €, Kreditlinie 75.000 €. In KW 4 steht der
   Stand bei −89.900 €, es fehlen 14.900 €.
2. Die Posten der KW 4: Löhne, Sozialversicherung, Darlehen und eine Lieferantenrechnung über
   61.000 € treffen zusammen.
3. Annahmen: Demo Chemie zahlt üblicherweise 30 Tage nach Fälligkeit. Deshalb steht deren
   Rechnung vom Januar erst in KW 7.
4. Als Tobias Lindner: Posten V-07, neuer Zahltag `12.02.2027`, Begründung, eintragen.
5. Als Petra Sommer freigeben. KW 4 steht jetzt bei −28.900 € und bleibt in der Linie.
6. Posten „Sozialversicherung Januar“ wählen und eintragen: verweigert, gesetzliche Frist.
7. Zweiter Fall, als Carsten Brandt: Forderung F-08, Zusage für den `29.01.2027`. Wirkt
   sofort, ohne Freigabe, und ist am Posten als Zusage vermerkt.
8. Als Paul Richter vorlegen, als Petra Sommer freigeben.
9. Protokoll zeigen.

## Grenzen

- Im Browser geöffnet und an den Kennzahlen der Beispieldaten geprüft. Im Alltag nicht erprobt.
- Alle Beträge sind Zahlbeträge, so wie sie auf dem Konto ankommen oder abgehen. Die Seite
  unterscheidet nicht zwischen netto und brutto.
- Die Termine der festen Zahlungen folgen üblicher Praxis: Lohnsteuer und Umsatzsteuer zum
  Zehnten, Sozialversicherung am drittletzten Bankarbeitstag, Löhne zum Monatsende. Geprüft
  hat das niemand, und Feiertage sind nicht berücksichtigt.
- Der Abstand je Kunde ist ein fester Wert. Eine Streuung oder ein Ausfall kommt nicht vor.
- Eine Zahlungszusage wirkt sofort und ohne Freigabe. Sie ist eine Annahme und am Posten so
  gekennzeichnet.
- Posten, die nach der dreizehnten Woche liegen, zeigt die Seite nicht.
- Die Vorschau zeigt die Lage am Ende jeder Woche. Ein Engpass innerhalb einer Woche, etwa
  am Tag des Lohnlaufs, kann tiefer liegen.

## Rechte

Alle Rechte vorbehalten, Alf-David Heermann 2026. Der Quelltext ist zum Ansehen und Ausprobieren
veröffentlicht. Kontakt: https://www.linkedin.com/in/alf-david-heermann
