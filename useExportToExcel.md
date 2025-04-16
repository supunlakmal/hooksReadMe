# useExportToExcel

A React hook that simplifies exporting data to Excel files with automatically adjusted column widths.

## Installation

This hook is included in the `supunlakmal/hooks` package:

```bash
npm install supunlakmal/hooks
# or
yarn add supunlakmal/hooks
```

### Dependencies

This hook requires the `xlsx` library:

```bash
npm install xlsx
# or
yarn add xlsx
```

## Usage

```jsx
import React from "react";
import { useExportToExcel } from "supunlakmal/hooks";

function ExportButton() {
  const exportToExcel = useExportToExcel();

  const data = [
    { id: 1, name: "John Doe", email: "john@example.com" },
    { id: 2, name: "Jane Smith", email: "jane@example.com" },
  ];

  const columns = [
    { key: "id", label: "ID" },
    { key: "name", label: "Full Name" },
    { key: "email", label: "Email Address" },
  ];

  const handleExport = () => {
    exportToExcel(data, columns, "user-data.xlsx");
  };

  return <button onClick={handleExport}>Export to Excel</button>;
}
```

## API

### `useExportToExcel(): ExportFunction`

Returns a function that exports data to an Excel file.

#### Return Value

The hook returns a function with the following signature:

```typescript
(data: any[], columns: Column[], fileName?: string) => void
```

##### Parameters for the export function

| Name       | Type       | Default       | Description                                    |
| ---------- | ---------- | ------------- | ---------------------------------------------- |
| `data`     | `any[]`    | (required)    | Array of objects containing the data to export |
| `columns`  | `Column[]` | (required)    | Array of column definitions                    |
| `fileName` | `string`   | `'data.xlsx'` | Name of the file to download                   |

##### Column Definition

| Property | Type     | Description                                   |
| -------- | -------- | --------------------------------------------- |
| `key`    | `string` | The object property to extract the value from |
| `label`  | `string` | The column header text to display             |

## Features

- Automatically downloads the file in the browser
- Auto-sizes columns based on content
- Formats data into a clean table structure
- Customizable file name

## Example: Data Table with Export

```jsx
import React, { useState, useEffect } from "react";
import { useExportToExcel } from "supunlakmal/hooks";

function DataTable() {
  const [users, setUsers] = useState([]);
  const exportToExcel = useExportToExcel();

  useEffect(() => {
    // Fetch data from an API
    fetch("/api/users")
      .then((res) => res.json())
      .then((data) => setUsers(data));
  }, []);

  const columns = [
    { key: "id", label: "ID" },
    { key: "name", label: "Name" },
    { key: "email", label: "Email" },
    { key: "role", label: "Role" },
    { key: "status", label: "Status" },
  ];

  const handleExport = () => {
    exportToExcel(users, columns, "users-report.xlsx");
  };

  return (
    <div>
      <div className="table-header">
        <h2>Users</h2>
        <button onClick={handleExport}>Export to Excel</button>
      </div>

      <table>
        <thead>
          <tr>
            {columns.map((col) => (
              <th key={col.key}>{col.label}</th>
            ))}
          </tr>
        </thead>
        <tbody>
          {users.map((user) => (
            <tr key={user.id}>
              {columns.map((col) => (
                <td key={`${user.id}-${col.key}`}>{user[col.key]}</td>
              ))}
            </tr>
          ))}
        </tbody>
      </table>
    </div>
  );
}
```

## Implementation Details

- Uses the [SheetJS (xlsx)](https://sheetjs.com/) library for Excel file generation
- Automatically calculates optimal column widths based on content
- Formats data from an array of objects into a spreadsheet structure
- Triggers a file download in the browser
