# Zeiterfassung

Die Zeiterfassung ist eine elementare Funktion in ZEIT.IO. Es gibt verschiedene Möglichkeiten,
wie Sie Ihre Arbeitszeiten und Projektzeiten erfassen können:

- **Timer**: Erfassen Sie Ihre Zeiten mit dem Timer, mit Start-, Stop- und Pausenzeiten.
- **Kalender**: Erfassen Sie Ihre Zeiten im Kalender, mit "Drag and Drop".
- **Import**: Importieren Sie Ihre Zeiten aus einem anderen System.

Außerdem gibt es verschiedene Clients, mit denen Sie Ihre Zeiten erfassen können:

- **WebApp**: Erfassen Sie Ihre Zeiten im Webbrowser auf der [ZEIT.IO Seite](https://zeit.io/de/).
- **Browser-Extension**: Erfassen Sie Ihre Zeiten im Browser, über die ZEIT.IO Browser-Extension, unabhängig
  von der ZEIT.IO Seite.
- **Mobile**: Erfassen Sie Ihre Zeiten auf dem Smartphone.

## Timer

Am einfachsten ist die Erfassung über den Timer. Der Timer
befindet sich, im Login-Bereich, immer links oben. Unabhängig vom Kontext, in dem Sie sich befinden,
ist der Timer immer an der gleichen Stelle. Hier sind die Funktionen des Timers grafisch dargestellt.

![Timer auf ZEIT.IO](../img/timer-functions.png)

Sie können jederzeit den Timer starten, pausieren, fortsetzen und stoppen. Wenn Sie auf das Stop-Symbol klicken,
dann öffnet sich ein modaler Dialog, in dem Sie die Buchung abschließen können. Erst am Ende der Buchung müssen Sie
sich entscheiden, auf welches Projekt Sie die Zeit buchen wollen. Das ist ein großer Vorteil, weil Sie sich nicht
vorher festlegen müssen. Sie können den Timer starten und dann später entscheiden, auf welches Projekt Sie die Zeit buchen.

Hier ein Beispiel für das modale Dialogfenster, das sich öffnet, wenn Sie den Timer stoppen:

![Timer-Modal](../img/context-employee/timetracking-01-de.png)

Bis auf "Dauer", sind alle Eingabefelder im modalen Dialog editierbar. Das bedeutet dass Sie, vor der Speicherung,
noch Anpassungen vornehmen können. Wenn Sie vergessen haben eine Pause zu tracken, dann können Sie die Pausenzeit hier
nachtragen. Das ist kein Problem. Sie können auch die Von- Bis-Zeiten nochmal anpassen.

Inter unteren Zeile haben Sie verschiedene Buttons. Hier sind die Funktionen der Buttons erklärt:

- **Speichern & Schließen**: Wenn Sie auf "Speichern & Schließen" klicken, dann wird die Zeit gebucht, der Timer wird zurückgesetzt auf 00:00:00
  und das modale Dialog wird wieder geschlossen.
- **Speichern & Starten**: Wenn Sie auf "Speichern & Schließen" klicken, dann wird die Zeit gebucht, der Timer wird zurückgesetzt auf 00:00:00, das modale Dialog wird geschlossen und der Timer wird gestartet.
- **Speichern & Neu**: Wenn Sie auf "Speichern & Neu" klicken, dann wird die Zeit gebucht, der Timer wird zurückgesetzt auf 00:00:00
  und das modale Dialog bleibt geöffnet, damit Sie gleich die nächste Buchung erfassen können.
- **Zeit verwerfen**: Wenn Sie auf "Zeit verwerfen" klicken, dann wird der Timer zurückgesetzt auf 00:00:00, ohne etwas zu speichern.

### Tastenkürzel für den Timer

Den Timer können Sie auch über die Tastatur steuern. Das funktioniert mit diesen Tastenkürzeln:

- **Starten**: `s`
- **Pausieren**: `p`
- **Fortsetzen**: `s`
- **Stoppen**: `e`

Das Formular im modalen Dialog kann mit der Tastenkombination `Strg + Enter` (`Command + Enter` auf Mac)
abgeschickt werden. Damit lassen sich Zeiten sehr schnell erfassen, auch ohne Maus.


### Zeiten nacherfassen mit dem Timer

Sie können auch Zeiten nacherfassen, die Sie vergessen haben zu erfassen. Dafür müssen Sie den Timer nicht extra starten.
Wenn der Timer nicht läuft, also auf `00:00:00` steht, dann können Sie trotzdem auf das Stopp-Symbol klicken.
Dadurch öffnet sich das modale Dialogfenster und Sie können die Zeiten nacherfassen. Im linken oberen Bereich des
modalen Dialogfensters, können Sie auch das Datum auswählen, für das Sie die Zeiten nacherfassen wollen.

Wenn Sie gleich mehrere Buchungen nacherfassen wollen, dann nutzen Sie gerne den "Speichern & Neu" Button. Damit wird
die aktuelle Buchung gespeichert und das modalen Dialogfenster bleibt geöffnet, damit Sie gleich die nächste Buchung
erfassen können.

### Zeiten nacherfassen mit dem Timer, wenn der Timer schon läuft

Wenn der Timer schon läuft und sie Zeiten mit Start- und Stoppzeit nacherfassen wollen, ohne den laufenden Timer
zu stoppen, dann können Sie dafür das vierte Symbol in der Reihe verwenden. Das schwarze Viereck im Kreis.
Damit öffnet sich der modale Dialog für die Zeiterfassung und Sie können Zeiten nacherfassen,
mit Start- und Stoppzeiten. Nach dem Speichern läuft der Timer weiter.

### Zeiten für andere Personen mit erfassen

Oft kommt es vor, das man zu zweit mit einem Kunden im Meeting ist. Wenn beide Personen den Timer laufen lassen, 
dann kommt kommt es oft vor, das die zwei Buchungen leicht unterschiedliche Start- und Stoppzeiten haben. Auf 
einem Leistungsnachweis, den später der Kunde bekommt, ist das nicht so schön. 

In dem Fall ist es sinnvoll, wenn nur eine Person den Timer laufen lässt und die Zeiten für beide Personen erfasst. 
Damit beiden Buchungen die gleichen Start- und Stoppzeiten haben. 

Wenn Sie im modalen Dialog für die Zeiterfassung, ein Projekt auswählen, welches mehrere aktive Mitglieder hat, 
dann erscheint ein weiteres Eingabefeld für die Teilnehmer. Hier können Sie dann die Teilnehmer auswählen, für die
Sie die Zeit mit erfassen wollen. Sie können hier auch mehrere Teilnehmer hinzufügen. Hier ein Beispiel, 
bei dem Max Mustermann hinzugefügt wurde. 

![Teilnehmer hinzufügen](../img/context-employee/participants-01-de.png)

Wenn Sie jetzt die Zeit buchen, dann wird die Zeit für beide Personen erfasst. Es werden dann zwei Buchungen 
erstellt, eine für Sie und eine für Max Mustermann. Beide Buchungen haben dabei den exakt gleichen Inhalt. 
Auf einem Leistungsnachweis sieht es dann sehr professionell aus, wenn die Zeiten der Meeting-Teilnehmer 
alle die gleichen Start- und Stoppzeiten haben.

## FAQs

### Wieso sind Buchungen nach einer bestimmten Zeit nicht mehr bearbeitbar? 

In ZEIT.IO haben alle Buchungen von Mitarbeitern eine sogenannte "Freeze Time". Das bedeutet, dass Buchungen 
nach einer bestimmten Zeit nicht mehr bearbeitbar sind. Die "Freeze Time" ist standardmäßig auf 30 Tage eingestellt. 
Das bedeutet, dass Buchungen, die älter als 30 Tage sind, nicht mehr bearbeitet werden können. Dies dient 
zum Schutz des Arbeitgebers. Für Controlling-Zwecke und für die Abrechnung ist es wichtig, dass Buchungen
nicht mehr verändert werden können.

Die "Freeze Time" kann pro Vertrag konfiguriert werden. Somit kann jeder Mitarbeiter eine andere "Freeze Time" haben.
Wenn Sie Buchungen nach einer bestimmten Zeit bearbeiten wollen, dann wenden Sie sich bitte an Ihren Vorgesetzten
oder an die Personalabteilung. Diese können die "Freeze Time" für Ihren Vertrag anpassen.
