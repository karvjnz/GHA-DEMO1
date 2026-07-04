# Common GitHub Actions Context Variables

| Variable | Description | Example |
|----------|-------------|---------|
| `${{ github.actor }}` | Username of the user who triggered the workflow | `karvjnz` |
| `${{ github.ref_name }}` | Branch or tag name | `main` |
| `${{ github.repository }}` | Repository name | `karvjnz/github-actions-demo` |
| `${{ github.event_name }}` | Event that triggered the workflow | `push` |
| `${{ github.sha }}` | Commit SHA | `4c2d7b6...` |
| `${{ github.workflow }}` | Workflow name | `If-condition Demo` |
| `${{ github.run_number }}` | Workflow run number | `15` |
| `${{ github.run_id }}` | Unique workflow run ID | `123456789` |
| `${{ github.server_url }}` | GitHub server URL | `https://github.com` |
| `${{ github.repository_owner }}` | Repository owner | `karvjnz` |


## Print GitHub Context

**Purpose:** Print useful GitHub context variables.

```yaml
- name: Print GitHub Context
  run: |
    echo "Actor      : ${{ github.actor }}"
    echo "Branch     : ${{ github.ref_name }}"
    echo "Repository : ${{ github.repository }}"
    echo "Workflow   : ${{ github.workflow }}"
    echo "Event      : ${{ github.event_name }}"
