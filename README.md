Appcubator is a browser-based WYSIWYG interface for rapidly building Express.js/MongoDB applications.

Design Goals
------------

1. Simple things should be simple: Easy to build a canonical web app.
2. Complex things should be possible: Allow extensibility with custom code
3. Interoperate with existing community code
4. Usable by people who don't have knowledge of web dev.

What is an Appcubator App?
--------------------------

An Appcubator app is represented as a javascript object in the browser, called the App State. It has a hierarchical structure with a well-defined schema.

The user creates and modifies App Components via the User Interface in order to build their app. These interactions correspond to data changes in nodes of the Javascript object.

When the user presses Publish, the javascript object is serialized to JSON, and shipped to a server.

The nodes of the javascript object go through macro-expansion to turn the user-inputted data into code.

The the code is written to disk, zipped, and shipped back to the user, or pushed to a server to be deployed.

Documentation
-------------

(these will be links)

1. mapping from the app state to the generated Node.js app
2. generator system
3. base app components built using generators
4. plugin system
5. user interface design and code
6. deployment
