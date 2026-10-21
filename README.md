# Tip & Bill Splitter

A small web app that splits a restaurant bill between any number of people, tip included. Built with HTML, CSS and vanilla JavaScript, no libraries.

## Features

- Enter the bill amount (in rand), a tip percentage and the number of people
- Shows the tip amount, the total, and what each person pays
- Validates input: rejects empty fields, negative values and zero people
- Results are written to the page, with the error message shown inline

## How to run

1. Download or clone this repo
2. Open `index.html` in any browser

No build step or dependencies needed.

## Example

| Bill | Tip | People | Tip amount | Total | Per person |
|------|-----|--------|-----------|-------|-----------|
| R500 | 10% | 4 | R50.00 | R550.00 | R137.50 |

## What I learned

- Input `.value` is always a string, so convert with `parseFloat()` before doing maths
- Validate inputs before calculating, with early returns
- Update the page with `textContent` instead of `console.log`
- Attach events with `addEventListener` instead of inline `onclick`

## Possible improvements

- Cap the tip percentage (currently 5000% passes validation)
- Add quick-select tip buttons (10%, 15%, 20%)
- Round the per-person amount up so the bill is always covered
