# Easy Socket Communication Server
### Git Repository
    cd /home/pi/
    sudo git clone https://github.com/borhanreo/easy_socket_server.git
    cd easy_socket_server
### At first need to configure server config file 
    sudo nano server.conf
**Change and save**
        
    [config]
    #HOST - change this to public IP if you are using it over the internet
    HOST = 127.0.0.2

    #PORT - any unused port can be used. forward this port if you want to use it over internet
    PORT = 777

    #PASSWORD - any password
    PASSWORD = borhan

    #VIEW - to view the live chat on the server change this to 1
    VIEW = 0    
    
### Need to run server
    sudo python server.py    
    
**Output**

    server v 0.1.1 | Borhan Uddin
	for queries: https://www.github.com/borhanreo/
    ('127.0.0.2', ' ', 777)
    neuron server started on port 777
    
### Then need to run client server
    # sudo python client.py  <host> <port> <password> <username>
    sudo python client.py  127.0.0.1 777 borhan user_borhan   