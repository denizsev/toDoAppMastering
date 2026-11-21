# Tasks (Görevler)

A touch-first to-do app in a single HTML file. You type only the task title; date, time, list and priority are chosen by tapping chips. No sign-up, no build step, no server.

**[Open the live app →](https://denizsev.github.io/toDoAppMastering/)** (interface in Turkish)

## Why

Most to-do apps either ask you to learn a syntax like `tomorrow 15:00 #school p1`, or carry desktop habits (shortcuts, sidebars, hover menus) over to the phone. This one is built for the thumb.

## Features

- **No syntax**: tap the + button, type a title, pick date, time, list and priority with chips.
- **Swipe gestures**: swipe right to complete, left to snooze or delete (also reachable with a long press).
- **Plan my day**: go through overdue tasks one by one with large buttons.
- **Lists**: an inbox plus your own lists.
- **Repeating tasks**: daily, weekdays, weekly, monthly.
- **Dark mode**, a progress ring and undo for deletes (5 seconds).
- **Your data stays local**: tasks are saved in the browser's `localStorage` and never sent anywhere.
- **Add to home screen**: opens full screen like an app on iOS.

## Tech stack

Vanilla JavaScript, HTML and CSS in one file, no dependencies.

- Dates are handled as calendar days (`YYYY-MM-DD`) to avoid time-zone and daylight-saving bugs.
- Reordering uses [fractional indexing](https://www.figma.com/blog/realtime-editing-of-ordered-sequences/), so moving one task never renumbers the others.

## Run locally

Download `index.html` and open it in a browser. That's all.

## License

[MIT](LICENSE)
