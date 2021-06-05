# AlaskanAirlines
An implementation of a data model for flight analytics.

## Assumptions
A few assumptions were made here, in order to reduce the solution space:
1. There is a way to determine and differentiate unique guests. This is important for determining the number of attempts a guest makes at searching non-existing flights.
2. 
## Implementation
I designed an ERD to demonstrate how I would model the data. Attached as well is a design of the physical architecture I would use for it. Since it is real time, and high velocity and volume, I would use a publisher/subscriber pattern, which is detailed below. To show how the data structure could be used to answer the primary question, I implemented a simple decision tree. The goal of the challenge isn't to design a machine learning model, as that would take more time and testing. It is to create a model suitable for handling such tasks, which is why the decision tree model is created, but not finely tuned/pruned.
