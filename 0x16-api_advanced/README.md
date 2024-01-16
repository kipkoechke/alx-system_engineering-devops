![img](https://assets.imaginablefutures.com/media/images/ALX_Logo.max-200x150.png)
  > Advanced REST API's

<!-- Man, I also thougt this would be GraphQL or something. Anyhow, "No  Rest for me this world, perhaps in the next" - Shelby -->

![api-guide](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/314/WIxXad8.png)

## Background Context

This project was further practice in working with API's. I collected data from the
[JSONPlaceholder REST API](https://jsonplaceholder.typicode.com/), and learned how
to export it to either CSV or JSON format.

## Resources

__Read or watch__:
1. [Reddit API Docs](https://www.reddit.com/dev/api/)
2. [Query String](https://en.wikipedia.org/wiki/Query_string)

## Learning Objectives

By the end of this project, you are excected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/) __without the help of Google__.

### General

- [X] How to read API documentation to find the endpoints you’re looking for
- [X] How to use an API with pagination
- [X] How to parse JSON results from an API
- [X] How to make a recursive API call
- [X] How to sort a dictionary by value

## Tasks :page_with_curl:

* **0. Gather data from an API**

  * [0-gather_data_from_an_API.py](./0-gather_data_from_an_API.py): Python script
  that returns information on the to-do list progress of a given employee ID.
  * Usage: `python3 0-gather_data_from_an_API.py <employee ID>`.
  * Output: `Employee <employee name> is done with tasks(<# completed tasks>/<total # tasks>):`
