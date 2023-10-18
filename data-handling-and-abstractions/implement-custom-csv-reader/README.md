# Implement a custom CSV reader

Data may come all in shapes and sizes, requiring us to build custom
readers and pipelines to make the information available to for further processing.

![](../_resources/base-workflow-highlight-import.png)

In this session we use a relatively simple text file from the
[HISTALP](../../resources/HISTALP/README.md) data set to discuss the
process of building a custom CSV reader.

## Learning goals

* Design and implement a reader function that takes a file path
  and returns a suitable data structure
* Discuss different approaches to dealing with data and meta-data

## Session Outline

### Warmup

In your team:
* Share how you usually read text and or CSV files.

Take a look at the data file and devise a strategy to process
its content.

Agree on the output of your reader function:
* What kind of data structure will you use?
* Which data will it include?
* How will you represent the data?

### Do

Tasks:
- [ ] Implement the reader function
- [ ] Provide documentation

### Reflect

* Did you implement different readers for different parameters? Explain.
* How are the data and the meta-data related and how did
  you model this relationship?
* How custom-made is your custom reader?
  * Did you re-use existing tools?
* How would you share your reader with your colleagues?
* How did you verify that it works?
* How would you *save* this data?
  * Does your way of saving the data simplify the process of reading it?
* How does the output of your reader look like, is it *tidy*?

## Optional: Follow Up

Ideas:
* Find a better way to represent the same information.
* Devise a *write* function to save your loaded data structure.
