# Syncfusion React Gantt Chart Sample

A React sample demonstrating the Syncfusion [React Gantt Chart](https://www.syncfusion.com/gantt-sdk/react-gantt-chart?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples) with task data, subtasks, custom columns, and [dependency mapping](https://ej2.syncfusion.com/react/documentation/gantt/task-dependency?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples).

## Features

- Renders a Syncfusion Gantt chart in React
- Uses `@syncfusion/ej2-react-gantt`
- Displays subtasks, dates, duration, and progress
- Maps task data fields to the Syncfusion model
- Supports [timeline](https://ej2.syncfusion.com/react/documentation/gantt/timeline/timeline?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples) view updates via `timelineSettings`

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

`src/App.tsx` renders the `GanttComponent` using a task field mapping configuration and local sample data (for example, `src/data.ts` or `src/data.js`). The Gantt chart uses this configuration to display the [timeline](https://ej2.syncfusion.com/react/documentation/gantt/timeline/timeline?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples), [columns](https://ej2.syncfusion.com/react/documentation/gantt/columns/columns?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples), and task hierarchy.

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

This sample focuses on core Syncfusion Gantt functionality and serves as a starting point for adding features such as editing, [sorting](https://ej2.syncfusion.com/react/documentation/gantt/sorting?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples), and [filtering](https://ej2.syncfusion.com/react/documentation/gantt/filtering/filtering?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples).

## Related Links

- [Explore React Gantt Chart](https://www.syncfusion.com/gantt-sdk/react-gantt-chart?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples)
- [Gantt Chart Feature Overview](https://ej2.syncfusion.com/react/documentation/gantt/overview?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples)
- [React Gantt Chart Getting Started Guide](https://ej2.syncfusion.com/react/documentation/gantt/getting-started?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples)
- [React Gantt API Documentation](https://ej2.syncfusion.com/react/documentation/api/gantt/index-default?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples)
- [React Gantt Chart Live Demos and Examples](https://ej2.syncfusion.com/react/demos/?utm_source=github&utm_medium=listing&utm_campaign=react-gantt-chart-github-samples#/tailwind3/gantt/default)
