<!--
SPDX-FileCopyrightText: The SWAP-IT Contributors
SPDX-License-Identifier: CC-BY-4.0
-->
# **Glossary**

### Assignment Agent
Entity that interacts with an Execution Engine and a Device Registry to assign a service to one concrete resource out of a set of possible resources.

### Device Registry
Registry Module where resource OPC UA server, representing field level devices, can register themsel and thus, make themself available to execute PFDL services.
In Addition, the Device Registry has a build-in functionality to filter suitable resources for a service execution based on a resource's capabilities.

### Execution Engine
Interface between the PFDL scheduler and field level resources that executes the scheduled services on the field level.
In addition, it handles the parameter flow between services and tasks.

### OPC UA Information Model
Contains all nodes and references to map a specific entity to an OPC UA server.

### Field Device
The Field level constitutes the lowest level of the automation pyramid and captures all kind of devices that are found in industrial manufacturing systems.
These devices are either sensors or actors and directly influence processes by measuring data or performing an arbitrary step of a manufacturing process.

### Production Flow Description Language
The Production Flow Description Language (PFDL) is a domain specific language that defines the basic sequence of work steps without choosing which machine performs which task.
PFDL files are getting parsed by the PFDL Scheduler which controls the production order and the execution of services.

### PFDL Scheduler
The PFDL scheduler comprises almost the complete execution of a production order including the parsing of the PFDL description, model creation and validation and execution of the petri net.
It interacts with the execution engine and informs it about services or tasks which started or finished.

###  Process Agent
Agent consisting of a PFDL scheduler and an Execution Engine.
It drives the execution of the process specified within a PFDL.