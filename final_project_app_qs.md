# SI 364 - Final Project questions

## Overall


* **What's a one-two sentence description of what your app will do?**

I will have the user enter an airport code and will then give them the weather to the airport. These will all be stored in a database and will send an email with the highest or lowest the temperature that was recorded when requested. 

## The Data

* **What data will your app use? From where will you get it? (e.g. scraping a site? what site? -- careful not to run it too much. An API? Which API?)**

I will get data from the FAA REST API that will allow me to acess the weather for U.S. airports. 

https://app.swaggerhub.com/apis/FAA/ASWS/1.1.0#/

* **What data will a user need to enter into a form?**

The user will enter their name and the airport code they want to get the weather and information about. There will also be an option to get an email of the highest and lowest temperature.  

* **How many fields will your form have? What's an example of some data user might enter into it?**

It will have three feilds. One enterting the name of the person looking for the information, the next will be entering the airport code and the other will be the option of sending the highest or lowest temperature that has been recorded to the email. 

* **After a user enters data into the form, what happens? Does that data help a user search for more data? Does that data get saved in a database? Does that determine what already-saved data the user should see?**

The information will be stored and there will be an option to send an email with the information stores. 

* **What models will you have in your application?**
I will have two models, one of the airport they searched and one of the types of weather. 

* **What fields will each model have?**
The fields within each models are user names, airport, and weather with the last time it was updated. 

* **What uniqueness constraints will there be on each table? (e.g. can't add a song with the same title as an existing song)**
You can't add the same airport code. 

* **What relationships will exist between the tables? What's a 1:many relationship between? What about a many:many relationship?**
It will be a one to many relationship. There is one airport, but you can have many different temperatures. 

Many - many relation: the weather can be rainy ect. can be at many different airports. 

* **How many get_or_create functions will you need? In what order will you invoke them? Which one will need to invoke at least one of the others?**
I am not exactly sure how many get or create functions I will neeed. 

## The Pages

* **How many pages (routes) will your application have?**
It will have at least 3. One will be to enter the information, one will be the list of information already stored, and one will be the option to send an email.  

* **How many different views will a user be able to see, NOT counting errors?**
There will be multiple views. One will be the log in page entering yoru name which will take you to enter in what airport you want to get weather about. The final page will give an option if they want to recieve an email or not 


* **Basically, what will a user see on each page / at each route? Will it change depending on something else -- e.g. they see a form if they haven't submitted anything, but they see a list of things if they have?**
They will be able to see the weather they requested and any recent updates. They will also be able to choose if they want it uploaded. If they do not submit anything they will receieve a list of all other information they previously entered in an output. 

## Extras

* **Why might your application send email?**
It will send emails of updates to the weather for example if my mom is checking the weather for when I am flying.

* **If you plan to have user accounts, what information will be specific to a user account? What can you only see if you're logged in? What will you see if you're not logged in -- anything?**

* **What are your biggest concerns about the process of building this application?**

I do not feel 100% comfortable with data bases yet and am nervous that since you cannot add something with the same name that the application will not work very long.  
