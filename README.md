# API-testing
## Authors
- Ubah Feisal
- Dennis Kimaita

  
## resources used
- API(url)= https://jsonplaceholder.typicode.com/posts
- Postman
- Python repl

  when using the terminal run **pipenv install requests**
  

# Testing
**get**
- GET requests from postman and the repl were sucsessful.
- Data fetched from the API and gave the status code:200
- terminal displays <Response [200]>


**post**
- POST request in postman was successful.
- add to header Content-Type with value application/json
- add to body data in JSON format:
{
    "userId": 1,
    "title": "mi casa su casa",
    "body": "childish gambino"
}
- Postman returns status code:201

- POST request in python repl was successful

- in addition to defining the url, we also defined and object and pass it as a second argument to request.post() i.e 
requests.patch(url,myobj)
- terminal displays <Response [201]>

**patch**
- PATCH request in postman was successful.
- Set the method to PATCH and update the url to include the id i.e "https://jsonplaceholder.typicode.com/posts/2"
- add to header Content-Type with value application/json
- add to body data in JSON format:
{
    "title": "updated title",
}
- Postman returns status code:200

- PATCH request in python repl was successful
- in addition to defining the url, we also defined and object and pass it as a second argument to request.patch() i.e requests.patch(url,updatedobj)
- terminal displays <Response [200]>

**delete**
- DELETE request in postman was successful.
- Set the method to DELETE and update the url to include the id i.e "https://jsonplaceholder.typicode.com/posts/2"
- Postman returns status code:200

- DELETE request in python repl was successful.
- while defining the url, update the url to include the id. 
- terminal displays <Response [200]>



