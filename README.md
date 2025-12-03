Exercise D4: Network Summary HTTP, TCP, UDP

Step 1:
Write HTTP Server with an endpoint /port
Upon GET request to this endpoint the server will fo the following:
Generate random number
Return this number to the caller as value of HTTP Header “PortNumber”
Check your server with postman 
You can use flask as your HTTP server. 
In fact, this will make your code very elegant, clean and enjoyable. You can also find plenty of documentation on how to do stuff there. 
Modern programming is using existing components and not rewriting things that are already available. 


Step 2: 	
The server will open a UDP server socket with that random number as its port number
Callers of this port with the code “Cyber Himmelfarb” will get the response  “Victory!”
Any caller with other code will get response “No Entry” 
Run the UDP server in a different thread.

Step 3:
Write a python client that ties everything together:
Calls the http-server 
Extracts the port from the response
Sends the code over UDP to this port
Print the response
Handle nicely any error on the way (connecting the HTTP server, error response from the HTTP server)


You can run everything on your localhost and use its IP address.



Enjoy
