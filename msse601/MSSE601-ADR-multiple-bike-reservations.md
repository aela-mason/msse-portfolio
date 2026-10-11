#### Aela Mason 

#### MSSE601_X40 Software Engineer Fundamentals 

#### Portfolio Decision Record 

#### 10/11/2026 

 

## Context 

The week six assignment provided several examples of edge cases. In addition to our own generated list, we wanted to look at these provided ones to determine if they were applicable to our system. One that required additional discussion was “a reservation covering multiple bikes”. While our system had been designed with heavy bike rental functionality, this was something we hadn’t nailed down yet. We felt that reservations were important to support, but multiple bikes in a single reservation posed significant questions in regard to our existing screens and structure. 

## Options 

Two straightforward options came out of this discussion. 

* Option 1: In alignment with the assignment description, allow reservations to contain multiple bikes. This would require a temporary storage entity to hold onto individual bikes that had been placed into a pending reservation and functionality around how long the entire reservation process was allowed to take so that we would know when to release pending bikes. 

* Option 2: Going against the examples in the assignment description but more in line with our existing screens, only allow one bike per reservation. This would require only the addition of basic reservation functionality. 

## Decision 

After significant back and forth, we decided to go with Option 2. 

## Reasoning 

This entire project is heavily constrained by both timeline and budget. Our Project Charter laid out an eight-week, $65,000 expectation for development, and the Golden Bike Shop is a small, locally owned business. The original requirements and screens didn’t account for multiple-bike reservation functionality, and it is non-negligible in how it would impact the existing structure. 

A consistent theme to the decisions we made as a team during each project component was to maximize simplicity and consistency. It impacted our decisions around requirements, overall architecture, and our UI. It was important to us that data design not be an exception. 

## Consequences 

This was one of the most difficult decisions we needed to make during the course simply because of its impact on customer interactions. Potential use cases for multiple bikes in a reservation are: 

* Group or family reservations with single payers. 

* Packages or bundled rentals, including cases where the Golden Bike Shop may want to give a bundled or bulk rental discount. 

We can absolutely see how this decision would result in added friction in customer transactions with rental employees. Customers are still able to reserve multiple bikes; they just have to do so in multiple reservations. This shouldn’t result in lost reservations due to those reservations being impossible, but could result in lost reservations if customers deem the process to be too difficult or prohibitive. 

We stand by this decision given the constraints of the project. However, if the Golden Bike Shop were to place a high priority on group bike rentals, we would be willing to revisit it and we have a rough solution designed for it. 

## Additional Notes 

This decision was made as part of the week six project component, Data Design. The decision itself is summarized in the Decision Record on that document, but its impact is primarily seen in the entity-relationship diagram and the corresponding table descriptions. 

No AI was used in this decision. We did surface an additional missing piece around rental bike pricing during the week’s interactions with AI, and we adapted our entities/tables to fill that gap. 

The flow of this decision was that one of my team members included multiple-bike reservations because of its presence in the assignment description. I pushed back against it since it didn’t fit with the way we had designed things in previous weeks, and the discussion happened from there. 
