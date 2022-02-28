# bcfOWL-testdata
The data in this repository is part of a research project on the organisation of federated construction projecst, with a focus on issue communication with the BIM Collaboration Format (BCF). In this research, project stakeholders maintain their own contributions to the project, and link to those of other stakeholders using [Linked Data](https://www.w3.org/DesignIssues/LinkedData.html). To organise this project, we make use of the Web specifications provided by the [Solid Project](https://solidproject.org/). 

## Setup
This repository contains a sample project, based on a BIM model of the Design Computation Chair at RWTH Aachen University. In this example, three office-related Solid Pods were set up, on three different instances of the [Solid Community Server](https://github.com/solid/community-server), an open source implementation of the Solid specifications. On each Solid server, one or more "employee pods" were created, who interact with the project.

* Server 1 (PORT: 3000, startup: npm run start:server_architect):
  * Architecture office (/office)
  * Employee 1 (/oliver)  
  * Employee 2 (/jeroen) 

* Server 2 (PORT: 3001, startup: npm run start:server_hvac)
  * HVAC office (/hvac-office)
  * Employee 1 (/jyrki)

* Server 3 (PORT: 3002, startup: npm run start:server_structure)
  * Structural Engineering Office (/structure-office)
  * Employee 1 (/jakob)

A sample project has been created (id: 8b71315b-7db2-4b35-a1e9-fcddaf8556f5), containing pointers to the project locations of the stakeholders in the project. This discovery-oriented architecture bases upon the data patterns of the LBDserver project [Werbrouck et al., 2022](http://www.semantic-web-journal.net/content/lbdserver-federated-ecosystem-heterogeneous-linked-building-data). Each