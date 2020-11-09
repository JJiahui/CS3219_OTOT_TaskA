# CS3219 OTOT Assignment Task A
Nginx, Docker, reverse proxy

## Setup & Run
Prerequisites
* Docker & Docker Compose
* Nginx

Within the directories `site1` and `site2`, run the following command.
```
docker-compose up -d
```
Navigate to `reverse-proxy`, and run the following commands.
```
docker-compose build
docker-compose up -d
```
Verify that the containers are running
```
docker-compose ps
```

Add the following lines to /etc/hosts  
```
<your-ip-address> site1.example.com  
<your-ip-address> site2.example.com  
```

For Windows follow these steps
* Press the Windows key.
* Type Notepad in the search field.
* In the search results, right-click Notepad and select Run as administrator.
* From Notepad, open the following file: c:\Windows\System32\Drivers\etc\hosts.
* Make the necessary changes to the file.
* Click File > Save to save your changes.

Visit site1.example.com and site2.example.com in a browser.


### Screenshots
<img src="./images/site1.jpg?raw=true" width="400"/>
<p></p>
<img src="./images/site2.jpg?raw=true" width="400"/>

### References
https://dev.to/sukhbirsekhon/what-is-docker-reverse-proxy-45mm
