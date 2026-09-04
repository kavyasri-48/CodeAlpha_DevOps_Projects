# CodeAlpha Jenkins Remoting Project

## Overview

This project demonstrates the **Jenkins Controller-Agent architecture using Jenkins Remoting**.

A Jenkins Controller manages and schedules build jobs, while a remote Linux Agent executes the assigned build tasks. The project demonstrates remote build execution using a Linux-based Jenkins Agent.

## Architecture

```text
Jenkins Controller
        |
        | Jenkins Remoting
        v
Linux Agent (linux-agent)
        |
        +-- Executor 0
        |
        +-- Executor 1
```

## Technologies Used

* Jenkins
* Jenkins Remoting
* Jenkins Agents
* Jenkins Executors
* Java
* Linux / Ubuntu
* Git
* GitHub
* Shell

## Implementation

1. Installed Jenkins on Ubuntu.
2. Created a Jenkins Agent named `linux-agent`.
3. Configured the Linux Agent for remote build execution.
4. Connected the Agent to the Jenkins Controller using Jenkins Remoting.
5. Configured two executors on the Linux Agent.
6. Created Jenkins jobs restricted to the `linux-agent`.
7. Executed build jobs on the remote Linux Agent.
8. Verified successful builds through Jenkins Console Output.
9. Tested remote execution and agent connectivity.

## Jenkins Controller

The Jenkins Controller is responsible for:

* Managing Jenkins jobs
* Scheduling builds
* Managing connected agents
* Assigning build tasks to available executors
* Monitoring build results

## Jenkins Agent

The Linux Agent named `linux-agent` performs the build tasks assigned by the Jenkins Controller.

The Agent was configured with **two executors**, allowing it to execute multiple build tasks.

## Jenkins Remoting

**Jenkins Remoting** provides communication between the Jenkins Controller and remote Agents.

Through this communication, the Controller can assign build tasks to the Linux Agent, while the Agent executes the tasks and sends the build results back to the Controller.

## Build Execution Flow

```text
Jenkins Job
     |
     v
Jenkins Controller
     |
     | Jenkins Remoting
     v
linux-agent
     |
     v
Executor
     |
     v
Build Execution
     |
     v
Build Result
```

## Screenshots

### Jenkins Linux Agent

![Jenkins Linux Agent](screenshots/Jenkins%20Linux%20agent.png)

### Jenkins Remote Agent

![Jenkins Remote Agent 1](screenshots/Jenkins%20remote%20agent%201.png)

![Jenkins Remote Agent 2](screenshots/Jenkins%20remote%20agent%202.png)

### Jenkins Console Output

![Jenkins Console Output 1](screenshots/Jenkins%20console%20output%201.png)

![Jenkins Console Output 2](screenshots/Jenkins%20console%20output%202.png)

![Jenkins Console Output 3](screenshots/Jenkins%20console%20output%203.png)

### Jenkins Log

![Jenkins Log](screenshots/Jenkins%20Log.png)

## Result

The Jenkins Controller successfully distributed build jobs to the remote Linux Agent using Jenkins Remoting.

The builds were successfully executed on the `linux-agent`, and the results were verified through Jenkins Console Output.

## Key DevOps Concepts

* Jenkins Controller-Agent architecture
* Jenkins Remoting
* Remote build execution
* Distributed builds
* Jenkins Agents
* Jenkins Executors
* Node labels
* Job scheduling
* Build automation
* Linux-based build execution
* Git and GitHub

## Learning Outcome

This project provided hands-on experience with **Jenkins distributed build architecture**, remote Linux agents, executors, and Jenkins Remoting.

It demonstrates how Jenkins can distribute build workloads from a Controller to remote Agents for execution.

## Internship Project

**CodeAlpha — DevOps Internship**

**Project:** Jenkins Remoting

