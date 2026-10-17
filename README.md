# Exam Clock

A lightweight, single-page timer for practising HSC written exams. It runs entirely in your browser with no build step, account, or external service.

**Live site:** `https://theinfintigamer.github.io/exam-clock/` (available after GitHub Pages finishes its first deployment)

## Features

- 2026 HSC paper presets for written exams, with search and paging.
- Separate reading and working time, adjustable in minutes and seconds.
- Start, pause, resume, add time, and reset controls.
- Optional finish sound, five-minute warning, and one-minute warning.
- Full-screen exam mode. If the browser reports that full screen was exited or the page was interrupted, the timer pauses and offers resume/reset.
- Appearance themes, custom timer/accent colours, glass transparency, graphics quality, and reduced motion.
- Local session recovery and saved preferences using browser `localStorage`.
- Responsive layout and accessibility labels, visible keyboard focus, and system reduced-motion support.

## Start practising

1. Open the live site in a current browser.
2. Open **Controls → Presets** and search for your subject or paper.
3. Review the selected paper's reading and working time in **Controls → Time**. You can adjust either phase before starting.
4. Select **Start exam**. The site requests full-screen mode and starts the countdown.
5. Use the on-screen pause and confirmation controls when you need to pause or change settings.

Preset timings are practice aids. Check the instructions printed on your own exam paper and the current NESA timetable before relying on a duration.

## Browser and privacy notes

- The site is plain HTML, CSS, and JavaScript. It has no package install or server component.
- Timer recovery, selected tab, appearance, graphics, and alert preferences are stored locally in this browser. They are not sent to a server by the site.
- Full-screen, sound, and screen-wake behavior depend on browser permissions and support. Browsers can always let a user leave full screen; the timer responds by pausing when it detects the interruption.
- Clearing this site's browser storage removes saved preferences and recovery state.

## Run locally

Download `index.html` and `ExamClockLogo.svg` into the same folder, then open `index.html` in a browser. The timer itself does not require a local server.

## Deployment and updates

GitHub Pages publishes the files at the repository root from the `main` branch. `.nojekyll` tells Pages to serve the static files directly. To update the site, replace `index.html` and any changed assets, then commit and push to `main`; Pages automatically builds and deploys the update.

## Project files

- `index.html` — complete timer application.
- `ExamClockLogo.svg` — browser tab icon.
- `.nojekyll` — disables Jekyll processing for this static site.
