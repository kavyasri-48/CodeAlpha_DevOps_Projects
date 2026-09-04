# CodeAlpha Jenkins Remoting Project

## Overview

This project demonstrates the **Jenkins Controller-Agent architecture using Jenkins Remoting**.

A Jenkins Controller distributes build jobs to a remote Linux Agent for execution. The Linux Agent performs the assigned builds using configured executors.

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
* Linux / Ubuntu
* Java
* Jenkins Agents
* Jenkins Executors
* Git
* GitHub

## Implementation

1. Installed Jenkins on Ubuntu.
2. Created a Jenkins Agent named `linux-agent`.
3. Configured the agent for remote build execution.
4. Connected the Linux Agent to the Jenkins Controller using Jenkins Remoting.
5. Created jobs restricted to the `linux-agent`.
6. Successfully executed builds on the remote agent.
7. Configured two executors on the agent.
8. Tested multiple jobs on the agent.

## Jenkins Controller

The Jenkins Controller is responsible for managing jobs, scheduling builds, and assigning work to connected agents.

## Jenkins Agent

The Linux Agent named `linux-agent` performs build tasks assigned by the Jenkins Controller.

The agent was configured with **two executors**, allowing it to execute multiple jobs concurrently.

## Jenkins Remoting

Jenkins Remoting enables communication between the Jenkins Controller and remote agents.

The Controller uses this communication to send build tasks to the Linux Agent, while the Agent executes those tasks and reports the results back to the Controller.

## Result

The Jenkins Controller successfully distributed jobs to the Linux Agent using Jenkins Remoting.

Both test jobs completed successfully on the remote Linux Agent.

## Key DevOps Concepts

* Controller-Agent architecture
* Jenkins Remoting
* Distributed builds
* Remote execution
* Node labels
* Executors
* Build automation
* Jenkins Agents
* Job scheduling
* Linux-based build execution

## Learning Outcome

This project provided hands-on experience with Jenkins distributed build architecture and demonstrated how build workloads can be executed on remote Linux agents.

## Internship Project

**CodeAlpha — Jenkins Remoting Project**

