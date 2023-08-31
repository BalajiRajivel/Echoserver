# Echoserver
Echo server and client using python socket

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

Design of echo server and client using python socket

### Step 2:

Implementation using Python code

### Step 3:

Testing the server and client 

## PROGRAM:
### CLIENT
```
import socket

s=socket.socket()
s.connect(('localhost',65124))
while(1):
msg=input("Client>")
s.send(msg.encode())
print("Server>"+s.recv(1024).decode())
```

## OUTPUT:

## RESULT:
The program is executed successfully
