---
layout: post
title: "LifeGuard Robotics"
description: ""
category: projects
tags: []
comments : false
---
{% include JB/setup %}


<img src="{{site.url}}/images/smallerboat.png" alt="LifeGuard Robotics Boat" style="width: 250px;" align="right"/>
As a member of the Autonomous Lifeguard Group I helped develope a system that provides rapid support to distressed swimmers. It is composed of two sub-systems: a command center, which will locate the swimmer, and an autonomous water vessel, which will navigate to the swimmer. The command center is an encoded tripod with a mounted scope that will be located on a Lifeguard’s post. A Lifeguard will center the scope on a distressed swimmer and at the push of a button, the GPS location of the swimmer will be wirelessly sent to the vessel. The vessel, docked in open water, will navigate to the swimmer upon recieving this information. Once the location is reached, the swimmer will grab hold of the vessel and await the arrival of a Lifeguard.


## My contributions

My work on this project was composed of multiple parts. 

* Xbee/Zigbee Communication
* Circuit Board Building/Testing
* GANTT Chart Supervisor
* Sonar

#### Wireless

Our two system approach required the command center to be in constant communication with the life boat. At any one point the life boat could be 300 to 1000 feet away from the command center which meant a robust wireless communication system must be implemented. 

Due to our expereince and knowledge of the Zigbee / Xbee system a decision was made to use the Xbee as our means of communication.

We quickly discovered however that the built in Xbee framework was not sustaniable. It did not allow us the low level communication we desired. Due to this we turned to an open source protocol, [Mavlink](https://github.com/mavlink/mavlink).

Based on this new framework we were able to properly communicate between the two systems. Including getting Acknowledgement messages when requiered. We were able to maintain communication reliably up to 1500 feet as long as line of sight was maintained.

#### Circuit board


<img src="https://users.soe.ucsc.edu/~jash/lib/exe/fetch.php?media=boat_io_boad.jpg" alt="LifeGuard Robotics Boat" style="width: 250px;" align="right"/>
Our system relied on the accurate connection of many sensors, and therefore it was quickly decided that a printed circuit board(PCB) would be requiered. Due to my expereince with the CNC board mill it was decided that I should build and test many of our two layer board designs. Along with my team-mate Shehadeh, we set out to build our circuit boards in eagle.

#### GANTT Chart and Waterfall Method

It was emphasised by our professor that we utilize a waterfall method since our projet was so long and complex. I therefore took it upon myself to develop a GANTT chart that contained all of the tasks that needed to be completed, and the estimated time they were estimated to take. 

Once a week we sat down with the professor and updated our chart to show the progress we had made and how we would catch up where we needed to. Although at first the team and I did not like the idea of the GANTT chart. By the end of the project we had all seen its benefits. 

#### Sonar

Our project attempted to use a sonar sensor to detect when we were within the presence of a drowning victim. Many tests were done with the device, including distance, accuracy, water proofing. 


## Presentations

## Posters

## Papers
For more information please see our final paper:

[Senior Design Final Report](https://users.soe.ucsc.edu/~jash/lib/exe/fetch.php?media=spring_sdp_final_report.pdf)
