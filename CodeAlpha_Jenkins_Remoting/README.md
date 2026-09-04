# Jenkins Remoting Project

## Overview

This project demonstrates Jenkins Controller-Agent architecture using Jenkins Remoting.

A Jenkins Controller distributes build jobs to a remote Linux Agent for execution.

## Architecture

Jenkins Controller
        |
        | Jenkins Remoting
        |
        v
Linux Agent (linux-agent)
        |
        +-- Executor 0
        |
        +-- Executor 1

## Technologies Used

- Jenkins
- Jenkins Remoting
- Linux / Ubuntu
- Java
- Jenkins Agents
- Jenkins Executors
- Git
- GitHub

## Implementation

1. Installed Jenkins on Ubuntu.
2. Created a Jenkins Agent named `linux-agent`.
3. Configured the agent for remote build execution.
4. Connected the agent to the Jenkins Controller.
5. Created jobs restricted to the `linux-agent`.
6. Successfully executed builds on the remote agent.
7. Configured two executors.
8. Tested multiple jobs on the agent.

## Result

The Jenkins Controller successfully distributed jobs to the Linux Agent using Jenkins Remoting.

Both test jobs completed successfully.

## Key DevOps Concepts

- Controller-Agent architecture
- Distributed builds
- Remote execution
- Node labels
- Executors
- Build automation
- Jenkins Remoting
