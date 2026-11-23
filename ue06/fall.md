# Der Fall — Terminplaner für die THM

<!-- Die vier Beschreibungen der Übung 6, gleichlautend mit dem Übungsblatt.
     Diese Datei bleibt unverändert; Sie und Ihr Agent lesen sie nur. -->

Lehrende bieten Sprechstunden an, Studierende buchen sie, und die
Sekretariate behalten den Überblick. Nach diesen Beschreibungen modellieren
Sie in den Aufgaben 1 bis 4.

## Beschreibung 1 — Was der Terminplaner leistet

Lehrende bieten im Terminplaner Sprechstunden an. Eine Sprechstunde legen
sie mit Datum, Beginn, Ende und Ort an; der Terminplaner teilt sie dabei in
Zeitfenster zu 15 Minuten. Studierende buchen ein freies Zeitfenster und
können ihre Buchung wieder stornieren. Ist eine Sprechstunde ausgebucht,
können sie sich beim Buchen auf eine Warteliste setzen lassen. Lehrende
können eine Sprechstunde absagen; der Terminplaner benachrichtigt dann alle,
die ein Zeitfenster gebucht haben. Storniert jemand eine Buchung,
benachrichtigt er die Lehrperson. Wer bucht, storniert, anlegt oder absagt,
meldet sich zuvor mit dem Hochschulkonto an; ob die Anmeldung gilt, prüft
der Anmeldedienst des Rechenzentrums. Sekretariate legen Sprechstunden für
die Lehrenden an, welche sie betreuen. Jede Buchung lässt sich als
iCal-Datei herunterladen.

## Beschreibung 2 — Ein Zeitfenster buchen

Die Studentin wählt eine Sprechstunde aus. Ist sie noch nicht angemeldet,
meldet sie sich zuerst mit ihrem Hochschulkonto an. Der Terminplaner zeigt
ihr die freien Zeitfenster der Sprechstunde; sie wählt eines aus und trägt
ihr Anliegen ein. Der Terminplaner prüft, ob das Zeitfenster noch frei ist,
denn andere buchen zur selben Zeit. Ist es inzwischen vergeben, zeigt er ihr
erneut die freien Zeitfenster. Ist es frei, trägt er die Buchung ein. Danach
geschieht dreierlei zugleich: Der Terminplaner schickt der Studentin eine
Bestätigung mit iCal-Datei, benachrichtigt die Lehrperson und vermerkt das
Zeitfenster als gebucht. Sind alle drei erledigt, ist die Buchung
abgeschlossen.

## Beschreibung 3 — Die Daten des Terminplaners

Jede Person im Terminplaner hat ein Hochschulkonto mit Kennung und Namen.
Lehrende führen zusätzlich einen Titel, Studierende einen Studiengang. Eine
Lehrperson bietet beliebig viele Sprechstunden an; jede Sprechstunde gehört
zu genau einer Lehrperson. Eine Sprechstunde hat ein Datum, einen Beginn,
ein Ende und einen Ort und besteht aus mindestens einem Zeitfenster. Ein
Zeitfenster gehört zu genau einer Sprechstunde und wird mit ihr gelöscht.
Für jedes Zeitfenster gibt es höchstens eine Buchung. Eine Buchung nennt die
Studentin oder den Studenten, welche gebucht haben, den Zeitpunkt der
Buchung und das Anliegen. Ein Sekretariat hat eine Bezeichnung und einen
Raum und betreut mehrere Lehrende; jede Lehrperson wird von höchstens einem
Sekretariat betreut.

## Beschreibung 4 — Die Zustände eines Zeitfensters

Ein Zeitfenster ist nach dem Anlegen frei. Bucht jemand, ist es gebucht;
wird die Buchung storniert, ist es wieder frei. Stornieren lässt sich nur
bis zwei Stunden vor Beginn. Lehrende können ein freies Zeitfenster sperren
und wieder freigeben. Solange ein Zeitfenster angeboten wird, d.h. frei,
gebucht oder gesperrt ist, kann die Lehrperson die ganze Sprechstunde
absagen; das Zeitfenster ist dann abgesagt. Ist der Beginn erreicht, gilt
ein gebuchtes Zeitfenster als wahrgenommen, ein freies oder gesperrtes
verfällt. Abgesagte, wahrgenommene und verfallene Zeitfenster ändern sich
nicht mehr.
