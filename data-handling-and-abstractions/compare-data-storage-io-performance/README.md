# Compare Data Storage Performance

When we [persist](https://en.wikipedia.org/wiki/Persistence_(computer_science)) data, we can ask
the at least the following questions:
* How long does it take to write the data?
* How large is the data on disk?
* How long does it take to read the data?

The answer to these questions may then, amongst other reasons, influence the choice of storage
option we follow through in our project.

## Learning goals

* Know about io-performance and disk-space characteristics of different storage options.
* Be able to make an informed decision regarding storage choice in projects.

## Session Outline

### Warmup

In your team:
* Share what you already know about the characteristics of the storages
  options you use in your projects.
* Discuss if/how the data types influence the characteristics.

Agree on a set of storage options you wish to compare a devise a strategy to do so.

### Do

For one or more data sets and two or more storage options.

Tasks:
- [ ] Measure read and write time
- [ ] Measure disk space
- [ ] Collect the data and present in an informative way
- [ ] Formulate a conclusion and derive recommendations based on your findings

### Reflect

* Did you observe differences depending on the machine where
  you performed the measurements? Explain.
* What other criteria are relevant when choosing a storage option?
* Do you know how much processing time in your pipelines is spend on
  IO in comparison to processing?
  * If not, how could you find out?
