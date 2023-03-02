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

Ich werde für dieses Projekt ReactJS anwenden:
ReactJS ist eine JavaScript-Bibliothek, die zur Erstellung von Benutzeroberflächen (UIs) in Webanwendungen verwendet wird. Sie wurde von Facebook entwickelt und wird jetzt von einer Community von Entwicklern gepflegt. ReactJS ermöglicht es Entwicklern, wiederverwendbare UI-Komponenten zu erstellen und effizient zu aktualisieren, basierend auf Änderungen in den Anwendungsdaten, was es zu einer beliebten Wahl für den Aufbau komplexer und dynamischer Webanwendungen macht. ReactJS verwendet eine deklarative Syntax und virtuelles DOM (Document Object Model), um die UI effizient zu verwalten und zu aktualisieren, basierend auf Benutzerinteraktionen und Datenänderungen.


# 3 Datenbank

Ich werde Firestore von Firebase anwenden:
Firestore ist eine NoSQL-Datenbank, die von Google entwickelt wurde und als Teil der Firebase-Plattform verfügbar ist. Sie ermöglicht es Entwicklern, schnell und einfach skalierbare und synchronisierte Anwendungen zu erstellen, die in Echtzeit Daten speichern und abrufen können. Firestore unterstützt auch eine Vielzahl von Plattformen, darunter Web, iOS, Android und mehr.

# 4.1 User Stories

| US-№    | Verbindlichkeit | Typ        | Beschreibung                                                 |
| ----    | --------------- | ---------- | ----------------------------------                           |
| US-1 | Muss | Funktional |Als Administrator möchte ich mich durch die Eingabe von Benutzername und Passwort authentifizieren können, um auf die Administrationsfunktionen zugreifen zu können. |
| US-2 | Muss | Funktional |Als Administrator möchte ich Rätselwörter anlegen, ändern und löschen können, um die Rätselbank zu verwalten.|
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
| US-13 | Muss | Funktional | Als Kandidat möchte ich jederzeit die Möglichkeit haben entweder weiter zu spielen |
| US-14 | Muss | Funktional | Als Administrator möchte ich sicherstellen, dass das Spiel mit einer spielbaren Anzahl Wörtern und Fragen gefüllt ist. |
| US-15 | Muss | Funktional | Als Administrator möchte ich die Anzahl der Spielrunden zählen zu können. |
| US-16 | Muss | Rand | Als Entwickler möchte ich sicherstellen, dass einfache Formulareingaben auf Client- und Serverseite geprüft werden. |
| US-17 | Muss | Rand | Als Entwickler möchte ich die Wahl haben, welche Art von Datenbank verwendet wird. |
| US-18 | Muss | Rand | Als Entwickler möchte ich eine Datenbankanbindung verwenden, die möglichst unabhängig vom tatsächlich eingesetzten Produkt ist. |
| US-19 | Muss | Rand | Als Entwickler möchte ich Transaktionsmanagement einsetzen, um die Integrität der Daten sicherzustellen. |
| US-20 | Muss | Rand | Als Entwickler möchte ich Sicherheitsaspekte umsetzen, um die Daten und die Anwendung vor unbefugtem Zugriff zu schützen. |
| MU-1 | Kann | Rand | Als Kandidat möchte ich mit anderen, die gleichzeitig das Spiel spielen, chatten. |


# 4.2 Testfälle

| TC-№ | Vorbereitung | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1 | Erstellen Sie ein gültiges Konto mit dem Benutzernamen "khang@cung.ch" und dem Passwort "Passwort321" | Geben Sie Benutzernamen "khang@cung.ch" und dem Passwort "Passwort321" ein | Erfolgreiche Anmeldung und Zugriff auf die Administrationsfunktionen |
| 2.1 | Legen Sie ein Rätselwort an | Fügen Sie als Rätselwort "Kiwi","Banana" als Antwort hinzu | Erfolgreiche Anlage des Rätselwortes |
| 3.1 | Legen Sie eine Kategorie an | Geben Sie "Früchte" als Kategorie und dazu mind. 1 Element in der Sammlung rein | Erfolgreiche Anlage der Kategorie |
| 4.1 | Löschen Sie einen Eintrag aus der Highscore-Liste | Wählen Sie den Eintrag "Spieler1" aus der Highscore-Liste und klicken Sie auf "Löschen" | Erfolgreiche Löschung des Eintrags "Spieler1|
| 5.1 | Öffnen Sie die Anwendung im Webbrowser | N/A | Anzeige der Anwendung im Webbrowser |
| 6.1 | Der Kandidat oder die Kandidatin gibt einen Namen ein | Geben Sie "Max Mustermann" als Namen ein (Das Spiel noch zu Ende spielen) | Er kommt ins Spiel rein |
| 7.1 | Der Kandidat oder die Kandidatin sieht den Kontostand | N/A | Anzeige des aktuellen Kontostands |
| 8.1 | Der Kandidat oder die Kandidatin sieht die Lebenspunkte | N/A | Anzeige der aktuellen Lebenspunkte |
| 9.1 | Der Kandidat oder die Kandidatin wählt eine Antwort | Wählen Sie Buchstaben aus | Anzeige "richtig" oder "falsch" |
| 10.1 | In der Highscore-Liste werden Rang, Name des Spielers aufgeführt | N/A | Anzeige der Highscore-Liste mit Rang, Name des Spielers |
| 11.1 | Die Highscore-Liste wird nach Rang, der durch die Höhe des Geldbetrags bestimmt wird, aufsteigend sortiert | N/A | Anzeige der Highscore-Liste sortiert nach Rang, der durch die Höhe des Geldbetrags bestimmt wird, aufsteigend |
| 12.1 | Kein Rätsel-Wort und keine Phrase sollen einem Spieler mehr als einmal gestellt werden | N/A | Keine Wiederholung von Rätsel-Wörtern und Phrasen für einen Spieler |
| 13.1 | Der Kandidat kann jederzeit entweder spielen, oder aufhören und seinen Gewinn in die Higscore-Liste übernehmen | Wählen Sie "Stop" | Das Spiel wird beendet und Sie werden zurück zur Login gebracht |
| 14.1 | Das Spiel soll mit einer spielbaren Anzahl Wörtern und Fragen gefüllt werden | N/A | Das Spiel enthält eine ausreichende Anzahl an Wörtern und Fragen für ein Spiel |
| 15.1 | Die Anzahl der Spielrunden soll gezählt werden | N/A | Anzeige der Anzahl der gespielten Runden im Spiel |
| 16.1 | Stellen Sie sicher, dass auf der Serverseite und Client-Seite Formulareingaben überprüft werden | Geben Sie ein leeres Textfeld ein | Fehlermeldung, dass das Textfeld nicht ausgefüllt werden darf |
| 17.1 | Wählen Sie eine Datenbank und verbinden Sie sie mit der Anwendung | N/A | Erfolgreiche Verbindung der Anwendung mit der gewählten Datenbank |
| 18.1 | Verwenden Sie eine Datenbankanbindung, die möglichst unabhängig vom tatsächlich eingesetzten Produkt ist | N/A | Anwendung nutzt eine Datenbankanbindung, die unabhängig vom eingesetzten Produkt ist |
| 19.1 | Setzen Sie Transaktionsmanagement ein | N/A | Transaktionsmanagement wurde erfolgreich implementiert |
| 20.1 | Stellen Sie sicher, dass Sicherheitsaspekte umgesetzt werden | N/A | Anwendung implementiert erfolgreich Sicherheitsaspekte |


# 5 Prototyp

Login Seite

![login](https://i.ibb.co/yXv8zVC/Screenshot-2023-02-17-000105.png)

Spin Site

![Spin](https://i.ibb.co/Y8CpJy5/Screenshot-2023-02-17-000527.png)

✍️ Erstellen Sie Prototypen für das GUI (Admin-Interface und Quiz-Seite).

# 6 Implementation

✍️ Halten Sie fest, wann Sie welche User Story bearbeitet haben

| User Story | Datum      | Beschreibung |
| ---------- | ---------- | ------------ |
| US1        | 05.02      | Ich habe einen Login und Sign Up erstellt             |
| US2        | 26.02      | Ich habe einen Admin Panel erstellt, welches ein ManageCat Klasse hat            |
| US3        | 26.02      | Ich habe einen Admin Panel erstellt, welches ein AddCat Klasse hat             |
| US4        | 01.03      | Ich habe einen Admin Panel erstellt, welches ein ManageUser Klasse hat             |
| US5        | Day 1      | Ich habe einen React App erstellt.             |
| US6        | 05.02      | Ich habe einen Login und Sign Up erstellt             |
| US7        | 10.02      | Ich habe angefangen mit dem Spiel programmieren             |
| US8        | 10.02      | Ich habe angefangen mit dem Spiel programmieren             |
| US9        | 05.02      | Ich habe angefangen mit dem Spiel programmieren             |
| US10        | 02.03      | Ich habe eine Liste Erstellt und darein die Daten aus der Sammlung "Users" genommen             |
| US11        | 05.02      | Ich habe diese oben genannte Liste sortiert nach Grösse             |
| US14        | 05.02      | Ich habe Sammlungen auf mein Firestore Datenbank erstellt             |
| US16        | 05.02      | Ich habe es programmiert, sodass, wenn der Benutzer nicht im Firebase ist, dass die Seite nicht wechselt             |
| US17        | 05.02      | Ich habe Firebase ausgewählt             |
| US18        | 05.02      | Ich habe Firebase angebunden             |
| US20        | 05.02      | Firebase hat ein automatisches Passwort Hashing             |


# 7 Projektdokumentation

| US-№ | Erledigt? | Entsprechende Code-Dateien oder Erklärung |
| ---- | --------- | ----------------------------------------- |
| 1    |  ja |   Erst wenn der Benutzer vom Firebase gesehen wird, wird die Seite gewechselt                                        |
| 2    |  ja |   Siehe ManageCat                                        |
| 3    |  ja |   Siehe AddCat                                        |
| 4    |  ja |   Siehe ManageUser                                        |
| 5    |  ja |                                           |
| 6    |  ja |                                           |
| 7    |  ja |                                           |
| 8    |  ja |                                           |
| 9    |  ja |                                           |
| 10    |  ja |                                           |
| 11    |  ja |                                           |
| 12    |  nein |                                           |
| 13    |  nein |                                           |
| 14    |  ja |                                           |
| 15    |  nein |                                           |
| 16    |  ja |                                           |
| 17    |  ja |                                           |
| 18    |  ja |                                           |
| 19    |  nein |                                           |
| 20    |  ja |                                           |



# 8 Testprotokoll

[Video Here](https://example.com/my-link](https://www.youtube.com/watch?v=6TU6qQCfEFQ) "Video Here")

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  | 02.03.2023      |   Gut       |   Cung     |
| 1.2  | 02.03.2023      |   Gut       |   Cung     |
| 1.3  | 02.03.2023      |   Gut       |   Cung     |
| 1.4  | 02.03.2023      |   Gut       |   Cung     |
| 1.5  | 02.03.2023      |   Gut       |   Cung     |
| 1.6  | 02.03.2023      |   Gut       |   Cung     |
| 1.7  | 02.03.2023      |   Gut       |   Cung     |
| 1.8  | 02.03.2023      |   Gut       |   Cung     |
| 1.9  | 02.03.2023      |   Gut       |   Cung     |
| 1.11  | 02.03.2023      |   Gut       |   Cung     |
| 1.14  | 02.03.2023      |   Gut       |   Cung     |
| 1.16  | 02.03.2023      |   Gut       |   Cung     |
| 1.17  | 02.03.2023      |   Gut       |   Cung     |
| 1.18  | 02.03.2023      |   Gut       |   Cung     |
| 1.20  | 02.03.2023      |   Gut       |   Cung     |


✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

# 9 `README.md`

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)


# 10 Allgemeines

- [ ] Ich habe die Rechtschreibung überprüft
- [ ] Ich habe überprüft, dass die Nummerierung von Testfällen und User Stories übereinstimmen
- [ ] Ich habe alle mit ✍️ markierten Teile ersetzt



