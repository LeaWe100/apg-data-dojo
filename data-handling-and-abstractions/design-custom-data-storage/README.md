# Design custom data storage

How you store your data can have a lasting influence the evolution of your project.

![](../_resources/base-workflow-highlight-import.png)

In this session we design a data storage solution for
the a relatively simple collection of data sets, namely the [HISTALP](../../resources/HISTALP/README.md)
data set to contrast different approaches.


## Learning goals

* Design a data storage solution for a given data set
* Contrast and compare this storage solution to other approaches
* Optional: implement the storage solution

## Session Outline

### Warmup

In your team:
* Do you have control over how raw/input data is stored in your project?
* Who is responsible for data management and what kind of requirements are at play?
* If you have designed a data store, share your experience.

Take a look at the data set and discuss its properties.
Make a sketch to visualize (!) relationships.

Change the perspective and put yourself in the role of a user:
* How might a user want to analyze the data?
* How can you provide the data in a way that it is easy to use?

### Do

Consider the following requirements:
* The data may change
* Not all parameters are available for all stations
* In our case the data is very small, consider the case that the data may be quite large as well

Tasks:
- [ ] Identify different options on how you can persists the data
- [ ] Discuss pros and cons of these approaches.
- [ ] Decide on the one approach that you consider *best* and work out the details
  - [ ] Explain your choice
- [ ] Document your findings

### Reflect

* Do you think your solution will be easy/difficult to *use*?
* How much does the user have to know about the implementation of your store?
  * To what extend will a change in your storage system affect the user?
  * How can provide access to your storage system in such a way that the
    user stays blissfully ignorant of any changes you might introduce in
    your storage system?
* Do you think your solution will be easy/difficult to *maintain*?
* How did you agree on benefits and tradeoffs?

## Optional: Follow Up

Ideas:
* Implement the data store you came up with.
* Introduce a layer that isolates the user from the
  implementation details of your store.