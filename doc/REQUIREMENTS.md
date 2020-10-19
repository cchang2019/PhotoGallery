# Requirements
Requirements for Photo Gallery
### Components and Basic Needs
  - **GUI:** <br>
    Graphic UserInterface should contain basic functionalities and properly connect to the Client side. <br>
    GUI is generated through Node JS / created through HTML and CSS. (NOT yet Determained)
  - **Client:** <br>
    Client side should be able to maintain a stable connection with the server, process server response, and manipulate files </br>
    (eg: convert, download, upload). <br>
    Client side also creating / linking (NOT yet Determained) the GUI.
  - **Server:**  
    A server that can handle client's requests, process data within the request, and be able to manipulate files </br>
    (eg: convert, download, upload).
  
  

### GUI
- The GUI starts with the login window which asking for username and password input.
- The home landing page of Photo Gallery will show all images of the user. In the home landing page, total number of image should be displayed (eg: 138 Images).
- When the user clicks on the image, the image will zoom in and fill most / entire window (view page). In view page, current image number should be displayed (eg: 57/138).
- A BACK button to go back to previous page. 
- A DELETE button to delete image(s).
- A UPLOAD button to upload local image(s).
- A DOWNLOAD button to download image(s) from Photo Gallery.
### Client Side
- The client needs an account(username and password pair) in order to login to Photo Gallery. 
- The client can veiw all uploaded images. 
- The client can upload one or multiple image(s) to Photo Gallery (this action will send data to the server side). 
- The client can delete image(s) on the Photo Gallery (this action will also erase the data on the server side).
- The client can download image(s) from the system if needed (in case where the original image was locally deleted by accident, but previously uploaded to the system).
### Server Side
- The server needs to validate the client identity.
- The server needs to send image(s) from the client's data folder to the client side when recieving get request.
- The server needs to handle the data (images) send by the client and store (download) the file to the client's data folder.
- The server needs to remove specific / all local file(s) in specific client's data folder when recieving delete request.
