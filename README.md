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
```py
import socket

s=socket.socket()
s.connect(('localhost',65124))
while(1):
msg=input("Client>")
s.send(msg.encode())
print("Server>"+s.recv(1024).decode())
```

### SERVER
```py
import socket

s=socket.socket()
s.bind(('localhost',65124))
s.listen(5)
c,addr=s.accept()

while(1):
msg=c.recv(1024).decode()
print(msg)
c.send(msg.encode())
```

## OUTPUT:
### CLIENT
![image](https://github.com/BalajiRajivel/Echoserver/assets/103949835/ec6bd2dd-ab71-4268-8455-f7b8bbc61095)

### SERVER
![image](https://github.com/BalajiRajivel/Echoserver/assets/103949835/cece7506-112b-4889-9f45-09079ed0aeac)

## RESULT:
The program is executed successfully
