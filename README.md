# Budget Tracker - Week 2 Assignment

This is a simple Budget Tracker built with HTML and CSS. This is the Week 2 upgrade from Week 1.

## What I Built
A web page that displays a list of expenses in a table and has a form to add new expenses, plus multimedia content.

## File Breakdown

### index.html
- **Header with Logo**: Uses `<img>` tag with `src`, `alt`, and `width` attributes for the logo near the main heading.
- **Expense Table**: Replaced the "No expenses yet" text with a `<table>` using `<thead>` for headers (Name, Amount, Category, Date) and `<tbody>` with 5 hardcoded expense rows using `<td>`.
- **Add Expense Form**: Wrapped all inputs inside a `<form>`. Replaced category text input with `<select>` containing 5 options (Food, Transport, Rent, Entertainment, Other). All inputs have matching IDs: `expense-name`, `expense-amount`, `expense-category`, `expense-date`. Button has `type="button"`.
- **Multimedia**: Embedded YouTube video using `<iframe>` with `width`, `height`, `title`, and `frameborder`.
- **Interactive Element**: Added `<details>` and `<summary>` for "How to use this tracker".

### style.css
- **Table Styling**: `border-collapse: collapse`, padding, colored header row (`thead tr`), alternating rows with `tr:nth-child(even)`.
- **Interactive Styles**: `tr:hover` changes background color, `cursor: pointer` on button.
- **Advanced Selectors Used (6 total, only 3 required)**:
    1. Descendant: `.expenses-section td`
    2. Direct Child: `.add-expense-section > form`
    3. Position pseudo-class: `tr:nth-child(even)` and `tr:first-child`
    4. Negation: `input:not([type="submit"])`
    5. Focus state: `input:focus`
