# AZD Introduction

Azure Developer CLI (azd) is an open-source tool that accelerates the time it takes for you to get your application from local development environment to Azure.  
Azd provides best practice, developer-friendly commands that map to key stages in your workflow, whether you’re working in the terminal, your editor or integrated development environment (IDE), or CI/CD (continuous integration/continuous deployment).

Details refer : https://learn.microsoft.com/en-us/azure/developer/azure-developer-cli/overview

## Installation

Below is the installation script you could run in windows, for other installation, please refer https://learn.microsoft.com/en-us/azure/developer/azure-developer-cli/install-azd?tabs=winget-windows%2Cbrew-mac%2Cscript-linux&pivots=os-windows
```poershell
winget install microsoft.azd
```

## Login 
```bash
azd login
```

## Templates
```bash
# list official templates
azd template list 

# just init and select a template then
azd init 

# specify a template and init it
azd init --template todo-python-mongo 

# use customized template

azd init --template calvinonazure/app-service-linux-node
azd init --template calvinonazure/app-service-linux-python

```
You could also view the public templates from https://github.com/topics/azd-templates

## Deploy
```bash
azd up
azd up --debug # up with debug
```

## Clean Up
```bash
azd down
```