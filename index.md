<!--
SPDX-FileCopyrightText: The SWAP-IT Contributors
SPDX-License-Identifier: CC-BY-4.0
-->
<style>body {text-align: justify}</style>
# **»SWAP-IT«: Innovative production architecture for the factory of the future**
In today's dynamic and demanding global marketplace, manufacturing companies are challenged to create customized and cost-effective products. In the face of increasing market volatility, these companies must not only be flexible, but also guarantee on-time delivery, high product quality and complete traceability. To meet these complex requirements, the interdisciplinary Fraunhofer consortium of ten different institutes offers innovative software and hardware solutions that include advanced approaches to production control and organization, component handling, quality assurance, and traceability.
<br /><br />
<center>
<iframe width="100%" height="625" src="https://www.youtube.com/embed/BqtzeEOSPfs?cc_load_policy=1" style="box-shadow: 0px 5px 5px gray" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>
<br />
## **The »SWAP-IT« Architecture**
The »[SWAP-IT](https://ieeexplore.ieee.org/document/9926665)« architecture was developed as part of the Fraunhofer lighthouse project »[SWAP-IT](https://www.produktion.fraunhofer.de/de/forschung-im-verbund/formate/leitprojekte/swap.html)«.
This new technological concept makes it possible to implement the production of tomorrow by transforming rigid production environments with individual processing stations into flexible and dynamic production environments.
The core of this innovation is a modular cyber-physical production system (CPPS) that efficiently integrates centralized and decentralized elements as a network of software and mechanical components.
The modules are specially designed to adapt seamlessly to different production environments and can be further developed with minimal effort.
SWAP distinguishes between base modules, which are available for all use cases, and use case-specific modules.
A base module, such as the registry module, provides ways to register machines and services to make them available.
Use case-specific modules are highly dependent on the problem domain and may include modules for specific services or provide optimization through use case-specific heuristics. 
<br />

<center>
    <img src="assets/img/swap-overview.svg" alt="drawing" width="70%"/>
</center>
<br />
  
Another innovation is the introduction of the »Production Flow Description Language« ([PFDL](https://ieeexplore.ieee.org/document/10003953)) which is also one of the base modules.
This specially developed domain-specific language enables production orders to act as active participants in the CPPS and to organize themselves independently.
The »PFDL« defines the basic sequence of work steps, but not which machine performs which task.
As a consequence, the »SWAP-IT« software decides how exactly the order should be executed and assigns individual tasks to machines that are currently available or conveniently located.
In this way, each order is executed individually and efficiently according to specifications, creating an order-centered and highly automated production environment.
This case-by-case flexibility is not possible in traditional manufacturing with its standardized workstations.

With the help of these basic software components the precise definition and execution of production orders is possible.
The use of the »SWAP-IT» architecture in combination with the »PFDL« enables fully automated and machine-readable production orders. This facilitates dynamic and efficient allocation of production resources, such as through the OPC UA-based connection of machine tools and production systems, and allows for immediate reaction during the production process.

<div class="wrapper">
    <div class="box sidebar">
    
    <div class="click-zoom">
  <label>
    <input type="checkbox">
    <img src="assets/img/swap_architecture.jpg" style="box-shadow: 10px 5px 5px gray;" alt="drawing" width="100%"/>
  </label>
</div>
    </div>
    <div class="box sidebar2"><iframe style="box-shadow: 10px 5px 5px gray;" width="100%" height="455" src="https://www.youtube.com/embed/bdl0mfd_s7k?cc_load_policy=1" frameborder="0" allowfullscreen></iframe></div>
</div>


<br />

## **New solutions for flexible, cooperative, and efficient scheduling of production resources at the runtime of the production order**
»SWAP-IT« and its modules are being used for the first time in four industry-relevant use cases with hardware demonstrators.
The project has developed basic and specific technology software components.
The basic software components and an [integration guide](https://github.com/iml130/swap-it-integration-guide) are freely available as open source on GitHub and are being used in initial heterogeneous use cases in the context of production and automation.

Production resources can automate processes to increase technical flexibility and handle a wide range of product variants.
This can be imagined as an »automation of the automation«.
Here, self-configuring algorithms are used for robot-based object handling to improve component flexibility.
Among other things, three new types of sensors for optical quality assurance have been integrated.
These sensors use holography and pattern projection to enable surface form measurement with micrometer accuracy, local measurement of defects and functional surfaces (digital holography), as well as mark-free identification of components using track & trace by means of the component's fingerprint.
The process achieves a wide range of variants by integrating the »SWAP-IT« architecture to increase organizational flexibility and optimize capacity utilization.
Workstations can be flexibly linked using freely navigating driverless transport vehicles to achieve an order-specific material flow.
AI-supported optimization algorithms enable optimal distribution of the workload across production resources, resulting in a short throughput time.
 
The configurations and applications available on GitHub allow for a lightweight start in »SWAP-IT« without any external dependencies.
To provide a simple introduction, the developments have been combined into a virtual use case for demonstration purposes.
This demonstration scenario features the latest developed software modules like a dashboard for visualization and creation of orders.
The example production scenario produces an industrial traffic light.
In this context, user can configure the composition of lights and the number of light segments.
Besides, the user can choose between multiple shapes for the stand segment of the traffic light.
Next to this simple example scenario, four use cases were already implemented and are introduced as [success stories](success-stories.md). 
 
## **Interfaces in OPC UA**

Highly flexible production systems can be implemented to cost-effectively manufacture customized products of the highest quality.
The interfaces are implemented using the established OPC CA standard to keep the entry barrier low for interested companies.
Open source software modules are available to simulate the functionality of the interface, measurement, and detection systems.
Companies can simulate and test integration without incurring external costs using
the software modules provided in this open source publication.
The modules include basic software that operates on common »SWAP-IT« models, as well as technology-specific modules from industrial use cases, such as measurement and detection systems.
Together, these modules enable simple piloting and simulation without external costs.

## **»SWAP-IT« Ecosystem and ready to use Components**

### Base Modules

- [Production Flow Description Language (PFDL)](https://github.com/iml130/pfdl) @ GitHub
  - [PFDL VS Code Extension](https://github.com/iml130/pfdl-vscode-extension)

### Tech Modules
- [Digital Holography](https://github.com/ipm-pk/digital-holography)
- [Fingerprint](https://github.com/ipm-pk/fingerprint)
- More modules are in preparation and will follow soon.

### Succes Stories
- [Demonstration Scenario](https://github.com/swap-it/swap-it-demo-scenario)

## **Where else to find »SWAP-IT«?**

### Upcoming

- **[Industry Workshop 2024](https://www.iwu.fraunhofer.de/de/veranstaltungen-und-messen/tagungen-und-workshops/industrieworkshop-swap.html)**
  - September 26, 2024, Dresden (Germany)
  - Industrial workshop in Dresden featuring presentations on results and industry feedback, along with live demonstrations of interconnected manufacturing units. The workshop includes practical sessions offering deep insights into project solutions and discussions on adapting the SWAP-IT architecture to various industrial requirements.

### Past

- **[Hannover Messe Industry (HMI)](https://www.fraunhofer.de/en/events/fraunhofer-at-trade-fairs/2023/hannover-messe-2023.html)**
  - World's largest trade fair, dedicated to the topic of industry development
  - April 17, 2023  -  April 21, 2023, Hannover (Germany)
  - Booth A12, Hall 16

- **[Control 2024](https://www.vision.fraunhofer.de/de/veranstaltungen/messe/control/fraunhofer-vision-control-2024/swap-roboterteams-produktionsarchitekturen.html)**
  - Control International trade fair for quality assurance
  - April 23, 2024  -  April 26, 2024, Stuttgart (Germany)
  - Booth 8201 / Hall 8
