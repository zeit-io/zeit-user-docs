# Projekte

Projekte sind ein zentraler Bestandteil von ZEIT.IO!
Jedes Projekt hat eine eindeutige Kennung, einen Namen, ein Start- und Enddatum, ein Stunden-Budget und ein Währungs-Budget.
Zeiten (TimeRecords), Ausgaben und Festpreis-Pakete können auf Projekte gebucht werden.
Projekte, die einer Organisation angehören, können von mehreren Personen bearbeitet werden.
Jedes Projekt hat eine Mitgliederliste, in der alle Personen aufgeführt sind, die auf das Projekt buchen dürfen.
Außerdem hat jedes Projekt auch eine Genehmigungsliste, in der alle Personen aufgeführt sind, die Buchungen auf dem Projekt genehmigen dürfen.

Wenn Sie im Kontext der Organisation sind, dann finden Sie im Hauptmenü den Punkt "Projekte".
Hier können Sie alle Projekte ansehen, die zur Organisation gehören.
Und Sie können auch neue Projekte erstellen.

## Name vs. Kennung

Jedes Projekt hat einen Namen und eine Kennung. Diese sind standardmäßig identisch, können aber auch unterschiedlich sein.
Der Name des Projektes ist relevant für das Rechnungsmodul.
Der Name wird auf Rechnungen und Gutschriften verwendet.
Setzen Sie den Projektnamen entsprechend so, wie sie das Projekt auf Ausgangsrechnungen und Gutschriften repräsentiert sehen wollen.

Die Projekt-Kennung muss eindeutig innerhalb der Organisation sein und wird innerhalb der Anwendung verwendet
um das Projekt anzuzeigen. So wird z.B. in der Projektauswahl für die Zeiterfassung immer die Projekt-Kennung angezeigt.
Und auch bei der Erfassung von Ausgaben wird bei der Projektauswahl immer die Projekt-Kennung angezeigt. Nicht der Name!

Sowohl Name als auch Kennung können jederzeit geändert werden.

## Projekt-Beschreibung

Jedes Projekt kann eine Beschreibung haben. Die Beschreibung ist optional und kann jederzeit geändert werden.
Die Beschreibung ist sichtbar für die Projekt-Mitglieder und Projekt-Genehmiger und kann verwendet werden, um zusätzliche Informationen zum Projekt bereitzustellen.

## Projektzeitraum

Jedes Projekt hat ein Start- und Ende-Datum.
Alle Buchungen (Zeiten, Ausgaben, Festpreis-Pakete) müssen innerhalb des Projekt-Zeitraums liegen.
Buchungen, die außerhalb des Projekt-Zeitraums liegen, können nicht auf das Projekt gebucht werden.
Start- und Ende-Date können jederzeit geändert werden.

## Budgets

Ein Projekt hat immer ein Stunden-Budget und ein Gesamt-Währungs-Budget.
Das Stundenbudget ist die Anzahl der Stunden, die maximal auf das Projekt gebucht werden dürfen.
Das Gesamt-Währungs-Budget ist der Betrag, der für das Projekt zur Verfügung steht.
Das Gesamt-Währungs-Budget ist die Summe der folgenden drei Budgets:

- **Budget (Zeiterfassung)**: Das Währungs-Budget für die Zeiterfassung.
- **Budget (Ausgaben)**: Das Währungs-Budget für die Ausgaben.
- **Budget (Festpreis-Pakete)**: Das Währungs-Budget für die Festpreis-Pakete.

Standardmäßig stellt ZEIT.IO auch sicher, dass diese Budgets nicht überschritten werden.
Es sei denn die Option für "Überbuchungen erlauben" ist aktiviert.
In dem Fall können die Budgets auch überschritten werden.

## Projektnummer & Bestellnummer

Projekte können optional eine Projektnummer und eine Bestellnummer haben.
In den Orga-Einstellungen kann konfiguriert werden, ob diese Felder Pflichtfelder sein sollen oder nicht.
Standardmäßig sind diese Felder keine Pflichtfelder.

Wenn eine Projektnummer oder Bestellnummer hinterlegt ist, dann wird diese auch auf Ausgangsrechnungen und Gutschriften verwendet.
Ausserdem können dann die folgenden Elemente ebenfalls nach Projektnummer und/oder Bestellnummer gefiltert werden:

- Zeiten (TimeRecords)
- Ausgaben/Reisekosten
- Leistungsnachweise (Timesheets)
- Ausgangsrechnungen
- Eingangsrechnungen
- Gutschriften

## Intervall

Mit dem Intervall im Projekt kann konfiguriert werden, wie feingranular die Zeiterfassung sein soll.
Standardmäßig ist die Zeiterfassung im Projekt minuten-genau.
Es können aber auch verschiedene Intervalle konfiguriert werden, wie z.B. 5 Minuten, 10 Minuten, 15 Minuten oder 30 Minuten.
In diesem Fall wird die Zeiterfassung immer auf das nächste Intervall gerundet.
So dass alle gebuchten Zeiten glatt durch ein Intervall teilbar sind.

Wenn z.B. ein 10 Minuten Intervall konfiguriert ist, dann wird eine Zeit von 12 Minuten auf 20 Minuten aufgerundet.
Jedes angefangene Intervall wird somit immer voll abgerechnet.

## Kunde

Jedes Projekt kann optional einem Kunden zugeordnet werden.
Im Dropdown für die Kundenauswahl tauchen nicht nur die Kunden auf, sondern auch die hinterlegten Abteilungen und Ansprechpartner der Kunden.
Im Idealfall weisen Sie das Projekt gleich der richtigen Abteilung, bzw. Ansprechpartner zu, die für den Rechnungsempfang zuständig ist.

Wenn Projektzeiten oder Ausgaben abgerechnet werden, dann ist das Rechnungsmodul mit dem Kunden vorbelegt, der dem Projekt zugeordnet ist.

Außerdem können Projekte, Zeiten, Ausgaben und Leistungsnachweise dann auch nach Kunden gefiltert werden.

## Ansprechpartner

Jedes Projekt kann optional einen Ansprechpartner haben.
Der Ansprechpartner ist sichtbar für alle Projektmitglieder und Projekt-Genehmiger.
Der Ansprechpartner kann verwendet werden, um eine Kontaktperson für das Projekt zu hinterlegen.

## Dynamische Felder

Projekte können optional dynamische Felder haben.
Wenn Sie bestimmte Informationen zum Projekt hinterlegen wollen, die nicht in den Standardfeldern abgebildet sind, dann können Sie das mit dynamischen Felder machen.
Dynamische Felder bestehen immer aus einem Key-Value Paar. Der ist der Bezeichner und der Wert ist der Inhalt.

Die dynamischen Felder aus dem Projekt werden automatisch in Ausgangsrechnungen übernommen und tauchen auf den Ausgangsrechnungen rechts oben auf.
Wenn Ihr Kunde neben Projektnummer und Bestellnummer weitere Nummern auf der Rechnung sehen möchte, z.B. eine ganz bestimmte SAP Nummer, dann können Sie das mit dynamischen Feldern realisieren.

Die dynamischen Felder werden **nicht** auf Gutschriften übernommen.
Die dynamischen Felder werden ausschließlich auf Ausgangsrechnungen übernommen!

Dynamische Felder sind nicht sichtbar für die Projekt-Mitglieder und Projekt-Genehmiger.
Diese Felder sind nur für Personen sichtbar, die Leserechte auf Projekte und das Rechnungsmodul der Organisation haben.

Dynamische Felder können jederzeit hinzugefügt, geändert oder gelöscht werden.

## Kommentare Zeiterfassung verpflichtend

Projekte können optional so konfiguriert werden, dass bei der Zeiterfassung ein Kommentar verpflichtend ist.
Dies ist auch die Standardeinstellung.

## Abrechenbar

Projekte können so konfiguriert werden, dass sie abrechenbar sind.
Das bedeutet, dass auf das Projekt gebuchte Zeiten, Ausgaben und Festpreis-Pakete auch abgerechnet werden können.
Wenn ein Projekt nicht abrechenbar ist, dann können auf das Projekt gebuchte Zeiten, Ausgaben und Festpreis-Pakete nicht abgerechnet werden.
Projekte, die nicht abrechenbar sind, tauchen auch nicht im Rechnungsmodul auf.

Die Standardeinstellung ist, dass Projekte abrechenbar sind.
