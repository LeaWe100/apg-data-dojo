# Manage Configurations and Credentials

How do we configure our workflows or applications?
How do we store credentials and secrets?

In this session we consider common scenarios to discuss
configuration management.

## Learning goals

* Learn about different options to manage configurations
* Learn about best practices

## Session Outline

### Warmup

In your team:
* Discuss the differences (and similarities) between
  * Data
  * Code
  * Configuration
* How would do you define *config*?
* Share how you manage configurations in your projects.
* Share how you treat secrets.

Identify and document scenarios or use cases that are
relevant in your context and formulate requirements regarding
configuration management.


### Do

#### Introductory Reading

We need to agree on a suitable definition of *config*.

Read and discuss this outline of best practices: [12factor.net/config](https://12factor.net/config).

Tasks:
- [ ] Define *config* in your own words.
- [ ] Give example of *config* in your projecs.
- [ ] Reflect how your treatment of config relates to t above article.

#### Learning from Tools

Tools often try to implement best practices or provide pragmatic
solutions to common problem.

One such tool is [dynaconf](https://www.dynaconf.com/), which
is a configuration management tool for Python.

**While it is a Python-tool, the principles discussed therein are not Python-specific.**

Tasks:
- [ ] Describe how you store configuration in you project.
- [ ] If you do not already use a tool, contrast your approach
  with an approach suggested by a tool, for example dynaconf from
  above.

#### Checklist

Consider the following scenarios and provide solutions:
- [ ] Alice and Bob work on the same project using Git.
  * Alice's data is located at `/home/data/coolproject/`
  * Bob's data is located at `C:\Users\Bob\Desktop\test1`
  * How can they implement data access without interference?
- [ ] You work on a fairly large data set that make interactive
  development cumbersome. Therefore, you created a small subsample
  that is easier to work with. How can you easily direct your entire workflow to either use the small or the large data set?
- [ ] To access an internal database or API, you need save the
  credentials. How do you do that?
- [ ] You work on an application. There are different *users*
  depending on the deployment environment. These users have
  different credentials. How do you manage these credentials?

### Reflect

* If you were to make your codebases public now, would you compromise
  any credentials?
* Have you encountered situations where it was convenient to that
  the configuration is part of the code? Explain and reflect.

## Optional: Follow Up

Ideas:
* Require strict separation of config from code in one of your
  projects and use a tool to facilitate the process.
