# Run Appium tests on iOS devices using self-hosted Azure DevOps Pipelines

This repository contains a sample Azure DevOps Pipeline which runs Appium tests
on real, physical iOS devices which you host on-premise.

This repository is configured to use Raspberry Pi 3 devices as the build agent,
but you can use any machine capable of running the Azure Pipeline Agent and
Docker.

## Setting up your Azure DevOps Agent

1. [Create a self-hosted agent](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/agents?view=azure-devops&tabs=browser#install)
2. Install `usbmuxd`: `apt-get install -y usbmuxd libimobiledevice-utils`
3. Install Docker: `apt-get install -y docker.io`