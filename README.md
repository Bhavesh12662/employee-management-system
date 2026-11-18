# PeopleDesk - Employee Management System

React 18 + Vite project for the Pynexia Week 3 Employee Management assignment.

## Assignment features implemented
- Employee dashboard KPI cards: total employees, active employees, employees on leave, department count.
- CRUD: add, view, edit and delete employee records.
- Employee form with required name/job title, email and phone validation.
- Department and employment-status filters.
- Search by name, role, email, department and location.
- Sorting by name, recently added, or department.
- Modal editor for add/update.
- Responsive dashboard and employee table.
- CSV export of the currently filtered records.
- LocalStorage persistence across refreshes.
- Light/dark theme toggle, empty state, delete confirmation and success toast.

## Structure
```text
employee-management-system/
├── index.html
├── package.json
├── vite.config.js
├── README.md
└── src/
    ├── main.jsx
    ├── App.jsx
    ├── data.js
    ├── styles.css
    └── components/
        ├── StatCard.jsx
        ├── EmployeeModal.jsx
        └── EmployeeTable.jsx
```

## Run
Install Node.js. In VS Code terminal, run:
```bash
npm install
npm run dev
```
Open the local URL shown by Vite (usually http://localhost:5173).

Production build:
```bash
npm run build
npm run preview
```

## React concepts used
- `useState`: employee records, form, filters, theme, notifications.
- `useEffect`: LocalStorage persistence and theme setting.
- `useMemo`: derived filtered/sorted employee list.
- Props: reusable StatCard, EmployeeModal and EmployeeTable.
- Array methods: `map`, `filter`, `sort`, `reduce` / `Set`.
- Controlled form fields and event handlers.

## Limitations
This is a frontend-only learning project. Data is stored in this browser's LocalStorage; there is no backend, database, authentication, role-based access, or cross-device sync. CSV export is not a database backup. The sample employees are fictional. Do not store sensitive real employee data in this demo.

## Test before submission
1. Add an employee and verify KPI counts.
2. Edit and delete an employee.
3. Search by name, role and email.
4. Filter by department and status.
5. Test all sort options.
6. Export CSV and open it in a spreadsheet.
7. Refresh and confirm data persists.
8. Test the mobile layout.
9. Be ready to explain useState, useEffect, useMemo, props, controlled inputs, and array methods.
# employee-management-system
