[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/thiagodepaulla/)](https://www.linkedin.com/in/thiagodepaulla/)   [![Github Badge](https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/thiagodpaulla)](https://github.com/thiagodpaulla)

# Hello and welcome to my repository
## Meet Personal orcament

![](https:)

## Feel free to interact with the project at the link:
https://thiagodpaulla.github.io/orcamentopessoal/

## Stretch a little more and, know a little more than I've been doing:


https://thiagodpaulla.github.io/

### Understand a little more about how it was created.



  * [Project](#project)
  * [Technologies](#technologies)
  * [License](#license)

#Project

This project proposes the creation of a CRUD (Create, Read, Update and Delete), containing personal expense information in a fast and objective way.



of the resources used in the project i would like to highlight some below as more relevant at this specific moment.

### Cookes



used the web storage resource because modern browsers generally implement data storage resources within the browser itself, before html 5 the cookes resource was used but with the advent of html 5 browsers started to use other methods for local storage data, the cooks function as data that is stored on the client side in the browser and whenever there is an http request, that is, whenever we access a particular page, cookies are attached to this request in such a way that the server is able to access these information, extract your logic in order to understand the information already registered on the client side and after this processing make the return of this information requested by the client, as in the e-commerce sites that store our queries and return the queries we made, and this is very useful because it is stored on the client side, and attached to the http request, being allowed by the analytical servers request by request and return exactly the logic of each client.

the case of local storage and session storage are similar to cookies with the difference of not being attached to an http request and are

### Session storage

Stores information while the browser the browser instance is active, when we close the browser all information kept in the browser instances is lost.



### Local storage

We can store the information, close the browser instances, shut down the machine or restart the machine and the data will remain stored until it is intentionally removed.







### JSON notations



Store data within local storage, converting a literal object to JSON

everything that goes inside a string can be stored in an object but in the case of JSON notation this string receives some instructions like

'{' category ':' household appliance '}'

keeping keys and values ​​encapsulated inside the quotes internally as well.





Retrieving a literal object previously instantiated within the application, and in the process of using this object in the set item function that will open a communication with the local storage, a JSON representation of this object was forwarded

        record (expense)

}

function record (d) {

    localStorage.setItem ('expense', JSON.stringify (d))

}

 in such a way that when it is retrieved within the application on the other side in the local storage case the application has the ability to parse this information by converting it into a new object.



the instance of an object exists only within an application when it needs to communicate with a server or other applications, in this case a local storage application is an internal application of the browser but an application external to my application, therefore communication is necessary and for this is necessary to create a communication protocol so that the data can be communicated, however literal objects they cannot be passed in this process because they are objects and these objects exist only in the application instance, so we need some way to transcribe this object in a text type notation in this case the JSON notation for this text to be attached to this communication that can be done either with the back end or with other applications and JSON will act however in this medium of communication field as it is natively supplied by javascript.

Json is an important javascript library and from it we can use the strigfy method that converts the project directly to a json object without having to concatenate strings.

 the opposite can also be done by transforming a JSCON object into a literal object using the JSON.parse method (productJSON)



 ### creation of dynamic indexes for inclusion of records within local storage



 retrieve the data and insert the data into the local storage, and now it is necessary to generate a new record as the creations are made so it is necessary to create a dynamic index, which will include a new item without overlapping the previous index.





 ### Data validation

 using a bootstrap component called a modal component, it displays a div on the screen calling the user's attention to that respective point so we can insert the information that I want the user to be aware of at the moment when he is typing.

 <option value="">Ano</option>

            <option value="2019">2019</option>


# Technologies

🚀 The project was developed using the following technologies

➜ Bootstrap

➜ JavaScript

➜ HTML

➜ CSS


# License
📂 Distributed under the MIT license. See LICENSE for more information.


