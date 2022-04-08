# github-actions

### Hello-World Action
```yml
name: Github Actions Testing
on: [push]
jobs:
  hello-world:
    runs-on: ubuntu-latest
    steps:
      - name: Hello-World
        run: echo "Hello-World"
```

### Hello-World Action
```yml
name: Github Actions Testing
on: [push]
jobs:
  build-app:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: actions/setup-node@v2
        with:
          node-version: '16.13.2'
      - name: Install node_modules
        run: npm install
      - name: Build Project
        run: npm run build
      - name: Build Complete
        run: echo "Build Completed Successfully!"
```