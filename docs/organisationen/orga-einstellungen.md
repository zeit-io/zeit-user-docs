# Einstellungen für die Organisation

Wenn Sie im Kontext der Organisation sind, dann finden Sie im Hauptmenü, ganz rechts, den Punkt "Einstellungen".
Hier können Sie die Einstellungen für die Organisation vornehmen. Bei den Einstellungen haben Sie folgenden Untersektionen:

## Name

Jede Organisation auf ZEIT.IO hat einen eindeutigen Namen auf ZEIT.IO. Diesen eindeutigen Namen können Sie hier ändern.
Es können nur Namen gewählt werden, die noch nicht von einer anderen Organisation auf ZEIT.IO verwendet werden.
Das Ändern des Namens der Organisation wirkt sich auf alte Links aus.
Es kann sein, dass nach einer Namensänderung alte Links (URLs) zu Reports innerhalb dieser Organisation nicht mehr funktionieren werden.

## Allgemein

Hier können Sie folgenden Standardwerte für Ihre Organisation festlegen:

- **Währung**: Die Währung, in der die Rechnungen erstellt werden sollen.
- **Steuersatz**: Der Standard-Steuersatz, der für die Rechnungen verwendet werden soll.
- **Sprache**: Die Sprache, in der die Benutzeroberfläche von ZEIT.IO angezeigt werden soll.
- **Urlaubspräfix für Kalendereinträge**: Das Präfix, das für Urlaubs-Kalendereinträge verwendet werden soll.
- **Pflichtfeld Bestellnummer**: Hier können Sie konfigurieren ob bei Projekten die Bestellnummer ein Pflichtfeld sein soll.
- **Pflichtfeld Projektnummer**: Hier können Sie konfigurieren ob bei Projekten die Projektnummer ein Pflichtfeld sein soll.

## Rechnungsadresse

Hier können Sie die folgenden Daten hinterlegen:

- **Branche**: Die Branche, in der Ihre Organisation tätig ist.
- **Rechnungsadresse**: Die offizielle Rechnungsadresse Ihrer Organisation. Samt Rechtsform, Steuernummer und Handelsregisternummer.
- **Kontaktdaten**: Die allgemeinen Kontaktdaten Ihrer Organisation.
- **Rechnungsempfänger**: Eine E-Mail-Adresse für eingehende Rechnungen. An diese E-Mail Adresse werden Sie auch die Rechnungen von ZEIT.IO erhalten.

Die Angaben hier werden auch verwendet für den Footer auf Ausgangsrechnungen und Gutschriften, die von ZEIT.IO erstellt werden.

## Rechnungsnummer

Hier können Sie das Format für die Rechnungsnummer festlegen, welches für Ausgangsrechnungen verwendet werden soll.
Gutschriften haben einen eigenen Nummernkreis, der separat konfiguriert werden kann.
Hier nachfolgend sind die möglichen Optionen beschrieben:

### FORTLAUFENDE-NUMMER

Diese Option entspricht dem Format: `<FORTLAUFENDE-NUMMER>`.<br/> 
Also z.B.: `123`.<br/>
Bei dieser Option wird eine fortlaufende Nummer für die Rechnungen verwendet.
Sie können die aktuelle Rechnungsnummer konfigurieren und die Mindestlänge für die Rechnungsnummer.
Wenn die aktuelle Rechnungsnummer kleiner ist als die Mindestlänge, dann wird die Nummer mit führenden 0en aufgefüllt.
Hier ein Beispiel. Die aktuelle Rechnungsnummer ist z.B. 199 und als Mindestlänge ist 5 eingestellt.
Dann wäre die nächste Rechnungsnummer: `00200`.

Dieses Format ist immer fortlaufend und wird auch am Jahresende nicht zurückgesetzt!

###  PREFIX - FORTLAUFENDE-NUMMER

Diese Option entspricht dem Format: `<PREFIX>-<FORTLAUFENDE-NUMMER>`.<br/>
Also z.B.: `RE-123`.<br/>
Sie können hier ein Präfix für die Rechnungsnummer festlegen, die aktuelle Nummer und die Mindestlänge für die fortlaufende Nummer.
Die Rechnungsnummer wird am Jahresende nicht zurückgesetzt! Bei diesem Format läuft die Nummer immer fortlaufend weiter.

###  FORTLAUFENDE-NUMMER/JAHR

Diese Option entspricht dem Format: `<FORTLAUFENDE-NUMMER>/<JAHR>`.<br/>
Also z.B.: `123/2025`.<br/>
Die fortlaufende Nummer wird am Jahresende zurückgesetzt und das Jahr wird in der Rechnungsnummer hinten eingefügt.
Rechnungen im neuen Jahr starten dann wieder mit der Rechnungsnummer 1.
Wie auch bei der ersten Option, können Sie sowohl die aktuelle Nummer als auch die Mindestlänge für die fortlaufende Nummer festlegen.

###  JAHR-FORTLAUFENDE-NUMMER

Diese Option entspricht dem Format: `<JAHR>-<FORTLAUFENDE-NUMMER>`.<br/>
Also z.B.: `2025-123`.<br/>
Das Jahr wird vorne in der Rechnungsnummer eingefügt, gefolgt von einer fortlaufenden Nummer. 
Die fortlaufende Nummer wird am Jahresende zurückgesetzt. Rechnungen im neuen Jahr starten dann wieder mit der Rechnungsnummer 1.
Wie auch bei der ersten Option, können Sie sowohl die aktuelle Nummer als auch die Mindestlänge für die fortlaufende Nummer festlegen.

###  JAHR MONAT TAG - TAGESZÄHLER

Diese Option entspricht dem Format: `<JAHR><MONAT><TAG>-<TAGESZÄHLER>`.<br/> 
Also z.B.: `20250101-1`.<br/>
Die Rechnungsnummer besteht aus dem Jahr, dem Monat, dem Tag und einem fortlaufenden Tageszähler.
Der Tageszähler wird jeden Tag zurückgesetzt. Rechnungen am gleichen Tag erhalten dann die Nummern 1, 2, 3, usw.
Wie auch bei der ersten Option, können Sie sowohl die aktuelle Nummer als auch die Mindestlänge für die fortlaufende Nummer festlegen.

### JAHR MONAT - MONATSZÄHLER

Diese Option entspricht dem Format: `<JJ><MONAT>-<MONATSZÄHLER>`. <br/>
Also z.B.: `2501-1`.<br/>
Die Rechnungsnummer besteht aus dem Jahr, dem Monat und einem fortlaufenden Monatszähler.
Der Monatszähler wird jeden Monat zurückgesetzt. Rechnungen im gleichen Monat erhalten dann die Nummern 1, 2, 3, usw.
Wie auch bei der ersten Option, können Sie sowohl die aktuelle Nummer als auch die Mindestlänge für die fortlaufende Nummer festlegen.

### PREFIX-JAHR-FORTLAUFENDE-NUMMER

Diese Option entspricht dem Format: `<PREFIX>-<JAHR>-<FORTLAUFENDE-NUMMER>`.<br/> 
Also z.B.: `RE-2025-123`.<br/>
Sie können hier ein Präfix für die Rechnungsnummer festlegen, die aktuelle Nummer und die Mindestlänge für die fortlaufende Nummer.
Das Jahr wird immer automatisch gesetzt! Die fortlaufende Rechnungsnummer wird am Jahresende zurückgesetzt!

### PREFIX-JJ-FORTLAUFENDE-NUMMER

Diese Option entspricht dem Format: `<PREFIX>-<JJ>-<FORTLAUFENDE-NUMMER>`.<br/> 
Also z.B.: `RE-25-123`.<br/>
Sie können hier ein Präfix für die Rechnungsnummer festlegen, die aktuelle Nummer und die Mindestlänge für die fortlaufende Nummer.
Das Jahr wird immer automatisch gesetzt! Die fortlaufende Rechnungsnummer wird am Jahresende zurückgesetzt!

### PREFIX-JJFORTLAUFENDE-NUMMER

Diese Option entspricht dem Format: `<PREFIX>-<JJ><FORTLAUFENDE-NUMMER>`.<br/> 
Also z.B.: `RE-25123`.<br/>
Sie können hier ein Präfix für die Rechnungsnummer festlegen, die aktuelle Nummer und die Mindestlänge für die fortlaufende Nummer.
Das Jahr wird immer automatisch gesetzt! Die fortlaufende Rechnungsnummer wird am Jahresende zurückgesetzt!


## Gutschriftsnummer

Hier können Sie das Format für die Gutschriftsnummer festlegen, welches für Gutschriften verwendet werden soll.

## Bankverbindungen

Hier können Sie die Bankverbindungen für Ihre Organisation hinterlegen.
Wenn Sie das Rechnungsmodul nutzen wollen, dann müssen Sie mindestens eine Bankverbindung hinterlegen.
Bei den Kunden können Sie jedem Kunden eine andere Bankverbindung zuweisen.
Bei einer Ausgangsrechnung an einen Kunden, wird dann die Bankverbindung, die Sie dem Kunden zugewiesen haben, verwendet
und im Footer der Rechnung angezeigt.

## Logo

Hier können Sie das Logo für Ihre Organisation hochladen.
Sie können ein Logo hochladen, welches für alle Rechnungen und Gutschriften verwendet wird.
Und Sie können ein separates Logo hochladen, welches in der Anwendung angezeigt wird.

## Margenberechnung

Hier können Sie einstellen, wie die prozentuale Marge in den Projekten berechnet werden soll.

## Gutschrifts-Strategie

Hier können Sie verschiedene Strategien für das Gutschriftverfahren festlegen.

## Benachrichtigungen

Hier können Sie verschiedene E-Mail-Verteiler konfigurieren für Benachrichtigungen.
Es gibt verschiedene Events in ZEIT.IO, für die Benachrichtigungen versendet werden können.
So z.B. für eingereichte Urlaube, Krankmeldungen oder für neue Eingangsrechnungen.

## Feiertage

Hier können Sie das Bundesland konfigurieren, für die Feiertage in der Organisation.
Außerdem können Sie hier zusätzliche Feiertage für die Organisation hinterlegen.

## Datenaufbewahrung

Hier können Sie die Richtlinie zur Datenaufbewahrung für Ihre Organisation festlegen.
Die Richtlinie zur Datenaufbewahrung legt fest, wie lange Daten in ZEIT.IO aufbewahrt werden.
Nach Ablauf der Frist werden die Daten automatisch gelöscht!

Aktuell können Sie hier einstellen, wie lange die Arbeitszeiten von festangestellten Mitarbeitern gespeichert werden sollen.
Diese Einstellung hat keine Auswirkung auf die Zeiten von Lieferanten/Freiberuflern.

Ein Background-Job für die Richtlinie zur Datenaufbewahrung wird einmal täglich ausgeführt.
Dieser Background-Job löscht alle Daten, die älter sind als die festgelegte Frist.
**Einmal gelöschte Daten können nicht wiederhergestellt werden!**
Wenn Sie den Wert z.B. auf 2 Jahre setzen, dann werden spätestens am nächsten Tag alle Daten gelöscht, die älter als 2 Jahre sind.

## Hauptmenü

Hier können Sie konfigurieren, welche Menüpunkte im Hauptmenü angezeigt werden sollen.

## AddOns

Hier können Sie AddOns für Ihre Organisation aktivieren.

## API Key

Hier finden Sie den API Key für Ihre Organisation.
Mit diesem API Key können Sie die ZEIT.IO API nutzen und programmatisch auf Ihre Daten zugreifen.

## Auditlogs

Hier finden Sie die Auditlogs für Ihre Organisation.
Hier können Sie sehen, wer wann welche Änderungen an den Einstellungen der Organisation vorgenommen hat.
