---
layout: project
type: project
image: img/customer/customer.jpeg
title: "Customer Queue"
date: 2023-4-12
published: true
labels:
  - Java
summary: "Java code creates a Customer class for simulating a system with arrival and service times, allowing chronological sorting and organization of customer objects."
---

This defines a class named "Customer" aiming to simulate a customer system, potentially for a queuing or service-oriented scenario. Each instance of the "Customer" class represents an individual customer and holds attributes such as "arrivalTime" and "serviceTime," signifying when a customer arrives and how long they require service. The constructor initializes these attributes randomly using the "Random" class, introducing variability into the simulation. Notably, the class implements the "Comparable" interface and overrides its "compareTo" method to enable comparison of "Customer" objects based on their "arrivalTime." This suggests a focus on organizing or sorting customers chronologically. 

<hr>
<pre>
	for(int i = 0; i < cashiers.length; i++) {
		if(currentTime >= cashiers[i]) {
			// Single queue implementation
			if(singleQueue) {
				if(queues[0].isEmpty()) continue;
				Customer nextCustomer = queues[0].poll();
				customersHelped++;
				cashiers[i] = currentTime + nextCustomer.serviceTime;
				totalWaitingTime += currentTime - nextCustomer.arrivalTime;
			}
			// Multiple queue implementation
			else {
				if(queues[i].isEmpty()) continue;
				Customer nextCustomer = queues[i].poll();
				customersHelped++;
				cashiers[i] = currentTime + nextCustomer.serviceTime;
				totalWaitingTime += currentTime - nextCustomer.arrivalTime;
			}
		}
	}
</pre>
<hr>
			
## Reflection
This assignment provided a fundamental framework for the simulation and management of a system involving a variety of arriving customers with processing needs, while also enabling chronological sorting for analytical insights. By working through this task, I not only deepened my understanding of Java programming concepts and techniques but also honed my problem-solving skills, which I'm eager to apply in future projects.
