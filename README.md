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

- Node.js installed
- npm available

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

`src/App.tsx` maps `taskValues` to the Gantt data model using `src/data.js`. The chart renders the configured columns and row data.

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

To change the timeline view, add `timelineSettings` to `GanttComponent` in `src/App.tsx`:

```tsx
<GanttComponent
  dataSource={projectData}
  taskFields={taskValues}
  timelineSettings={{ timelineViewMode: 'Day' }}
>
```

## Notes

This sample focuses on basic Syncfusion Gantt features and serves as a starting point for extending the chart with editing, sorting, filtering, and additional settings.
