## Personality Test

This exercise requires a little bit of front end and back end.
Please provide some code which allows a user to answer questions for a personality test (both client and server), based on the data provided.
You'll find a JSON file in [database/personality_test.json](./database/personality_test.json)

The answers to the questions should be stored, and should be queryable in the future.

If you're stronger on the backend, that's fine to concentrate on that more - just let us know in the notes you've done so (and likewise for the front end)

Please, however, ensure both the client and server side is *well tested* and *clean code* and that the code works before you submit your code.


### Client side

The client side can be either web or app.
If it's web, please ensure it can be used on multiple devices.
Completely up to you what frameworks you use; on our own code we use angular 2 or react for web, and all the usual libs for android and iOS that allows MVVM, MVP, and easier testing.

##### Web Requirements
Please provide an list of questions, separated by category.  Please ensure the web views can work on any device.
You can either submit the answers one by one when they are being answered or send it all at the end

##### App Requirements
Please provide an list of questions, separated by category. 
The resulting app should handle rotation and scale for tablets as well as phones.
You can either submit the answers one by one when they are being answered or send it all at the end.


### Server side

The server side can be in whatever language you are strong with.  
We mainly use js, java, and a little bit of php and go, so please try to use one of them that you're stronger with.

There is a small json file provided [database/personality_test.json](./database/personality_test.json) for all the questions.  
Please use this data as the basis for your service.
If you opt to use a db, please import this data as your starting point, and ensure you provide full setup script or instructions for the db.
You can use whatever storage you think fits the problem.
