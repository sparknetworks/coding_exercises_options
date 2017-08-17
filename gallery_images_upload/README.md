## Gallery Images Upload


Please provide a gallery with an image upload feature.
This exercise is mostly front end with a tiny bit of back end.
If you're stronger on the backend, you can try this one, but we'll definitely be looking strength on the front end.
Please also ensure both the client and server side is *well tested* and *clean code* and that the code works before you submit your code.

### Client side

The client side can be either web or app.
If it's web, please ensure it can be used on multiple devices.
Completely up to you what frameworks you use; on our own code we use angular 2 or react for web, and all the usual libs for android and iOS that allows MVVM, MVP, and easier testing.

##### Web Requirements
* Provide a gallery view of all previously uploaded images
* For image Upload:
    * mobile web, tablet - this will be a button which will prompt you to either access the camera and take a pic, or select from files on device
    * desktop web - will have 2 options: drag image to page to upload, or a button which allows selection of multiple files on device
* super nice to see the web-views handling rotation on devices

##### App Requirements
For the image upload please provide:
 * a gallery view of all previously uploaded images
 * a button which can either request to take a picture, or upload from camera roll
 * the ability to rotate or crop images


### Server side
The server side can be in whatever language you are strong with.  
We mainly use js, java, and a little bit of php and go, so please try to use one of them that you're stronger with.

Don't worry too much about how this stuff should be stored and served properly on the server (such as s3 buckets, and CDNs etc).
It's fine to store and serve the images locally.

If you opt for a db approach, store in whatever storage you see fit.

