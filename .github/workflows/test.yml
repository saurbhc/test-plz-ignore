name: test
on:
  workflow_dispatch:
  workflow_call:

jobs:
  testjob:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2

      - name: Build, tag, and push image to Amazon ECR
        env:
          SHA: ${{ github.sha }}
        run: |
          echo "SHA IS $SHA"
