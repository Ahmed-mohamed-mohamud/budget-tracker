# Budget Tracker

A simple web page for tracking personal income and expenses, built with
plain HTML and CSS as part of a week-by-week coding assignment.

## What I built

- **Logo/header** — a small wallet icon (`<img>`) next to the page title.
- **Collapsible help section** — a `<details>`/`<summary>` block titled
  "How to use this tracker" that explains how the form works.
- **Add Expense form** — a `<form>` with a text input for the expense
  name, a number input for the amount, and a `<select>` dropdown for
  category (Food, Transport, Rent, Entertainment, Other). Every input
  has a unique `id` (`expense-name`, `expense-amount`,
  `expense-category`) so a future JavaScript version can read them
  easily. The "Add Expense" button doesn't do anything yet — that
  functionality is planned for a later week.
- **Expense table** — a proper `<table>` with `<thead>`/`<tbody>`,
  column headers for Name, Amount, Category, and Date, and five
  hardcoded sample rows.
- **Budgeting tip video** — an embedded YouTube video via `<iframe>`.

## What each part does

| Section | Purpose |
|---|---|
| `index.html` | Page structure and content |
| `style.css` | All visual styling, including the table, form, hover effects, and advanced selectors |

## Advanced CSS selectors used

- **Direct child selector** — `.expense-section > form` styles only the
  form that is a direct child of the expense section.
- **Descendant selector** — `.expenses-section td` styles every table
  cell inside the expenses section, however deeply nested.
- **Position-based pseudo-class** — `tbody tr:nth-child(even)` shades
  every other table row for readability.
- **Negation pseudo-class** — `input:not([type="number"])` gives text
  inputs a different left border than number inputs.
- **Focus state** — `input:focus, select:focus` highlights whichever
  field the user is currently interacting with.

## Interactive touches

- Table rows change background color on hover.
- The "Add Expense" button shows a pointer cursor on hover.
- The "How to use this tracker" section can be expanded or collapsed.

## Next steps

Future weeks will add JavaScript so the "Add Expense" button actually
adds new rows to the table using the values from the form.
