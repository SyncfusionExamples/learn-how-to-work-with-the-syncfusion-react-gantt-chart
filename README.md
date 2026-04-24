# Syncfusion React Gantt Chart Sample

A React sample demonstrating the Syncfusion React Gantt Chart with task data, subtasks, custom columns, and dependency mapping.

## Features

- Renders a Syncfusion Gantt chart in React
- Uses `@syncfusion/ej2-react-gantt`
- Displays subtasks, dates, duration, and progress
- Maps task data fields to the Syncfusion model
- Supports timeline view updates via `timelineSettings`

## Getting started

### Prerequisites

- Node.js (LTS or later)
- npm 

### Install

```bash
npm install
```

### Run

```bash
npm start
```

Open `http://localhost:3000`.

## How it works

`src/App.tsx` renders the `GanttComponent` using a task field mapping configuration and local sample data (for example, `src/data.ts` or `src/data.js`). The Gantt chart uses this configuration to display the timeline, columns, and task hierarchy.

Mapped fields:

- `TaskID`
- `TaskName`
- `StartDate`
- `EndDate`
- `Duration`
- `Progress`
- `subtasks`
- `Predeceesor`

## Customization

Timeline behavior can be adjusted using the `timelineSettings` property on the `GanttComponent`.

```tsx
<GanttComponent
  dataSource={projectData}
  taskFields={taskValues}
  timelineSettings={{ timelineViewMode: 'Day' }}
>
```

## Notes

This sample focuses on core Syncfusion Gantt functionality and serves as a starting point for adding features such as editing, sorting, and filtering.