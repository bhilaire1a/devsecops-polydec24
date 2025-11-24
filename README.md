# DevSecOps December 2025 - Polytech

## ⚠️ IMPORTANT: Academic Integrity Policy

**AI ASSISTANCE IS STRICTLY PROHIBITED FOR THIS EXERCISE**

By participating in this course, you agree to:
- Complete all exercises using your own knowledge and skills
- NOT use AI assistants (GitHub Copilot, ChatGPT, Claude, Bard, etc.)
- NOT use AI-powered code completion or generation tools
- NOT share solutions with other students
- Conduct independent research using official documentation only

**Violation of this policy may result in academic sanctions.**

For detailed restrictions, see `AI-AGENTS.md` and `LICENSE.txt`.

## Disclaimer
This code is a copy of a tutorial from GitHub.
It contains INTENTIONAL security findings but none of them are active.
This is for EDUCATION purpose ONLY.

## Exercice

/!\ Note : for education purpose, you should NOT use the template workflow but only the manual setup.

### Exercice 1 : Hello World

1. Create a workflow file
2. EXIT : the workflow must PASS and echo the content of `hello_world.txt`

#### Results
- Workflow code
- URL of the BUILD (https://github.com/...../actions/runs/12098085715)
- Screenshot of the ECHO in the build


### Exercice 2 : Build and Test

1. Create a new workflow file
2. The workflow must build (`npm run build`) the application in 1 step and execute tests (`npm test`) in another
3. EXIT : All workflows RUN needs to be passing

#### Results
- Workflow code
- URL of the BUILD (https://github.com/...../actions/runs/12098085715)
- Screenshot of the TEST logs

### Exercice 3 : Execute SCA
This exercice is NOT in the previous tutorial but based on the previous exercice. The goal is to run an SCA, find vulnerabilities and fix them.

1. Update the workflow from exercice 2
2. The workflow must execute an SCA to find vulnerabilities in dependencies
3. The code needs to be fixed to update (or remove) the vulnerable dependency. HINT : the update is minimal.
4. EXIT : All workflows RUN needs to be passing

#### Results
- Workflow code
- Screenshot of the SCA run
- URL of the BUILD (https://github.com/...../actions/runs/12098085715)
- SCA finding (dependency name and version)
- Fix proposal

### Exercice 4 : Execute a SAST
This exercice is NOT in the previous tutorial but based on the previous exercice. The goal is to run an SAST, find 2 critical vulnerabilities and fix them.
HINT : for differents reason, you may need to find a SAST tool that starts with a B.

1. Update or create a new workflow
2. The workflow must execute a SAST to find issues in code
3. The code needs to be fixed to remove the finding
4. EXIT : All workflows RUN needs to be passing

#### Results
- Workflow code
- Screenshot of the SAST critical findings
- URL of the BUILD (https://github.com/...../actions/runs/12098085715)
- SAST findings (files + lines + CWEs + small explanation about the risks) 

## Going further

### CICD
You may continue the tutorial (see `SUPPORT.MD`) and play with workflow template to learn more about CICD

### Security
I recommand to play with the (OWASP Juice Shop)[https://github.com/juice-shop/juice-shop] to scan it and find nice vulnerabilties to train yourself.
