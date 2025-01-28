# GitHub Actions Lab - CheckPoint 3 (CSP 451 NIA - Winter 2025) 

## Objective
CheckPoint 3 demonstrates how to create a simple GitHub Actions workflow to automate a basic task in a GitHub repository.

## Prerequisites
- A GitHub account
- Basic knowledge of Git
- A text editor (Notepad)

## Steps Taken 

1. **Created a New GitHub Repository**
   - https://github.com/sangeethvethanayagam/CheckPoint3.git

2. **Set Up the Workflow Directory**
  
	Added a new directory structure by creating a new file 
        .github/workflows/.gitkeep 

3. **Created the Workflow File**
   - In the `.github/workflows` directory, created a file named `main.yml`.

4. ** Workflow**
   - Added the following content to the `main.yml` file:
     ```yaml
name: CheckPoint3Workflow

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v3

      - name: Print message
        run: echo "Hello, GitHub Actions!"
     ```

5. **Committed and Pushed Changes**
  


## Expected Outcome
The workflow will run successfully and display the message `Hello, GitHub Actions!` in the logs.

## Troubleshooting from Lab instructions 
- Ensure the `main.yml` file has correct YAML syntax.
- Verify the trigger event is correctly defined. Ensure that the event you specified in the on
  keyword matches the action that triggered the workflow.
- Check logs in the Actions tab for any errors.



## Thank you
## Sangeeth
