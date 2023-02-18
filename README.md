# Producer-Consumer-Simulation-Program
+ A project generated by Angular CLI version 14.2.10 for frontend and Springboot version 3.0.2 for backend.
## Project Overview
## Design patterns applied
1. **Concurrency: “ Producer/Consumer DP”**
* Each machine runs on a separate thread consuming products from a queue such that if the queue is empty, it waits, otherwise it takes a product from the queue and processes it for its service time.
2. **Observer:**
* Each machine is an observer which observes the queues -observable- it consumes its products from.
* When the queue is empty, it registers itself to the queue as an observer and waits for notification.
* When the queue contains elements, it notifies its observers so they can consume them.
4. **Snapshot:**
* System keeps states of its machines and queues once updated so we can replay the whole simulation again.
* A Memento class saves the state of the machine and the queue.
* An Originator class to save the states.
* A CareTaker class to retrieve the state.
6. **Singleton:**
* CareTaker class implements singleton to have only one instance of it.
## Model-View-Controller(MVC)
## UML class diagram
## User manual to run the code
+ In **cmd** cd to **backend folder** and run ./mvnw spring-boot: run or by opening the folder with java IDE then run the main file ProducerConsumerApplication.java
+ Open **frontend folder** and open new terminal then type **ng serve** and navigate to this link http://localhost:4200/
## Program UI
## User Guide
