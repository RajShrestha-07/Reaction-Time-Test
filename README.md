# Reaction Test

Reaction Test is a small web game that measures how fast you react. Tap the box to start, wait for it to turn orange, then tap as fast as you can. It shows your time in milliseconds, your last eight results, your best time and your average. Your best time is saved on your device.

Live demo: https://rajshrestha-07.github.io/Reaction-Time-Test/

Built with: HTML, CSS and JavaScript.

What this project shows: The game uses a timer and a clock. When you start, `setTimeout` waits a random time between 1.5 and 4 seconds before turning the box orange, so you can't guess when it will change. At that moment the code saves the time with `performance.now()`, which is accurate to a fraction of a millisecond. When you tap, it subtracts the saved time from the current time to get your reaction time. If you tap too early, the timer is cancelled and the round restarts. The game is a small state machine: idle, wait, go, result and early.

What I'm learning from it: I'm studying how the code uses `setTimeout` and `performance.now()` to measure time, and how the `state` variable decides what each tap does.
