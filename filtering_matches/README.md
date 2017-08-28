## Filtering Matches

This exercise requires a little bit more back end and a little bit less front end.
Please provide some code which allows you to filter on a prebuilt set of filters (using server side filtering)
If you're stronger on the frontend, that's fine to concentrate on that more - just let us know in the notes you've done so.
Please, however, ensure both the client and server side is *well tested* and *clean code* and that the code works before you submit your code.

### Filtering Details

| Filter | Details |
|--------|---------|
| Has photo | Boolean yes / no filter |
| In contact | Boolean yes / no filter |
| Favourite | Boolean yes / no filter |
| Compatibility Score | range: from 1% to 99% |
| age | range: from 18 years old until > 95 years old |
| height | range: from 135cm to > 210cm |
| distance in km | single selection: lower bound < 30 km, upper bound > 300 km | 


### Server side

The server side can be in whatever language you are strong with.  
We mainly use js, java, and a little bit of php and go, so please try to use one of them that you're stronger with.

There is a small json file provided [database/matches.json](./database/matches.json).  
Please use this data as the basis for your service.
If you opt to use a db, please import this data as your starting point, and ensure you provide full setup script or instructions for the db.
You can use whatever storage you think fits the problem.


### Client side

The client side can be either web or app.
If it's web, please ensure it can be used on multiple devices.
Completely up to you what frameworks you use; on our own code we use angular 2 or react for web, and all the usual libs for android and iOS that allows MVVM, MVP, and easier testing.

##### Web Requirements
Please provide an initial list view with all existing matches provided in the [database/matches.json](./database/matches.json) file.
You should also have a number of filters available, as listed above.
If you use range sliders or any components where you have dragging actions etc, please ensure ensure they are cross device compatible
Note - for filtering "distance in km" assume that the user has logged in as one of the users in matches.json file, and use their "city" property.  You don't need to ask location from their browser

##### App Requirements
Please provide an initial list view of all existing matches and a number of filters, as listed above.
The resulting app should handle rotation and scale for tablets as well as phones.
Note - for filtering "distance in km" assume that the user has logged in as one of the users in matches.json file.  Ask for the users location in the app first.  If the user does not supply it, use their "city" property from their profile
