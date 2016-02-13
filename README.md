# Secure-Smart-Card-Reader-Without-Applet

#### As Oracle going to stop the Applet support from Java 1.9 , A 100% secure solution is needed to integrate a smart card reader into an enterprise application

###### Its done here

###### How it works

1. A https server is designed in a desktop application which handles the card reader communication
2. The desktop application is signed with a proper private key
3. If a user initiates a request from the browser to the webapp ,the webapp encrypts the request with the signed private key and a token as a response
4. Then the browser pass it to the desktop app
5. If desktop app able to decrypt then it will encrypt the card data with the token
6. The browser will send then it to the server
7. Based on the session and token id the server will respond positive or negative response

###### Targeted Audience

1. Requirements to avoid fraud data and fraud desktop app

   
