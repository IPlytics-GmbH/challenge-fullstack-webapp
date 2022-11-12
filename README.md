# IPlytics coding challenge
This coding challenge is for candidates for the position "Fullstack Developer - Web Applications"

## Overview
Our software lets users search for Patents and Standards, amongst other things. Our web application is the gateway to our data sets, and we would like to see how well you can build an application that models a little part of our data universe.

We want to know how well you can work with the following:
* Client-side applications
* Code design & architecture
* RESTful API design
* Unit and integration testing
* Written and generated documentation

## Specifications
The IPlytics platform is at its core a search platform. We deal with patents and standards on a daily basis. You task is to build a mini platform that allows for creating and searching patents.


### What we want you to do

You should build a small application of two parts - A Frontend and a Backend part -  in order to pass our test. In addition to doing the tasks below, we want to see that you can:
* Write clean code and structure it well
* Cover your code with tests in a suitable manner
* Write good commit messages and break up your work into sensibly-sized chunks
* Add documentation where necessary. This could be handwritten or auto-generated from your code


Here are your tasks:

### Data Model

Design the data model for the patents entity. You are free to choose any database technology you wish. A patent consists of:
<br>
`- publication_number: Id`
<br>
`- publication_date: Date`
<br>
`- title: String`

### CRUD for patents 
Our users need to be able to add their own patents to the system. 

* Using the technology/framework you wish, build an api that allows the user to create new patent entries. Make sure to use the best practices of RESTful API design, to return sensible responses, and the correct status codes as required. You should also add integration and unit tests as needed.
* Create a `/search` endpoint that allows the user to search our patents database by `any` field. The search endpoint should be able to handle sorting and paging.

### Search UI
Our users need a user interface in order to view and query our data.

* Using the technology you wish (strong preference for React), build a basic user interface with a simple search bar, search button and an add button for inserting new patents. Clicking the add button should trigger a popup to open reqiring the user to create a new patent.
* When a user searches by any keyword, a list of relevant patents should be returned and rendered on the webpage.
* We would like to have an autocomplete functionality too, so the user would get search suggestions as they type. Implement an autocomplete behaviour for the search bar. You are free to render the suggestions the way you see fit.

`NOTE: Do not spend time on styling your webpage, focus on having a functional solution beforehand.`


### Bonus - Handle Declarations
One interesting aspect of industrial or technology standards is how they are composed. Companies or organisations typically work with a standard-setting organisation (like ISO or ETSI) to "declare" their patent to be a necessary part of a standard. So there is a relational connection between patents and standards, which we can model as a "declaration".

* Create a SQL model for a declaration, and include the appropriate foreign key relationships.

* Create new endpoint(s) which let a user declare their patent(s) to be part of a standard. As in the previous task, ensure that appropriate responses and status codes are returned.

## How to submit
Once you're happy with your work and want to submit, put both repos into a parent folder and  `zip` the folder and submit it via email to our HR manager. Remember to include the whole assignment directory (including hidden files), so we can see your git commit history.

Best of luck and thanks for taking the time to complete this challenge.
