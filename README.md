PINC_Node_App

This test application was made to the following specs.

Create an VueJS app that allow adding of multiple modal pop-ups
- Put an 'Add' button to add a modal on the screen
- Clicking ‘Add’ multiple times will result in multiple modals being added
- Each modal should be draggable and resizable
- Each modal should be closable

In order to run the application, please follow the following specs.

1. Navigate to the "pinc_client" folder and do the following:
	a. npm install
	b. npm run dev

2. On your browser, navigate to "http://localhost:8080/#/modalpage"

3. Click the "Propagate" button to keep adding draggable and resizable objects. Multiple objects can be added by clicking the button multiple times.

4. On each object, click the "Close" button to close each object.

5. A video of how it works can be found at the following link: "https://www.useloom.com/share/7e7100ccbc8f45cb8a7561da7d519dc7"

NOTE:

As a bit of practice, I added an express based backend and linked it to the frontend vue app, creating a registration page at "http://localhost:8080/#/register".

In order to get the node server running for any reason, navigate to the "pinc_server" folder and do the following:
	a. npm install
	b. npm run start
