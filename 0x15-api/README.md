![img](https://assets.imaginablefutures.com/media/images/ALX_Logo.max-200x150.png)
  > Rest APIs

![no-rest-for-the-wicked-lol](https://media3.giphy.com/media/HkGiwbwqhJ5oeV9746/200w.webp?cid=ecf05e47mda0zcx3nsrypg8rdygxetp5ka5100rmcopqrawo&rid=200w.webp&ct=g)

## API

API stands for Application Programming Interface. Simply put, an API is a set of rules that enables one application to communicate with another. APIs can be used to allow different applications to share data and functionality. For example, if you use a weather app on your phone, it may be getting its data from an API provided by a weather service.

This project was further practice in working with API's. I collected data from the
[JSONPlaceholder REST API](https://jsonplaceholder.typicode.com/), and learned how
to export it to either CSV or JSON format.

## Background context

Old-school system administrators usually only know Bash and that is what they use to build their scripts. While Bash is perfectly fine for a lot of things, it can quickly get messy and not efficient compared to other programming languages. The new generation of system administrators, usually called SREs, are pretty much regular software engineers but instead of building products, they are managing systems. And one of the big differences with their predecessors is that they know more than just Bash scripting.

One popular way to expose an application and dataset is to use an API. Often, they are the public facing part of websites and micro-services so that allow outsiders to interact with them – access and modify their data. In this project, you will access employee data via an API to organize and export them to different data structures.

This is a perfect example of a task that is not suited for Bash scripting, so let’s build Python scripts.

## Resources

__Read or watch__:
1. [Friends don't let friends program in shell script](https://www.turnkeylinux.org/blog/friends-dont-let-friends-program-shell-script)
2. [What is an API](https://www.webopedia.com/definitions/api/)
3. [What is an API? In English please](https://www.freecodecamp.org/news/what-is-an-api-in-english-please-b880a3214a82/)
4. [What is a REST API](https://www.sitepoint.com/rest-api/)
5. [What are microservices](https://smartbear.com/learn/api-design/microservices/)
6. [PEP8 Python style - having a clean code respecting style guide is really appreciated in the industry](https://peps.python.org/pep-0008/)

## Learning objectives

By the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/) __Without the help of Google__:

## General

* [X] What Bash scripting should not be used for
* [X] What is an API
* [X] What is a REST API
* [X] What are microservices
* [X] What is the CSV format
* [X] What is the JSON format
* [X] Pythonic Package and module name style
* [X] Pythonic Class name style
* [X] Pythonic Variable name style
* [X] Pythonic Function name style
* [X] Pythonic Constant name style
* [X] Significance of CapWords or CamelCase in Python

## Tasks :page_with_curl:

* **0. Gather data from an API**
  * [0-gather_data_from_an_API.py](./0-gather_data_from_an_API.py): Python script
  that returns information on the to-do list progress of a given employee ID.
  * Usage: `python3 0-gather_data_from_an_API.py <employee ID>`.
  * Output: `Employee <employee name> is done with tasks(<# completed tasks>/<total # tasks>):`

* **1. Export to CSV**
  * [1-export_to_CSV.py](./1-export_to_CSV.py): Python script exports to-do list
  information of a given employee ID to CSV format.
  * Usage: `python3 1-export_to_CSV.py <employee ID>`
  * File name: `<user id>.csv`.
  * Format: `"<user id>","<username>","<task completed status>","<task title>"`.

* **2. Export to JSON**
  * [2-export_to_JSON.py](./2-export_to_JSON.py): Python script that exports
  to-do list information of a given employee ID to JSON format.
  * Usage: `python3 2-export_to_JSON.py <employee ID>`
  * File name: `<user id>.json`
  * Format: `{ "<user id>": [ {"task": "<task title>", "completed": <task completed status>, "username": "<username>"}}, ... ]}`

* **3. Dictionary of list of dictionaries**
  * [3-dictionary_of_list_of_dictionaries.py](./3-dictionary_of_list_of_dictionaries.py):
  Python script that exports to-do list information for all employees to JSON format.
  * Usage: `python3 3-dictionary_of_list_of_dictionaries.py`
  * File name: `todo_all_employees.json`
  * Format: `{ "<user id>": [ {"username": "<username>", "task": "<task title>", "completed": <task completed status>}, {"username": "<username>", "task": "<task title>", "completed": <task completed status>}, ... ], "<user id>": [ {"username": "<username>", "task": "<task title>", "completed": <task completed status>}, {"username": "<username>", "task": "<task title>", "completed": <task completed status>}, ... ]}`


