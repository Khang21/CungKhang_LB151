# Projekt-Dokumentation

✍️ Cung

| Datum     | Version | Zusammenfassung                                              |
| -----     | ------- | ------------------------------------------------------------ |
|09.12.2022 | 0.0.1   | Ich habe diesen Repository erstellt                          |
|28.12.2022 | 0.0.2   | Ich habe mit der Dokumentation angefangen.                   |



# 0 Ihr Projekt

In diesem Projekt werde ich das bekannte "Glücksrad" nachprogrammieren, dies war und ist noch einen der bekanntesten Spielshows in der USA und wird auch bald Adaptionen von mehrere anderen Länder haben.

# 1 Analyse

* Tier 1 (Presentation): Eine Website
* Tier 2 (Webserver): Daten aus einer Datenbank lesen und schreiben
* Tier 3 (Application Server): NaN
* Tier 4 (Dataserver): Vorinstallierte Wörterliste mit Kategorien + High Score des Spielers

# 2 Technologie

Ich werde für dieses Projekt HTML CSS JQUERY BOOTSTRAP anwenden:
Bootstrap ist ein beliebtes Front-End-Entwicklungsframework, das Entwicklern hilft, responsive, mobile-first Websites und Webanwendungen zu erstellen. Es umfasst eine Sammlung von CSS- und JavaScript-Komponenten wie Navigationsleisten, Schaltflächen, Formulare und Modals. jQuery ist eine JavaScript-Bibliothek, die die Arbeit mit HTML-Dokumenten, die Verarbeitung von Ereignissen, die Erstellung von Animationen und die Entwicklung leistungsstarker und interaktiver Front-End-Webanwendungen erleichtert. Bootstrap kann mit jQuery verwendet werden, um die Funktionalität von Webseiten zu verbessern und sie interaktiver zu gestalten. Zusammen können Bootstrap und jQuery Entwicklern helfen, schnell und einfach professionell aussehende und benutzerfreundliche Websites und Webanwendungen zu erstellen.


# 3 Datenbank

Ich werde MySQL anwenden:
MySQL ist ein beliebtes relationales Open-Source-Datenbankmanagementsystem. Es wird häufig für Webanwendungen und Data Warehousing verwendet. Es verwendet Structured Query Language (SQL) für die Verwaltung und Bearbeitung von in Tabellen gespeicherten Daten. MySQL ist bekannt für seine Schnelligkeit, Zuverlässigkeit und Benutzerfreundlichkeit.

# 4.1 User Stories

| US-№    | Verbindlichkeit | Typ        | Beschreibung                                                 |
| ----    | --------------- | ---------- | ----------------------------------                           |
| US-1 | Muss | Funktional |Als Administrator möchte ich mich durch die Eingabe von Benutzername und Passwort authentifizieren können, um auf die Administrationsfunktionen zugreifen zu können. |
| US-2 | Muss | Funktional |Als Administrator möchte ich Phrasen und Rätselwörter anlegen, ändern und löschen können, um die Rätselbank zu verwalten.|
| US-3 | Muss | Funktional |Als Administrator möchte ich Kategorien anlegen können, um die Rätsel und Phrasen zu organisieren und jedes Wort bzw. jede Frage einer Kategorie zuordnen zu können. |
| US-4 | Muss | Funktional |Als Administrator möchte ich einzelne Einträge der Highscore-Liste löschen können, um die Integrität und Richtigkeit der Liste zu gewährleisten. |
| US-5 | Muss | Funktional | Als Client möchte ich einen Webbrowser nutzen können, um das Spiel zu spielen. |
| US-6 | Muss | Funktional | Als Kandidat oder Kandidatin möchte ich meinen Namen eingeben können, der auf der Highscore-Liste erscheint. |
| US-7 | Muss | Funktional | Als Kandidat oder Kandidatin möchte ich jederzeit meinen Kontostand sehen können. |
| US-8 | Muss | Funktional | Als Kandidat oder Kandidatin möchte ich jederzeit meine Lebenspunkte sehen können. |
| US-9 | Muss | Funktional | Als Kandidat oder Kandidatin möchte ich erfahren ob die gewählte Antwort richtig oder falsch war. |
| US-10 | Muss | Funktional | Als Kandidat oder Kandidatin möchte ich in der Highscore-Liste Rang, Name des Spielers, Zeitpunkt des Spiels, Geldbetrag und Anzahl Spielrunden sehen können. |
| US-11 | Muss | Funktional | Als Kandidat oder Kandidatin möchte ich dass die Highscore-Liste nach Rang, der durch die Höhe des Geldbetrags bestimmt wird, aufsteigend sortiert ist. |
| US-12 | Muss | Funktional | Als Administrator möchte ich sicherstellen, dass kein Rätsel-Wort und keine Phrase einem Spieler mehr als einmal gestellt werden. |
| US-13 | Muss | Funktional | Als Kandidat möchte ich jederzeit die Möglichkeit haben entweder weiter zu spielen oder aufzuhören und meinen Gewinn in die Highscore-Liste übernehmen zu können. |
| US-14 | Muss | Funktional | Als Administrator möchte ich sicherstellen, dass das Spiel mit einer spielbaren Anzahl Wörtern und Fragen gefüllt ist. |
| US-15 | Muss | Funktional | Als Administrator möchte ich die Anzahl der Spielrunden zählen zu können. |
| US-16 | Muss | Rand | Als Entwickler möchte ich sicherstellen, dass einfache Formulareingaben auf Client- und Serverseite geprüft werden. |
| US-17 | Muss | Rand | Als Entwickler möchte ich die Wahl haben, welche Art von Datenbank verwendet wird. |
| US-18 | Muss | Rand | Als Entwickler möchte ich eine Datenbankanbindung verwenden, die möglichst unabhängig vom tatsächlich eingesetzten Produkt ist. |
| US-19 | Muss | Rand | Als Entwickler möchte ich Transaktionsmanagement einsetzen, um die Integrität der Daten sicherzustellen. |
| US-20 | Muss | Rand | Als Entwickler möchte ich Sicherheitsaspekte umsetzen, um die Daten und die Anwendung vor unbefugtem Zugriff zu schützen. |


# 4.2 Testfälle

| TC-№ | Vorbereitung | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1 | Erstellen Sie ein gültiges Konto mit dem Benutzernamen "admin" und dem Passwort "password" | Geben Sie "admin" als Benutzernamen und "password" als Passwort ein | Erfolgreiche Anmeldung und Zugriff auf die Administrationsfunktionen |
| 2.1 | Legen Sie eine Phrase oder ein Rätselwort an | Geben Sie "Welche Farbe hat eine Orange?" als Phrase ein, "Orange" als Antwort und "Früchte" als Kategorie | Erfolgreiche Anlage der Phrase oder des Rätselwortes |
| 3.1 | Legen Sie eine Kategorie an | Geben Sie "Früchte" als Kategorie | Erfolgreiche Anlage der Kategorie |
| 4.1 | Löschen Sie einen Eintrag aus der Highscore-Liste | Wählen Sie den Eintrag "Spieler1" aus der Highscore-Liste und klicken Sie auf "Löschen" | Erfolgreiche Löschung des Eintrags "Spieler1|
| 5.1 | Öffnen Sie die Anwendung im Webbrowser | N/A | Anzeige der Anwendung im Webbrowser |
| 6.1 | Der Kandidat oder die Kandidatin gibt einen Namen ein | Geben Sie "Max Mustermann" als Namen ein | Der Name "Max Mustermann" erscheint auf der Highscore-Liste |
| 7.1 | Der Kandidat oder die Kandidatin sieht den Kontostand | N/A | Anzeige des aktuellen Kontostands |
| 8.1 | Der Kandidat oder die Kandidatin sieht die Lebenspunkte | N/A | Anzeige der aktuellen Lebenspunkte |
| 9.1 | Der Kandidat oder die Kandidatin wählt eine Antwort | Wählen Sie die Antwort "Orange" für die Phrase "Welche Farbe hat eine Orange?" | Anzeige "richtig" oder "falsch" |
| 10.1 | In der Highscore-Liste werden Rang, Name des Spielers, Zeitpunkt des Spiels, Geldbetrag, Anzahl Spielrunden aufgeführt | N/A | Anzeige der Highscore-Liste mit Rang, Name des Spielers, Zeitpunkt des Spiels, Geldbetrag und Anzahl Spielrunden |
| 11.1 | Die Highscore-Liste wird nach Rang, der durch die Höhe des Geldbetrags bestimmt wird, aufsteigend sortiert | N/A | Anzeige der Highscore-Liste sortiert nach Rang, der durch die Höhe des Geldbetrags bestimmt wird, aufsteigend |
| 12.1 | Kein Rätsel-Wort und keine Phrase sollen einem Spieler mehr als einmal gestellt werden | N/A | Keine Wiederholung von Rätsel-Wörtern und Phrasen für einen Spieler |
| 13.1 | Der Kandidat kann jederzeit entweder spielen, oder aufhören und seinen Gewinn in die Higscore-Liste übernehmen | Wählen Sie "Aufhören" und "Gewinn in die Highscore-Liste übernehmen" | Der aktuelle Gewinn des Kandidaten wird in die Highscore-Liste übernommen und das Spiel beendet |
| 14.1 | Das Spiel soll mit einer spielbaren Anzahl Wörtern und Fragen gefüllt werden | N/A | Das Spiel enthält eine ausreichende Anzahl an Wörtern und Fragen für ein Spiel |
| 15.1 | Die Anzahl der Spielrunden soll gezählt werden | N/A | Anzeige der Anzahl der gespielten Runden im Spiel |
| 16.1 | Stellen Sie sicher, dass auf der Serverseite und Client-Seite Formulareingaben überprüft werden | Geben Sie ein leeres Textfeld ein | Fehlermeldung, dass das Textfeld nicht ausgefüllt werden darf |
| 17.1 | Wählen Sie eine Datenbank und verbinden Sie sie mit der Anwendung | N/A | Erfolgreiche Verbindung der Anwendung mit der gewählten Datenbank |
| 18.1 | Verwenden Sie eine Datenbankanbindung, die möglichst unabhängig vom tatsächlich eingesetzten Produkt ist | N/A | Anwendung nutzt eine Datenbankanbindung, die unabhängig vom eingesetzten Produkt ist |
| 19.1 | Setzen Sie Transaktionsmanagement ein | N/A | Transaktionsmanagement wurde erfolgreich implementiert |
| 20.1 | Stellen Sie sicher, dass Sicherheitsaspekte umgesetzt werden | N/A | Anwendung implementiert erfolgreich Sicherheitsaspekte |


# 5 Prototyp

Login Seite

![alt text](https://i.ibb.co/yXv8zVC/Screenshot-2023-02-17-000105.png)

✍️ Erstellen Sie Prototypen für das GUI (Admin-Interface und Quiz-Seite).

# 6 Implementation

✍️ Halten Sie fest, wann Sie welche User Story bearbeitet haben

| User Story | Datum | Beschreibung |
| ---------- | ----- | ------------ |
| ...        |       |              |

# 7 Projektdokumentation

| US-№ | Erledigt? | Entsprechende Code-Dateien oder Erklärung |
| ---- | --------- | ----------------------------------------- |
| 1    | ja / nein |                                           |
| ...  |           |                                           |

# 8 Testprotokoll

✍️ Fügen Sie hier den Link zu dem Video ein, welches den Testdurchlauf dokumentiert.

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

# 9 `README.md`

✍️ Beschreiben Sie ausführlich in einer README.md, wie Ihre Applikation gestartet und ausgeführt wird. Legen Sie eine geeignete Möglichkeit (Skript, Export, …) bei, Ihre Datenbank wiederherzustellen.

# 10 Allgemeines

- [ ] Ich habe die Rechtschreibung überprüft
- [ ] Ich habe überprüft, dass die Nummerierung von Testfällen und User Stories übereinstimmen
- [ ] Ich habe alle mit ✍️ markierten Teile ersetzt
