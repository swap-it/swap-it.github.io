<!--
SPDX-FileCopyrightText: The SWAP-IT Contributors
SPDX-License-Identifier: CC-BY-4.0
-->
# **Glossary**

### Execution Engine
The Execution Engine (EE) provides an interface that connects the PFDL Scheduler to the Field Level Devices.

### Field Device
The Field level constitutes the lowest level of the automation pyramid and captures all kind of devices that are found in industrial manufacturing systems.
These devices are either sensors or actors and directly influence processes by measuring data or performing an arbitrary step of a manufacturing process.

### Production Flow Description Language
The Production Flow Description Language (PFDL) is a domain specific that defines the basic sequence of work steps without choosing which machine performs which task.
PFDL files are getting parsed by the PFDL Scheduler which controls the production order and the execution of services.

### PFDL Scheduler
The PFDL scheduler comprises almost the complete execution of a production order including the parsing of the PFDL description, model creation and validation and execution of the petri net.
It interacts with the execution engines and informs them about services or tasks which started or finished.

