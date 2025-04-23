---
title: Team Block Diagram, Sequence Diagram, and Message types
---

## 1) Team Block Diagram

Below is our connected team block diagram. It shows each individual block diagrams and then how all four will connect together physcially. The subsystems are chained togther with Divine's upstream of Andrey's, Andrey's upstream from Jacob's, Jacob's upstream from Jake's, and Jake's upstream from Divine's.

![diagram_01](Team_Block.png "Team block diagram")

### Reference -> Individual Block Diagrams

Linked Below is each team member's individual block diagrams

- [Andrey's Block Diagram](https://lordandrey17.github.io/andreypodoprigora.github.io/Personal-Block-Diagram/)
- [Divine's Block Diagram]()
- [Jacob's Block Diagram]()
- [Jake's Block Diagram](https://jakestrube.github.io/DataSheet/Individual_BlockDiagram/)

### Ribbon Cable Connector Structure

![diagram_015](Ribbon.png "Ribbon cable structure")

## 2) Sequence Diagram of Team Communication

Below is our sequence diagram of team communication. It visualizes all the messages that we will send across our subsytems and how each message will interact with every subsystem and the user inputs. 

![diagram_02](Comm.png "Sequence diagram")

## 3) Message Types

Below is a combination of diagrams describing different types of messages that are being sent between individual boards

![diagram_03](Mes_Str.png "Message types")






## Message protocol

| Message Type | Message ID (Char) | Andrey: Sensor ID: A | Jacob: Motor ID: W | Jake: HMI ID: S | Divine: MQTT ID: D|
|--------------|------------|----------------------|--------------------|-----------------|-------------------|
| Update motor speed | 4 | - | R: (Update speed at which motors move) | S: (HMI menu and button press) R:(Displayed on HMI) | S: (mqtt topic: /EGR314/TEAM204/MOTORSPEED) R: (mqtt topic: /EGR314/TEAM204/MOTORSPEED)|
| Update following distance | 5 | R: (update distance sensor wants to keep) | - | SS: (HMI menu and button press) R:(Displayed on HMI) | S: (mqtt topic: /EGR314/TEAM204/DISTANCE) R: (mqtt topic: /EGR314/TEAM204/DISTANCE) |


