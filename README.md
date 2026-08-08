# Daily Ledger

A simple daily task tracker and progress calendar built as a single HTML file.

## Features

- Add daily tasks
- Edit task names by clicking a task
- Mark tasks as completed
- Delete tasks
- Add optional times to tasks
- Automatically saves tasks and progress in the browser using `localStorage`
- Daily progress score shown at the top
- Calendar view with color-coded daily progress
- Click any calendar date to view task history
- Add events to upcoming dates
- Event countdowns such as Today, Tomorrow, and days left
- Automatically starts a new day at midnight
- Fullscreen mode when supported by the browser
- Responsive layout for desktop and mobile screens
- Landscape optimization for smaller screens

## How to Use

### 1. Open the website

Open `index.html` in a modern web browser.

No server, database, or account is required for the basic functionality.

### 2. Add a task

Type a task into the **Task** box and press `+`.

To add a time:

1. Press the 🕐 button.
2. Select a time.
3. Press `+`.

### 3. Complete a task

Click the checkbox beside a task.

Completed tasks are counted toward the day's progress.

### 4. Edit a task

Click the task name, edit the text, and press Enter or click somewhere else to save it.

### 5. Delete a task

Press the `✕` button beside the task.

### 6. Check previous days

Click a date in the calendar.

For past dates, the website can show:

- Completed tasks
- Missed tasks
- Completion percentage

### 7. Add an event

Click a future date in the calendar and enter an event.

Events appear separately on the calendar and can show a countdown.

## Progress Colors

| Color | Meaning |
|---|---|
| Dark green | 100% completed |
| Green | 80–99% completed |
| Yellow | 60–79% completed |
| Orange/Red | 40–59% completed |
| Dark red | 0–39% completed |
| Grey | No data |
| Cyan | Event |

## Data Storage

The website stores its data locally in the browser using `localStorage`.

The current implementation stores:

- Task list
- Daily task completion history
- Calendar events

This means the data is tied to the browser/device where the website is being used.

**Important:** Clearing the browser's site data/local storage can remove the saved information.

## Project Structure

```text
Daily-Ledger/
└── index.html
```

The current version is self-contained: HTML, CSS, and JavaScript are all inside `index.html`.

## Publishing with GitHub Pages

1. Create a new repository on GitHub.
2. Upload `index.html`.
3. Open the repository's **Settings**.
4. Go to **Pages**.
5. Select **Deploy from a branch**.
6. Select the `main` branch and `/ (root)`.
7. Save the settings.
8. GitHub will provide the public website URL.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Browser `localStorage`
- CSS Grid
- CSS Flexbox
- Responsive Media Queries
- Fullscreen Web API

## Notes

The website does not use a backend or online database. Saving is performed locally on the device/browser.

The interface uses Google Fonts when an internet connection is available; the browser falls back to system fonts if the fonts cannot be loaded.
