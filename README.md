# quaternionmedia/.github

Organization defaults for Quaternion Media

## Issue templates

### 📋 Because / Done when

### 🐛 Bug Report

### 💡 Feature Request

## Workflows

### `build.yml`

Workflow action to:

- Build a docker image
- Extract labels and tags
- Login to gchr.io
  - Can override with environment variables
- Publish image

#### Usage

Create a `WORKFLOW_NAME.yml` file in your repository under `.github/workflows/`

```yml
name: 🪂 Continuous Deployment

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main
  release:
    types: [published, edited, prereleased]

jobs:
  build:
    name: 🔨 Build and deploy
    uses: quaternionmedia/.github/.github/workflows/build.yml@main
```

## Organization Profile

Coming soon!
