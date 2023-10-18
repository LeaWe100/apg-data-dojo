# Try web APIs

In a business or application setting, a lot of data may be
accessed through a web API.

![](../_resources/base-workflow-highlight-import.png)

In this session we provide a starting point on how to
interact with a web API.
While a general introduction web APIs
is out of scope, it is useful to see how data
can to loaded (and queried) through such an API.

## Learning Goals

* See how a web API can be accessed through R/Python to query data
* Provide foundation for future learning

## Session Outline

### Warmup

In your team:
* Share what you know about web APIs and why they are useful.
* Do you have a web API in use?
* Based on your current experience, share use cases and applications
  for web APIs compared to direct data access.

Assuming that everyone is familiar with file-based data sources,
what are your personal experiences with working with web APIs?

Formulate a set of questions you wish to explore.

### Preparation and additional resources

#### Background reading

It is worth mentioning the following resources:
* [Wikipedia on Web API](https://en.wikipedia.org/wiki/Web_API)
* [Wikipedia on HTTP](https://en.wikipedia.org/wiki/HTTP)
* [Wikipedia on JSON](https://en.wikipedia.org/wiki/JSON)

#### A note on security

**Do not hard-code API credentials.**

(In the examples used later, no credentials are needed.)

#### Example APIs

We consider two different public APIs.

**[chucknorris.io](https://api.chucknorris.io/)** is a free API for hand curated Chuck Norris facts.

Tasks:
- [ ] Retrieve a random chuck joke through the browser
- [ ] Retrieve another random chuck joke through the browser

**[Fake Store API](https://fakestoreapi.com/)** is a free API that mimics a somewhat realistic e-commerce or shopping website prototype.

Tasks:
- [ ] Visit the site to get a feeling for the kind of data is provided through the API and how it can be accessed

If you have [curl](https://en.wikipedia.org/wiki/CURL) available on your system,
execute the queries through the command line as well.

While we are at it, do you know about [wget](https://en.wikipedia.org/wiki/Wget)?

### Do

Let's focus on the following scenario:
* A web API is given
* We wish to perform a given query
* We wish to execute the query through R/Python and obtain
  the result in a suitable format

If you are not sure which query to execute, try `GET https://api.chucknorris.io/jokes/random` to
collect yet another joke.

Tasks:
- [ ] Execute query and inspect the result
- [ ] Unpack the JSON response object if needed
- [ ] Inspect the response object and discuss its meaning

If you use R, see https://httr2.r-lib.org/articles/httr2.html.

If you use Python, see https://wesmckinney.com/book/accessing-data#io_web_apis.


### Reflect

* Do you know how the data is stored on the server side of our example APIs?
  * Do you have to know?
  * Could the data store also be a file?
* What benefits do you see in having an API to interact with a data store?
* Do you see any limitations in using such a web API?


## Follow up

If you are new to web APIs, it may be recommended to a bit of background reading
and learning about the APIs use in your working context.

If you are interested in creating a web API, it may be worthwhile to consider
tools such as [FastAPI](https://fastapi.tiangolo.com/tutorial/first-steps/).

Depending on your use case, different serialization formats or technologies
may be more appropriate.
