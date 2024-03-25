# Zeiterfassung

Die Zeiterfassung ist eine elementare Funktion in ZEIT.IO. Es gibt verschiedene Möglichkeiten,
wie Sie Ihre Arbeitszeiten und Projektzeiten erfassen können:

- **Timer**: Erfassen Sie Ihre Zeiten mit dem Timer mit Start-, Stopp- und Pausenzeiten.
- **Kalender**: Erfassen Sie Ihre Zeiten im Kalender mit "Drag and Drop".
- **Import**: Importieren Sie Ihre Zeiten aus einem anderen System.

Außerdem gibt es verschiedene Clients, mit denen Sie Ihre Zeiten erfassen können:

- **WebApp**: Erfassen Sie Ihre Zeiten im Webbrowser auf der [ZEIT.IO Seite](https://zeit.io/de/).
- **Browser-Extension**: Erfassen Sie Ihre Zeiten im Browser über die ZEIT.IO Browser-Extension, unabhängig
  von der ZEIT.IO Seite.
- **Mobile**: Erfassen Sie Ihre Zeiten auf dem Smartphone.

## Timer

Am einfachsten ist die Erfassung über den Timer. Der Timer
befindet sich im Login-Bereich immer links oben. Unabhängig vom Kontext in dem Sie sich befinden
ist der Timer immer an der gleichen Stelle. Hier sind die Funktionen des Timers grafisch dargestellt:

![Timer auf ZEIT.IO](../img/timer-functions.png)

Sie können jederzeit den Timer starten, pausieren, fortsetzen und stoppen. Wenn Sie auf das Stopp-Symbol klicken,
dann öffnet sich ein modaler Dialog, in dem Sie die Buchung abschließen können. Erst am Ende der Buchung müssen Sie
sich entscheiden, auf welches Projekt Sie die Zeit buchen wollen. Das ist ein großer Vorteil, weil Sie sich nicht
vorher festlegen müssen. Sie können den Timer starten und dann später entscheiden, auf welches Projekt Sie die Zeit buchen.

Hier ein Beispiel für das modale Dialogfenster, das sich öffnet, wenn Sie den Timer stoppen:

![Timer-Modal](../img/context-employee/timetracking-01-de.png)

Bis auf "Dauer" sind alle Eingabefelder im modalen Dialog editierbar. Das bedeutet, dass Sie vor der Speicherung
noch Anpassungen vornehmen können. Wenn Sie vergessen haben eine Pause zu tracken, dann können Sie die Pausenzeit hier
problemlos nachtragen. Auch die Von-Bis-Zeiten können Sie nochmal anpassen.

In der unteren Zeile haben Sie verschiedene Schaltflächen. Hier sind deren Funktionen erklärt:

- **Speichern & Schließen**: Wenn Sie auf "Speichern & Schließen" klicken, dann wird die Zeit gebucht, der Timer zurückgesetzt auf 00:00:00
  und der modale Dialog wieder geschlossen.
- **Speichern & Starten**: Wenn Sie auf "Speichern & Schließen" klicken, dann wird die Zeit gebucht, der Timer zurückgesetzt auf 00:00:00, der modale Dialog geschlossen und der Timer gestartet.
- **Speichern & Neu**: Wenn Sie auf "Speichern & Neu" klicken, dann wird die Zeit gebucht, der Timer zurückgesetzt auf 00:00:00
  und der modale Dialog bleibt geöffnet, damit Sie gleich die nächste Buchung erfassen können.
- **Zeit verwerfen**: Wenn Sie auf "Zeit verwerfen" klicken, dann wird der Timer ohne etwas zu speichern auf 00:00:00 zurückgesetzt.

### Tastenkürzel für den Timer

Den Timer können Sie auch über die Tastatur steuern. Das funktioniert mit diesen Tastenkürzeln:

- **Starten**: `s`
- **Pausieren**: `p`
- **Fortsetzen**: `s`
- **Stoppen**: `e`

Das Formular im modalen Dialog kann mit der Tastenkombination `Strg + Enter` (`Command + Enter` auf Mac)
abgeschickt werden. Damit lassen sich Zeiten sehr schnell erfassen, auch ohne Maus.


### Zeiten nacherfassen mit dem Timer

Sie können auch Zeiten nacherfassen, die Sie zuvor vergessen haben. Dafür müssen Sie den Timer nicht extra starten.
Wenn dieser nicht läuft, also auf `00:00:00` steht, können Sie trotzdem auf das Stopp-Symbol klicken.
Dadurch öffnet sich das modale Dialogfenster und Sie können die Zeiten nacherfassen. Im linken oberen Bereich des
modalen Dialogfensters können Sie auch das Datum auswählen, für das Sie die Zeiten nacherfassen wollen.

Wenn Sie gleich mehrere Buchungen nacherfassen wollen, dann nutzen Sie gerne die "Speichern & Neu"-Schältfläche. Damit wird
die aktuelle Buchung gespeichert und das modale Dialogfenster bleibt geöffnet, damit Sie gleich die nächste Buchung
erfassen können.

### Zeiten nacherfassen mit dem Timer, wenn dieser schon läuft

Wenn der Timer schon läuft und Sie Zeiten mit Start- und Stoppzeit nacherfassen wollen, ohne den laufenden Timer
zu stoppen, dann können Sie dafür das vierte Symbol in der Reihe verwenden, das schwarze Viereck im Kreis.
Damit öffnet sich der modale Dialog für die Zeiterfassung und Sie können Zeiten mit Start- und Stoppzeiten nacherfassen. 
Nach dem Speichern läuft der Timer weiter.

### Zeiten für andere Personen mit erfassen

Oft kommt es vor, dass man zu zweit mit einem Kunden im Meeting ist. Wenn beide Personen den Timer laufen lassen,
kann es passieren, dass die beiden Buchungen leicht unterschiedliche Start- und Stoppzeiten haben. Auf
einem Leistungsnachweis, den später der Kunde bekommt, ist das nicht so schön.

In dem Fall ist es sinnvoll, wenn nur eine Person den Timer laufen lässt und die Zeiten für beide Personen erfasst, 
so dass beide Buchungen die gleichen Start- und Stoppzeiten haben.

Wenn Sie im modalen Dialog für die Zeiterfassung ein Projekt auswählen, welches mehrere aktive Mitglieder hat,
dann erscheint ein weiteres Eingabefeld für die Teilnehmer. Hier können Sie dann die Teilnehmer auswählen, für die
Sie die Zeit mit erfassen wollen. Das Autocomplete schlägt die Benutzernamen der aktiven Mitglieder vor. 
Sie können hier auch mehrere Teilnehmer hinzufügen. Hier ein Beispiel, bei dem Max Mustermann hinzugefügt wurde.

![Teilnehmer hinzufügen](../img/context-employee/participants-01-de.png)

Wenn Sie jetzt die Zeit buchen, dann wird sie für beide Personen erfasst. Es werden  zwei Buchungen
erstellt, eine für Sie und eine für Max Mustermann. Beide Buchungen haben dabei den exakt gleichen Inhalt.
Auf einem Leistungsnachweis sieht es dann sehr professionell aus, wenn die Zeiten der Meeting-Teilnehmer
alle die gleichen Start- und Stoppzeiten haben.

## FAQs

### Wieso sind Buchungen nach einer bestimmten Zeit nicht mehr bearbeitbar? 

In ZEIT.IO haben alle Buchungen von Mitarbeitern eine sogenannte "Freeze Time". Das bedeutet, dass Buchungen 
nach einer bestimmten Zeit nicht mehr bearbeitbar sind. Die "Freeze Time" ist standardmäßig auf 30 Tage eingestellt, 
und dient zum Schutz des Arbeitgebers. Für Controlling-Zwecke und für die Abrechnung ist es wichtig, dass Buchungen
nicht mehr verändert werden können.

Die "Freeze Time" kann pro Vertrag konfiguriert werden, so kann jeder Mitarbeiter eine andere "Freeze Time" haben.
Wenn Sie Buchungen nach einer bestimmten Zeit bearbeiten wollen, dann wenden Sie sich bitte an Ihren Vorgesetzten
oder an die Personalabteilung. Diese können die "Freeze Time" für Ihren Vertrag anpassen.
