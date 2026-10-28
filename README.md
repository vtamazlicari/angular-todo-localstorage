# TodoAngular

A small todo app built with Angular 6 and Bootstrap 4. Tasks are saved in the browser's `localStorage` (key `TASK`), so they stay after a page reload. There is no backend.

## Features

- **Todo list** (`/` or `/todo`): add a task with a name, date and description. Open tasks are listed first and finished tasks after them. Any task can be deleted.
- **Task details** (`/details/:name`): shows a single task and lets you mark it as finished.
- **Contact** (`/contact`): a contact form with validation (name, valid email, message). Submitting it only shows the values in an alert; nothing is sent anywhere.
- **About** (`/about`): a page of placeholder text.

Tasks are looked up by name, so two tasks with the same name will conflict.

## Project structure

```
src/app/
  core/       layout, header, navbar, footer, task details
  modules/    todo (page + TodoService), contact, about
  shared/     Tasks interface
```

## Development server

Run `npm install`, then `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app reloads automatically when you change a source file.

## Build

Run `ng build` to build the project. The build output goes to `dist/`. Use `--prod` for a production build.

## Tests

- `ng test` runs the unit tests via [Karma](https://karma-runner.github.io).
- `ng e2e` runs the end-to-end tests via [Protractor](http://www.protractortest.org/).
