# Projekte

Projekte sind ein zentraler Bestandteil von ZEIT.IO!
Jedes Projekt hat eine eindeutige Kennung, einen Namen, ein Start- und Enddatum, ein Stunden-Budget und ein Währungs-Budget.
Zeiten (TimeRecords), Ausgaben und Festpreis-Pakete können auf Projekte gebucht werden.
Projekte, die einer Organisation angehören, können von mehreren Personen bearbeitet werden.
Jedes Projekt hat eine Mitgliederliste, in der alle Personen aufgeführt sind, die auf das Projekt buchen dürfen.
Außerdem hat jedes Projekt auch eine Genehmigungsliste, in der alle Personen aufgeführt sind, die Buchungen auf dem Projekt genehmigen dürfen.

Wenn Sie im Kontext der Organisation sind, dann finden Sie im Hauptmenü den Punkt "Projekte".
Hier können Sie alle Projekte sehen, die zur Organisation gehören.

## Neues Projekt anlegen

Wenn Sie im Hauptmenü auf "Projekte" klicken, dann sehen Sie eine Liste aller Projekte, auf die Sie Zugriff haben.
Rechts oben auf der Seite befindet sich ein Button "Neues Projekt anlegen".
Wenn Sie da drauf klicken, dann öffnet sich ein Dialog, in dem Sie ein neues Projekt anlegen können.

## Projektfelder

Wenn Sie ein neues Projekt anlegen oder ein bestehendes Projekt bearbeiten, dann öffnet sich ein Formular mit verschiedenen Feldern.
Hier nachfolgend sind alle Felder detailliert erklärt.

### Projektart

Bei ZEIT.IO gibt es aktuell die zwei Projektarten "Time & Material" und "Festpreis".
Die Projektart bestimmt, wie die Marge im Projekt berechnet wird.

#### Time & Material

Bei der Projektart "Time & Material" wird das Projekt nach Aufwand abgerechnet.
Bei diesen Projekten hat man mit dem Kunden einen Stundensatz oder Tagessätze vereinbart und die angefallenen Aufwände werden entsprechend in Rechnung gestellt.

Bei Time & Material Projekten ist die Marge zu Beginn des Projektes immer 0.
Weil noch keine Aufwände gebucht wurden, gibt es auch keine Marge.

Die Marge wird auf Basis der gebuchten Zeiten berechnet.
Die Mitglieder im Projekt haben alle einen EK- und einen VK-Stundensatz hinterlegt.
Die Differenz zwischen dem VK- und dem EK-Stundensatz ist die Marge.

Hier ein Beispiel. Der Freiberufler Max Mustermann ist als Mitglied im Projekt hinterlegt und an seiner Projekt-Mitgliedschaft sind folgende Stundensätze hinterlegt:

- VK-Stundensatz: 100€
- EK-Stundensatz: 77€

Die Marge pro Stunde beträgt also 23€. Wenn er zwei Stunden auf das Projekt bucht, dann beträgt die Marge im Projekt 46€.
Mit jeder gebuchten Zeit erhöht sich die Marge im Projekt.

#### Festpreis

Bei der Projektart "Festpreis" wird das Projekt nach einem festen Preis abgerechnet.
Hierbei gehen wir davon aus, dass das hinterlegte Währungs-Budget für das Projekt auch der Festpreis ist.

Wenn das Projekt ein Währungs-Budget von 100.000€ hat, dann ist das auch der Festpreis, zu dem das Projekt abgerechnet wird.
Unabhängig davon, wie viele Stunden gebucht werden.

Für die Margenberechnung bedeutet das, dass die Marge im Projekt zu Beginn immer 100% beträgt.
Als Marge wind am Anfang immer das volle Währungs-Budget angezeigt. Also z.B 100.000€.
Weil noch keine Aufwände angefallen sind.
Wenn im Projekt dann Aufwände gebucht werden, dann sinkt die Marge entsprechend.

Hier ein Beispiel. Der Freiberufler Max Mustermann ist als Mitglied im Projekt hinterlegt und an seiner Projekt-Mitgliedschaft sind folgende Stundensätze hinterlegt:

- VK-Stundensatz: 100€
- EK-Stundensatz: 77€

Da es sich hierbei um ein Festpreis-Projekt handelt, ist der hinterlegte VK-Stundensatz für die Margenberechnung irrelevant.
Relevant ist in dem Fall nur der EK-Stundensatz.
Wenn Max jetzt zwei Stunden auf das Projekt bucht, dann verursacht er Kosten im Wert von 154€.
Dementsprechend sinkt die Marge im Projekt von 100.000€ auf 99.846€.
Jede gebuchte Zeit und jede gebuchte Ausgabe reduziert die Marge im Projekt.

### Name vs. Kennung

Jedes Projekt hat einen Namen und eine Kennung. Diese sind standardmäßig identisch, können aber auch unterschiedlich sein.
Der Name des Projektes ist relevant für das Rechnungsmodul.
Der Name wird auf Rechnungen und Gutschriften verwendet.
Setzen Sie den Projektnamen entsprechend so, wie sie das Projekt auf Ausgangsrechnungen und Gutschriften repräsentiert sehen wollen.

Die Projekt-Kennung muss eindeutig innerhalb der Organisation sein und wird innerhalb der Anwendung verwendet
um das Projekt anzuzeigen. So wird z.B. in der Projektauswahl für die Zeiterfassung immer die Projekt-Kennung angezeigt.
Und auch bei der Erfassung von Ausgaben wird bei der Projektauswahl immer die Projekt-Kennung angezeigt. Nicht der Name!

Sowohl Name als auch Kennung können jederzeit geändert werden.

### Projekt-Beschreibung

Jedes Projekt kann eine Beschreibung haben. Die Beschreibung ist optional und kann jederzeit geändert werden.
Die Beschreibung ist sichtbar für die Projekt-Mitglieder und Projekt-Genehmiger und kann verwendet werden, um zusätzliche Informationen zum Projekt bereitzustellen.

### Projektzeitraum

Jedes Projekt hat ein Start- und Ende-Datum.
Alle Buchungen (Zeiten, Ausgaben, Festpreis-Pakete) müssen innerhalb des Projekt-Zeitraums liegen.
Buchungen, die außerhalb des Projekt-Zeitraums liegen, können nicht auf das Projekt gebucht werden.
Start- und Ende-Date können jederzeit geändert werden.

### Budgets

Projekte auf ZEIT.IO haben folgende Budgets:

- **Stundenbudget**: Die Anzahl der Stunden, die maximal auf das Projekt gebucht werden dürfen.
- **Budget (Zeiterfassung)**: Das Währungs-Budget für Zeiterfassung. Diese Summer ergibt sich in der Regel aus dem Stundenbudget multipliziert mit dem durchschnittlichen VK-Stundensatz.
- **Budget (Ausgaben)**: Das Währungs-Budget für Ausgaben/Reisekosten.
- **Budget (Festpreis-Pakete)**: Das Währungs-Budget für Festpreis-Pakete.
- **Budget (Gesamt)**: Die Summe der drei Währungs-Budgets (Zeiterfassung, Ausgaben, Festpreis-Pakete).

Standardmäßig stellt ZEIT.IO sicher, dass diese Budgets eingehalten werden.
Wenn eine Buchung eines der Budgets überschreiten würde, dann wird die Buchung abgelehnt.
Es sei denn, die Option für "Überbuchungen erlauben" ist aktiviert.
In dem Fall können die Budgets auch überschritten werden.

!!! Info
    Wenn Zeiten auf das Projekt gebucht werden sollen, dann müssen zwingend Stundenbudget und Budget (Zeiterfassung) hinterlegt sein.
    Beide Felder müssen in dem Fall größer als 0 sein. Wenn eines der zwei Felder 0 ist, dann können keine Zeiten auf das Projekt gebucht werden!

### Projektnummer & Bestellnummer

Projekte können optional eine Projektnummer und eine Bestellnummer haben.

In den Einstellungen der Organisation, unter dem Punkt "Allgemein", kann konfiguriert werden, das die Bestellnummer ein Pflichtfeld sein soll.
Wenn diese Option aktiviert ist, dann muss bei der Erstellung eines neuen Projektes zwingend eine Bestellnummer hinterlegt werden!
Auf bereits bestehende Projekte hat dies erstmal keine Auswirkungen.
Die gleiche Option gibt es auch für die Projektnummer.
Auch die Projektnummer kann als Pflichtfeld konfiguriert werden.

Standardmäßig sind diese Felder aber keine Pflichtfelder.

Wenn eine Projektnummer oder Bestellnummer hinterlegt ist, dann wird diese auch auf Ausgangsrechnungen und Gutschriften verwendet.
Außerdem können dann Objekte, die dem Projekt zugeordnet sind, ebenfalls nach Projektnummer und/oder Bestellnummer gefiltert werden.
Dazu gehören folgende Objekte:

- Zeiten (TimeRecords)
- Ausgaben/Reisekosten
- Leistungsnachweise (Timesheets)
- Ausgangsrechnungen
- Eingangsrechnungen
- Gutschriften

Wenn die Bestellnummer/Projektnummer im Projekt geändert wird, dann wird die Änderung auch auf alle oben genannten Objekte übernommen.
Somit ist sichergestellt, dass die Filterung nach Projektnummer/Bestellnummer immer korrekt ist.

### Intervall

Mit dem Intervall im Projekt kann konfiguriert werden, wie feingranular die Zeiterfassung sein soll.
Standardmäßig ist die Zeiterfassung im Projekt minuten-genau.
Es können aber auch verschiedene Intervalle konfiguriert werden, wie z.B. 5 Minuten, 10 Minuten, 15 Minuten oder 30 Minuten.
In diesem Fall wird die Zeiterfassung immer auf das nächste Intervall gerundet.
So dass alle gebuchten Zeiten glatt durch ein Intervall teilbar sind.

Wenn z.B. ein 10 Minuten Intervall konfiguriert ist, dann wird eine Zeit von 12 Minuten auf 20 Minuten aufgerundet.
Jedes angefangene Intervall wird somit immer voll abgerechnet.

### Kunde

Jedes Projekt kann optional einem Kunden zugeordnet werden.
Im Dropdown für die Kundenauswahl tauchen nicht nur die Kunden auf, sondern auch die hinterlegten Abteilungen und Ansprechpartner der Kunden.
Im Idealfall weisen Sie das Projekt gleich der richtigen Abteilung, bzw. Ansprechpartner zu, die für den Rechnungsempfang zuständig ist.

Wenn Projektzeiten oder Ausgaben abgerechnet werden, dann ist das Rechnungsmodul mit dem Kunden vorbelegt, der dem Projekt zugeordnet ist.

Außerdem können Projekte, Zeiten, Ausgaben und Leistungsnachweise dann auch nach Kunden gefiltert werden.

### Ansprechpartner

Jedes Projekt kann optional einen Ansprechpartner haben.
Der Ansprechpartner ist sichtbar für alle Projektmitglieder und Projekt-Genehmiger.
Der Ansprechpartner kann verwendet werden, um eine Kontaktperson für das Projekt zu hinterlegen.

### Dynamische Felder

Projekte können optional dynamische Felder haben.
Wenn Sie bestimmte Informationen zum Projekt hinterlegen wollen, die nicht in den Standardfeldern abgebildet sind, dann können Sie das mit dynamischen Felder machen.
Dynamische Felder bestehen immer aus einem sogenannten "Key-Value" Paar. 
Wobei der "Key" der Bezeichner ist und der "Value" der Inhalt.

Die dynamischen Felder aus dem Projekt werden automatisch in Ausgangsrechnungen übernommen und tauchen auf den Ausgangsrechnungen rechts oben auf.
Wenn Ihr Kunde neben Projektnummer und Bestellnummer weitere Nummern auf der Rechnung sehen möchte, z.B. eine ganz bestimmte SAP Nummer, dann können Sie das mit dynamischen Feldern realisieren.

Die dynamischen Felder werden **nicht** auf Gutschriften übernommen.
Die dynamischen Felder werden ausschließlich auf Ausgangsrechnungen übernommen!

Dynamische Felder sind nicht sichtbar für die Projekt-Mitglieder und Projekt-Genehmiger.
Diese Felder sind nur für Personen sichtbar, die Leserechte auf Projekte und das Rechnungsmodul der Organisation haben.

Dynamische Felder können jederzeit hinzugefügt, geändert oder gelöscht werden.

### Kommentare Zeiterfassung verpflichtend

Projekte können optional so konfiguriert werden, dass bei der Zeiterfassung ein Kommentar verpflichtend ist.
Dies ist auch die Standardeinstellung.

### Abrechenbar

Projekte können so konfiguriert werden, dass sie abrechenbar sind.
Das bedeutet, dass auf das Projekt gebuchte Zeiten, Ausgaben und Festpreis-Pakete auch abgerechnet werden können.
Wenn ein Projekt nicht abrechenbar ist, dann können auf das Projekt gebuchte Zeiten, Ausgaben und Festpreis-Pakete nicht abgerechnet werden.
Projekte, die nicht abrechenbar sind, tauchen auch nicht im Rechnungsmodul auf.

Die Standardeinstellung ist, dass Projekte abrechenbar sind.
