# END TO END QR CODE GENERATOR
## Technologies used 
- NodeJs
- Express
- React 
## Creating Backend
- Create new folder backend and install required dependencies
```sh
npm install express
npm install cors
npm install qrcode
```
- QRcode.toDataURL -> it generates a long string which represents the QRcode 
- When the frontend hits the "/generate-url" route backend generates the long String and sends it to frontend 
- Backend also checks for the errors and handles the errors 

## Creating Frontend
- Initialize the new React project in frontend folder 
- Install all the required node modules for frontend
```sh
npm install axios
```
- On clicking the Submit url button backend request goes to ("http://localhost:3000/generate-url")
- Frontend sends the input box url in body to backend 
- Frontend receives the long string 
- Storing the long string in a state variable 
- Now frontend can generate and display the QRcode.
