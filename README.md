# Emergency Ambulance Dispatch Queue

## Project overview
This mini project demonstrates an emergency call queue for an ambulance dispatch desk. Users can register calls, assign a severity level, view the waiting queue, dispatch the next call, and review dispatch history.

## Problem statement
When several emergency calls arrive, the most urgent case should be handled first. A normal first-in-first-out queue may delay a critical case behind a less urgent case.

## Objective
To implement a simple priority-based queue that organizes emergency calls according to severity while preserving arrival order for calls with the same severity.

## Features
- Add emergency calls with caller name, location, and severity.
- Priority levels: Critical (P1), Urgent (P2), Routine (P3).
- Dispatch the highest-priority waiting call.
- FIFO order for calls with equal priority.
- Remove a waiting call.
- View dispatch history.
- Reset the demonstration.

## Data structure / algorithm
The project uses an array of call objects as a priority queue. After a call is added, the array is sorted by:
1. Priority number in ascending order (1 is highest).
2. Arrival time in ascending order for equal priorities.

Dispatch removes the first item from the queue.

## Technologies used
- HTML
- CSS
- JavaScript

## How to run
1. Download or clone this repository.
2. Open `index.html` in a web browser.
3. Add sample emergency calls and test dispatch.

No installation is required.

## Sample test
Add these calls in this order:
- Caller A — Location A — Routine (P3)
- Caller B — Location B — Critical (P1)
- Caller C — Location C — Urgent (P2)

Expected dispatch order:
1. Caller B (P1)
2. Caller C (P2)
3. Caller A (P3)

## Limitations
This is an educational simulation only. It does not connect to ambulance services, GPS, hospitals, or real emergency systems. Do not use it for actual emergency dispatch.

## Future enhancements
- Ambulance availability tracking.
- Estimated travel time display.
- Hospital selection.
- Persistent database storage.
- Login and dispatch operator dashboard.

## Author
Student mini project
