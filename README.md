# StudyTasks – Frontend

- **Teammitglied:** Anakin Timm
- **Projektname:** StudyTasks

## Projektbeschreibung

StudyTasks ist ein Aufgabenplaner für Studierende. Die Anwendung soll
Studienaufgaben und Abgabetermine übersichtlich darstellen. Später sollen
Aufgaben erstellt, bearbeitet, gelöscht und als erledigt markiert werden können.

## Milestone 2

Das Frontend wurde mit Vue 3 und TypeScript umgesetzt.

Die Hauptkomponente `App.vue` bindet die eigene Unterkomponente
`TaskList.vue` ein. Diese stellt drei fest hinterlegte Beispielaufgaben
mit `v-for` dar. Jede Aufgabe besitzt eine eindeutige ID, die über
`:key="task.id"` verwendet wird.

Angezeigt werden Titel, Beschreibung, Abgabedatum und Erledigungsstatus.

Eine Verbindung zum Spring-Boot-Backend besteht in diesem Stand noch nicht.

## Lokal starten

Voraussetzung: eine mit dem Projekt kompatible Node.js-Version und npm.

Abhängigkeiten installieren:

```sh
npm install
```

Entwicklungsserver starten:

```sh
npm run dev
```

Anschließend die im Terminal angezeigte lokale Adresse im Browser öffnen.

## Produktionsbuild

```sh
npm run build
```

Der Befehl prüft die TypeScript-Typen und erstellt den Produktionsbuild
im Ordner `dist`.

## Tech-Stack

- Vue 3
- TypeScript
- Vite
- CSS

Für das Gesamtprojekt sind außerdem Spring Boot, Managed PostgreSQL
und das Deployment auf Render vorgesehen.