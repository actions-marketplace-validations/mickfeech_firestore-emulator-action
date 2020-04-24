# GitHub Action for Firestore Emulation

Creates a backend Firestore emulator for testing purposes

## Usage

### Example workflow file

```
name: Run tests

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    
    steps:
    - name: Git checkout
      uses: actions/checkout@v2
    
    - name: Start Firestore
      uses: mickfeech/firestore-emulator-action@0.0.2
      with: 
        fireStoreProjectID: project-test
```