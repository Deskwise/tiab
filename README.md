# TDD-in-a-Box

Everything you need to replicate the DroidForge Autopilot + Task-master workflow in a brand-new repository.

## Contents

```
tdd-in-a-box/
├── README.md                          # This overview
├── docs/
│   └── guides/
│       ├── autopilot-tdd-stack-setup.md   # Full setup instructions
│       ├── autopilot-agent-runbook.md     # Daily operating procedure for agents
│       ├── taskmaster-guardrails.md       # Non-negotiable rules
│       └── human-in-the-loop-workflow.md  # Post-subtask approval policy
└── scripts/
    ├── start-agent-work.sh                # Launches the next Autopilot session
    ├── autopilot-reset.sh                 # Clears stale workflow-state.json safely
    └── autopilot-wrapup.sh                # Logs end-of-session status snapshot
```

## How to use this kit

1. Copy the entire `tdd-in-a-box/` folder into your new repository’s root.
2. Run through `docs/guides/autopilot-tdd-stack-setup.md` step-by-step to install dependencies, initialize Task-master, and wire up guardrails.
3. After setup, share `docs/guides/autopilot-agent-runbook.md` with every agent. It references the other two guides and scripts so the workflow stays consistent.
4. Commit the copied files so future clones inherit the same process.

Keep this kit versioned: when guardrails or scripts evolve, update the files here and re-tag your downstream repos.
