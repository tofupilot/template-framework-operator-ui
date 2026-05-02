# Framework Operator UI

![Cover](cover.png)

Two-phase Framework procedure showing operator UI components: a numeric input + slider for parameters, then live text and progress bar updates from Python.

## What's Inside

- `procedure.yaml`: defines two phases with UI components
- `phases/run_test.py`: updates display components during execution
- `pyproject.toml`: uv-managed Python project

## Use This Template

Clone it from the **New Procedure** flow in TofuPilot. TofuPilot creates the repository in your account, links a procedure, builds the first deployment, and pushes it to a station.

## Structure

```
.
├── procedure.yaml
├── phases/
│   └── run_test.py
├── pyproject.toml
└── README.md
```

## Key Concepts

- **Input components**: `number_input`, `slider` for operator data entry
- **Display components**: `text`, `progress` for live updates
- **Reading inputs**: access operator values with `ui.component_key`
- **Updating displays**: assign with `ui.component_key = value` from Python

## Next Steps

See the [TofuPilot guides](https://www.tofupilot.com/guides) for more templates.
