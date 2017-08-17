## Editable Profile


This exercise requires a little bit of front end and back end.
Please provide some code which allows you to edit your profile (both client and server), based on the attributes below.
If you're stronger on the backend, that's fine to concentrate on that more - just let us know in the notes you've done so (and likewise for the front end).
Please, however, ensure both the client and server side is *well tested* and *clean code* and that the code works before you submit your code.

### Client side
Front end can be either a web or app front end.  
If it's web, make sure it can be used on multiple devices.
Completely up to you what frameworks; on our own code we use angular 2 or react for web, and all the usual libs for android and iOS that allows MVVM, MVP, and easier testing.
For the image upload, a file picker is fine

### Server side
The server side can be in whatever language you are strong with.  
We mainly use js, java, and a little bit of php and go, so please try to use one of them that you're stronger with.
If you opt for a db approach, store in whatever storage you see fit.


#### Http Server for Fixed Values
We have provided a small http server for serving the fixed attributes for multiple choice and lookup fields, such as ethnicity, smoking frequency, cities lat/lon etc
You can find this in the ```server``` folder, and is spun up using ```./server.sh``` on mac / linux.
This is a simple http server, using npm, serving flat json files, from the respective folders.
You can use what's provided or build something yourself to serve these attributes.
So you're free to modify the structure of the urls, change how it gets served etc, but ensure the json structure remain the same

The 2 urls are:
* http://localhost:8080/en/locations/cities.json
* http://localhost:8080/en/single_choice_attributes.json

#### Attributes for Editing on Profile

Note that some of the attributes below are only used internally, and wouldn't be displayed on the platform.  
They're needed for targeting / matchmaking etc at a later date.  
You can decide how you want to tell the user of the platform that information.


|     Field    	   |  Type                              | Mandatory  | Display on platform?    |
|------------------|------------------------------------|------------|-------------------------|
| Display Name	   | free text, up to 256 char          | X          | X	                   | 
| Real Name		   | free text, up to 256 char          | X          |                         |
| Profile Picture  | upload component                   |            | X                       |
| Birthday         | date                               | X          | X	                   | 
| Gender	       | single selection                   | X          | X	                   | 
| Ethnicity        | single selection                   |            | X	                   | 
| Religion	       | single selection                   |            | X	                   | 
| Height	       | not editable, only on signup       |            | X	                   | 
| Figure	       | single selection                   |            | X	                   | 
| Marital Status   | single selection                   | X          |  	                   | 
| Occupation	   | free text, up to 256 char          |            |  	                   | 
| About Me	       | free text, up to 5000 char         |            | X	                   | 
| Location	       | text autocomplete (type city name, store lat/lon) | X | X                 |

Note; all free text fields should disallow any markup, and be secure (xss etc)