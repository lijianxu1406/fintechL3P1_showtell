# fintechL3P1_showtell
Project for Fintech L3 P1 show-tell presentation

## Objective of the DevOps project: 
* To automate a series of workflow that executed itself when users triggered a git push / pull_request; stimulating a CI/CD pipeline in DevOps.
* To familiarise with Github workflow. 

## Workflow Structure
![Current Workflow](./images/currentworkflow.png)

### 1. **Deployment of Static Pages via Github Pages [static.yml]**
From the course, static pages deployment can be achieved simply from Github Pages Tabs under Setting from Github.
![gitpage](./images/gitpage.png)

Similarly, Github Actions to deploy a static page can be done through a .yml file under .github/workflows folder; which was the method used in this project. 
![pagebuilddeployment](./images/pagebuilddeployment.png)
A git push / pull request will trigger the automatic deployment of static pages which can be found under the link: https://lijianxu1406.github.io/fintechL3P1_showtell/
![link](./images/link.png)

Issue faced: If Github Pages are implemented before the creation of index.html file or lack of index.html file, the static page deployed will be based on the readme.md file. This can be rectify through the naming of the desired webpage-to-be-displayed to index.html. 

### 2. **Slack Notification on committed changes**
![slack](./images/slack.png)
A slack.yml are used to trigger a notification message to be sent to the owner’s slack upon commited change.
![notification](./images/notification.png)
This exercise introduces the use of Github Secret in storing and encrypting privacy data that user do not wish to share to the public. At the same time, it serves to introduce the importance of having consistent indentation in formatting .yml file. 
