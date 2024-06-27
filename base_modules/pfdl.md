### **Production Flow Description Language**
The Production Flow Description Language (PFDL) is a powerful tool used in the realm of manufacturing and production management.
It serves as a standardized language for describing and documenting the various steps and processes involved in manufacturing a product.
A PFDL program corresponds to a single ordered product and specifies the production steps involved.
It also serves as an input for an order controlled production, which can process it automatically.
A PFDL program consists of structs and tasks, allowing for the definition of runtime aspects such as loops, conditions, and synchronization.

PFDL offers a structured and systematic approach to defining the production flow.
It allows manufacturers to break down the entire production process into individual tasks and sequences, providing a clear and comprehensive representation of how the product is made.
Within a PFDL program, manufacturers can define different aspects of the production flow such as task dependencies, parallel execution, loops, conditions, and synchronization. 
This flexibility enables the creation of complex and dynamic production flows that accurately reflect real-world manufacturing scenarios.
Overall, PFDL plays a crucial role in enhancing the understanding, communication, and automation of manufacturing processes, ultimately leading to improved productivity, quality, and efficiency in the production environment.


#### PFDL Scheduler
The PFDL itself is just the description language and needs to be parsed, validated, and transformed into a structure to control the production process.
All of these functionalities is done by the so-called PFDL Scheduler.
The scheduler parses and validates PFDL files, which are then transformed into a domain model, which is a representation of the production order as a python object.
This model can then be used to generate a petri net, which is used to control the production by triggering events and receivve events, e.g. when a service has finished.
To enable this, the PFDL provides interfaces in both directions enabling a process control that makes use of generated PFDLs and keep track of the current state of the execution.

#### **PFDL VS Code Extension**
To support the development of PFDL programs in [Visual Studio Code](https://code.visualstudio.com/), an extension has been developed that provides features such as syntax and error highlighting, code completion, and visualization of the PFDL code as a Petri net.
These features increase integration speed and enable a deeper understanding of the implemented process flow by observing the generated petri net.
<br /><br />
<center>
<img src="assets/img/pfdl_vs_code_extension.png" style="box-shadow: 10px 5px 5px gray;" width="70%" alt="drawing"/>
</center>
<br />

The extension generates a graphical representation of the PFDL program and provides a dynamic webview for development purposes. The visualization can be displayed alongside the PFDL program and is updated reactively. You can choose the orientation of the graph, either horizontal or vertical, for convenience. The nodes in the graph can be moved, but overlapping is not allowed. Labels for individual nodes are hidden by default and only shown when the mouse is over them. Box labels can also be hidden. As the PFDL program becomes more complex, collapsing large components into a single one can be helpful. Within the webview, you can select specific components to collapse or collapse all at once. Expanding nodes is done accordingly. When a PFDL program is open in the active text editor in VS Code, two buttons appear in the top right corner. "Visualize Code" displays the graph visualization of the PFDL program, and "Download PNG" saves the graph as a .png file. The graph is always updated when the PFDL program is saved. Error messages are displayed if there are any errors in the file.