# github-actions

### Hello-World Action
```yml
name: Github Actions Testing
on: [push]
jobs:
  build-app:
    runs-on: ubuntu-latest
    steps:
      - name: Hello-World
        run: echo "Hello-World"
```