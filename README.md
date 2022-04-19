# Test assignment for PHP developer (Advertising team)
## Task
It is necessary to create a service for storing and submitting adverts. Adverts must be stored in a database. The service should provide an API that runs in JSON format.

## Requirements
* PHP programming language
* The final version should be posted on github.com
* Simple instruction to start (ideally - with the ability to run through `docker-compose up`, but this is optional);
* Implement 3 methods: getting a list of ads, getting one ad, creating an ad;
* Validation of fields: each advert has no more than 3 pictures (links to pictures), description no more than 1000 characters, title no more than 200 characters;
* No need to implement HTML and JS parts. PHP only;

If you have doubts about the details - make the decision yourself, but in your README.md we recommend writing down the questions, and the decisions made on them.

## Details
#### Method for getting list of ads 
* Pagination: 10 ads should be present on one page;
* Sorting: by price (ascending / descending) and by date of creation (ascending / descending);
* Fields in the response: ad title, link to the main picture (the first in the list if there are several pictures), price.

#### Method of getting a specific ad 
* Required fields in the response: ad title, price, link to the main picture;
* Optional fields (can be requested by passing the 'fields' parameter): description, links to all pictures.

#### Ad creation method
* Accepts all the above fields: title, description, several links to pictures (you don't need to upload pictures anywhere), price;
* Returns the ID of the created ad, and the result code (error or success).

## Complications
Not required, but the task can be completed with any number of complications:
* Unit tests: try to achieve coverage of 70% or more;
* Containerization: it is possible to raise the project using the command `docker-compose up`;
* The architecture of the service is described in the form of text and / or diagrams
* Documentation: there is a structured description of the service methods.
