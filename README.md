# 3c.CREATION FOR FILE TRANSFER USING TCP SOCKETS
## AIM
To write a python program for creating File Transfer using TCP Sockets Links
## ALGORITHM:
1. Import the necessary python modules.
2. Create a socket connection using socket module.
3. Send the message to write into the file to the client file.
4. Open the file and then send it to the client in byte format.
5. In the client side receive the file from server and then write the content into it.
## PROGRAM

##CLIENT
```
host = socket.gethostname() 
port = 60000 
s.connect((host, port)) 
s.send("Hello server!".encode()) 
with open('received_file', 'wb') as f:
    while True:
        print('receiving data...')
        data = s.recv(1024)
        print('data=%s' % data)
        if not data:
            break
        f.write(data)

print('Successfully got the file')
s.close()
print('connection closed') 
```

## SERVER
```
host = socket.gethostname() 
port = 60000 
s.connect((host, port)) 
s.send("Hello server!".encode()) 
with open('received_file', 'wb') as f:
    while True:
        print('receiving data...')
        data = s.recv(1024)
        print('data=%s' % data)
        if not data:
            break
        f.write(data)

print('Successfully got the file')
s.close()
print('connection closed')
```
## OUPUT
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/3e87f02f-00e2-4b3f-a6ba-76b9d8fd4610" />

## RESULT
Thus, the python program for creating File Transfer using TCP Sockets Links was 
successfully created and executed.
