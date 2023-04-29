# Computer Networks

![c](https://user-images.githubusercontent.com/116082827/235302516-a6a14249-ea52-44b0-aa59-2581cbd525e2.png)


Computer networks are systems of interconnected devices that communicate with each other using a variety of protocols and technologies. Understanding computer networks is essential for developing software that operates in networked environments. Here's an example of a simple network program in Python using the socket library:



import socket



# Create a socket object

s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)



# Get local machine name

host = socket.gethostname()



# Reserve a port for your service

port = 12345



# Bind the socket to a specific address and port

s.bind((host, port))



# Listen for incoming connections

s.listen(5)



while True:

    # Wait for a connection

    client, addr = s.accept()

    print('Got connection from', addr)

    

    # Send a message to the client

    message = 'Thank you for connecting!'

    client.send(message.encode('ascii'))

    

    # Close the connection

    client.close()
