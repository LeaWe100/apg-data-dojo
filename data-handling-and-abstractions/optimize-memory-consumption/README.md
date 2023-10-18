# Optimize Memory Consumption

Our ability to conveniently and interactively work with data can be
hampered by the size of the data we wish to process.

Choosing suitable data types can help reduce the memory (RAM) consumption
of our data structures and decrease computation time.
If data types are not explicitly stated, tools usually opt for a defensive
way to represent data by using a larger type.

## Learning goals

* Understand the relative sizes of common data types.
* Know how the memory footprint of a dataframe be reduced by using appropriate the types.

## Session Outline

### Warmup

In your team:
* Share which data types you know about (and how the are represented *internally*).
* Do you usually care about the memory footprint of your data structures?
* Do you sometimes reduce the size of the data structure?

Identify a few common data types (or variable types) that you want to focus on.


### Do

For the data types that are relevant to you, answer the following questions:
- [ ] How can their size be reduced? We call this process *downcasting*.
- [ ] Under which circumstances is it safe to do so?
- [ ] How can you verify that it is indeed safe to do so?

Tasks:
- [ ] Create some sample data
- [ ] Create a new object where you reduce the data types according to your guidelines from above
- [ ] Compare the memory consumption of both objects


Notes:
* Wikipedia has an article on [type conversion](https://en.wikipedia.org/wiki/Type_conversion)


### Reflect

* What benefits to you see in choosing the appropriate data type?
* Once you have chosen the right data types, how can you persist them?
* How would you notice that your data type causes troubles?


## Optional: Follow up

Ideas:
* Are [data normalization](https://en.wikipedia.org/wiki/Database_normalization) and [wide and narrow data](https://en.wikipedia.org/wiki/Wide_and_narrow_data) related in any sense?
* What other options do you have if the data you wish to process just
  does not fit into you RAM? Make a list.
