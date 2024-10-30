# Rechnungsausgang

Im Rechnungsausgang können Sie Ihre Rechnungen erstellen und versenden.
Dafür klicken Sie im Hauptmenü auf "Rechnungen" und dann auf "Rechnungsausgang".
Dort sehen Sie eine Liste aller Rechnungen, die bereits erstellt wurden.
Neue Rechnungen können entweder manuell erstellt werden, mit dem grünen Button "Neue Rechnung erstellen",
oder automatisch über das [Auto-Ausgangsrechnungen Feature](/organisationen/auto-invoicing/).

## Anhänge  

Wenn Sie eine Rechnung erstellen, können Sie auch Anhänge hinzufügen. Sie können mehrere PDF-Dateien hochladen 
und diese werden dann mit der erstellten Rechnungs-PDF zusammengefügt. Somit erhalten Sie eine PDF-Rechnung mit
allen notwendigen Anhängen, in einer einzelnen Datei.

## Leistungsnachweise 

Wenn mir der Rechnung Projektzeiten abgerechnet werden, dann kann optional ein Leistungsnachweis ausgewählt werden, 
welcher die abgerechneten Zeiten enthält. Der Leistungsnachweis wird dann als Anhang zur Rechnung hinzugefügt.
Für diesen Leistungsnachweis-Anhang gibt es verschieden Formate, die Sie auswählen können:

### Kein Leistungsnachweis

Bei dieser Option wird kein Leistungsnachweis zur Rechnung hinzugefügt.

### Timesheet PDF Anhang 

Wenn die Rechnung vom Type "Timesheet" (Leistungsnachweis) ist, und das Timesheet einen PDF-Anhang hat, 
dann wird die PDF aus dem Timesheet an die Rechnung angehängt. Diese Option macht vor allem Sinn, für 
externe Leistungsnachweise, die nicht in ZEIT.IO erstellt wurden. Lesen hierzu auch
- [Externen Leistungsnachweis genehmigen lassen](/freiberufler/leistungsnachweise/#externen-leistungsnachweis-genehmigen-lassen).

### ZEIT.IO Leistungsnachweis (Gruppiert bei Benutzer)

Der Standard-ZEIT.IO-Leistungsnachweis wird an die Rechnung angehängt. Dieser enthält eine Tabelle mit allen genehmigten TimeRecords für den ausgewählten Zeitraum. 
Die Einträge beinhalten: 

- Datum 
- Start- & Stopzeiten 
- Projekt/Aktivität 
- Kommentar 
- Name des Experten/Benutzers
- Dauer der Buchung.

Die TimeRecords sind gruppiert nach Experten/Benutzer. 
Die Leistungsnachweise der einzelnen Benutzer sind getrennt durch Seitenumbruch.

### ZEIT.IO Leistungsnachweis (Gruppiert bei Aktivität)

Wenn Aktivitäten vorhanden sind, dann wird als aller erstes eine Tabelle eingeblendet, bei der die gebuchten Zeiten nach Aktivitäten gruppiert sind. 
Anschließend wird eine Tabelle mit allen genehmigten TimeRecords für den ausgewählten Zeitraum gerenderd. 
Die Einträge beinhalten Datum, Start- & Stopzeiten, Projekt/Aktivität, Name des Experten/Benutzers, sowie Kommentar und Dauer der Buchung.

### Conti Leistungsnachweis 

Es wird der Conti-Leistungsnachweis an die Rechnung angehängt. 
Dieser Leistungsnachweis entspricht den Vorgaben von Continental Automotive. 
Als Messeinheit werden DevUnits verwendet. 1 DevUnit = 1 Std. Die DevUnits sind gruppiert nach Aktivitäten.

### Dacuro Leistungsnachweis

Dieser Leistungsnachweis enthält eine Tabelle mit allen genehmigten TimeRecords für den ausgewählten Zeitraum. 
Die Einträge beinhalten Datum, Projekt/Aktivität, Kommentar und Dauer der Buchung. 
Nicht enthalten sind Start- Stoppzeiten und die Namen der Experten/Benutzer. 
Wenn Aktivitäten vorhanden sind, dann wird als aller erstes eine Tabelle eingeblendet, bei der die gebuchten Zeiten nach Aktivitäten gruppiert sind.
Da dieser Leistungsnachweis weder Start- noch Stoppzeiten enthält, können Einträge mit gleichem Datum und gleichem Kommentar verwirrend sein.
Deshalb werden Einträge mit gleichem Datum und gleichem Kommentar zusammengefasst und die Dauer addiert.

## CSV Export

Unterhalb der Tabelle auf der rechten Seite gibt es einen Link "CSV Export".
Mit diesem Link können Sie die aktuelle Tabelle für die Ausgangsrechnungen als CSV Datei herunterladen.
Jede Ausgangsrechnung wird als eine Zeile in der CSV Datei dargestellt.

Die Ausgangsrechnungen können nach verschiedenen Kriterien gefiltert werden.
Die CSV Datei enthält die Ergebnismenge der aktuellen Filtereinstellungen.

## DATEV CSV Export

Wenn Sie die Ausgangsrechnungen nach einem Leistungs-Monat oder Jahr filtern, dann erscheint unterhalb der Tabelle, auf der rechten Seite, ein zusätzlicher Link "DATEV CSV Export".
Mit diesem Link können Sie die aktuelle Tabelle für die Ausgangsrechnungen als DATEV CSV Datei herunterladen.
Die DATEV CSV Datei enthält alle Ausgangsrechnungen, die in dem gewählten Leistungs-Monat oder Jahr erstellt wurden.
Jede einzelne Position auf der Ausgangsrechnung wird als eine Zeile in der CSV Datei dargestellt.
Deshalb kann die Datei auch mehr Zeilen enthalten als die Tabelle auf der Webseite.

Die Datei entspricht dem [DATEV Buchungsstapel Format](https://developer.datev.de/datev/platform/de/dtvf/formate/buchungsstapel) und enthält alle notwendigen Informationen für die Buchhaltung.
Die DATEV CSV Datei kann dann in Ihre Buchhaltungssoftware importiert werden.
