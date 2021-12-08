# Developing a Simple Webserver
## AIM:

To develop a simple webserver to serve html pages.
## DESIGN STEPS:
### Step 1:
HTML content creation
### Step 2:
Design of webserver workflow
### Step 3:
Implementation using Python code
### Step 4:
Serving the HTML pages.
### Step 5:
Testing the webserver
## PROGRAM:
~~~
from http.server import HTTPServer,BaseHTTPRequestHandel content ="""
<title>My webserver</title>
NAME: sarveshkaran
Ref No: 21000082
E-mail: sarveshaugusto2419@gmail.com
""" class myhandle(BaseHTTPRequestHandler): def do_GET(sefl):print("request received) self.send_response(200)   I text/html; charset=utf-8') self.end_headers() self.wfile.write(content.encode()) server_address = (",8080) httpd 
HTTPServer(server_address,myhandler) print("my webserver is running...") httpd.serve_forever()
~~~
## OUTPUT:
![output](sarweb.png)
## RESULT:
Thus the program run successfully
