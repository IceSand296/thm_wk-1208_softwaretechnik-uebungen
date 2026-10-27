# Anforderung oder Lösung? — Terminplaner für die THM

Kürzel: janp

## Funktionale Anforderung (FA)

- Studierende können einen freien Sprechstundentermin bei einer Lehrperson buchen.
- Die Anmeldung erfolgt ausschließlich über das Hochschulkonto.
- Vor jeder Buchung fragt die Komponente „Buchung“ bei der Komponente „Kalender“ an, ob der Termin noch frei ist.
- Ein bereits gebuchter Termin kann kein zweites Mal gebucht werden.
- Über die API kann ein KI-Agent freie Termine abfragen und im Namen einer Person buchen.
- Ein Sekretariat sieht alle Prüfungstermine seines Fachbereichs auf einen Blick.
- Sagt eine Lehrperson eine Sprechstunde ab, erhalten alle, die gebucht haben, eine Nachricht.
- Eine Buchung ist für Studierende in höchstens drei Schritten abgeschlossen.

## Qualitätsanforderung (QA)

- Auch zu Beginn der Prüfungsanmeldung, wenn bis zu 2.000 Personen zugleich buchen, zeigt das System eine Seite in weniger als zwei Sekunden an.

## Randbedingung (RB)

- Die Buchungsseite ist mit einem Screenreader vollständig bedienbar.
- Personenbezogene Daten werden nach den Vorgaben der EU-DSGVO verarbeitet.

## Keine Anforderung — Lösung (WIE)

- Die erste Ausbaustufe geht zum Sommersemester 2027 in Betrieb.
- Das System wird im Rechenzentrum der THM betrieben.
- Die API nimmt Anfragen als REST-Aufrufe entgegen und antwortet in JSON.
- Jeder gebuchte Termin lässt sich als iCal-Datei herunterladen.
- Termine werden in einer PostgreSQL-Datenbank gespeichert.

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

Keine Karte markiert.

<!-- zuordnung ue03-anforderung-oder-loesung: k01=fa k02=wie k03=fa k04=fa k05=fa k06=wie k07=fa k08=fa k09=rb k10=qa k11=wie k12=wie k13=rb k14=fa k15=wie k16=fa | unsicher: – -->
