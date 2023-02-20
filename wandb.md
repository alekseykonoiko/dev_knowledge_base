### Tracking
Track all experiments
`wandb.init`

`wandb.logs`

### Artifacts
Version and track datasets and models

```bash
# Start run
with wandb.init(project="artifacts-example", job_yupr="load-data") as run:
```

```bash
# Create artifact
```

```bash
# Store new file into artifact, and write something into its content (like adding new images to dataset)
```

```bash
# Save the artifact to W&B
```

```bash
```

### W&B sweeps
Tune hyperparameters
