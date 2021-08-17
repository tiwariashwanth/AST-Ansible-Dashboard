# Deploying Azure Dashboards using Ansible and ARM templates

## For templating, Jinja2 has been used

## Pre-reqs

- Azure resource group 
- Dashboard JSON needs to be converted to ARM template format
- Parameterize Dashboard JSON


## Running Ansible Playbook

`ansible-playbook deploy.yaml -e env=dev -e dashboardname=devdashansible002 -e deployname=atansibledeployment010 -e subscriptionId="bfba7d97-7864-445c-9b1f-75d94abbf5ff" -e rgname=atDashboardTestRG3 `


### To debug use -vvv

`ansible-playbook deploy.yaml -e env=dev -e dashboardname=devdashansible002 -e deployname=atansibledeployment010 -e subscriptionId="bfba7d97-7864-445c-9b1f-75d94abbf5ff" -e rgname=atDashboardTestRG3 -vvv`

### Added AZCollection in the main.yaml. To run playbook

`ansible-playbook deploy.yaml -e env=dev -e dashboardname=devdashazcoll002 -e deployname=devdashazdeployment010 -e subscriptionId="bfba7d97-7864-445c-9b1f-75d94abbf5ff" -e rgname="atDashboardTestRG4" -e location="australiaeast" -vvv`
