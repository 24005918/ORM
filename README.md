# Ex02 Django ORM Web Application
# Date:28.08.2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![WhatsApp Image 2024-12-13 at 09 31 03_361b8c4e](https://github.com/user-attachments/assets/47579f68-a135-49b9-9971-e150e3e13d8e)

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM:

```
from http.server import HTTPServer, BaseHTTPRequestHandler

content = '''
<html>
<head>
<title>My Laptop</title>
</head>
<body>
<center>
    <h1>My Laptop Configuration</h1>
    <table border="5" cellpadding="5" align="center">
        <tr>
            <th>System Specs</th>
            <th>Description</th>
        </tr>
        <tr>
            <td>Processor</td>
            <td>13th Gen Intel(R) Core(TM) i5-1335U 1.30 GHz</td>
        </tr>
        <tr>
            <td>Operating System</td>
            <td>Windows 11 Home Single Language 64-bit</td>
        </tr>
        <tr>
            <td>Graphics Card</td>
            <td>Integrated Intel® Iris® Xe Graphics</td>
        </tr>
        <tr>
            <td>Memory</td>
            <td>16 GB DDR4-3200MHz (8 GB SODIMM + 8 GB Soldered)</td>
        </tr>
        <tr>
            <td>Storage</td>
            <td>512 GB SSD M.2 2242 PCIe Gen4 TLC Opal</td>
        </tr>
        <tr>
            <td>Display</td>
            <td>16-inch WUXGA (1920×1200), IPS, Anti-Glare, 100% sRGB, 300 nits, 60Hz</td>
        </tr>
    </table>
</center>
</body>
</html>
'''

class MyServer(BaseHTTPRequestHandler):
    def do_GET(self):
        print("GET request received...")
        self.send_response(200)
        self.send_header("Content-type", "text/html")
        self.end_headers()
        self.wfile.write(content.encode())

print("This is my webserver")
server_address = ('', 8000)
httpd = HTTPServer(server_address, MyServer)
httpd.serve_forever()

```
# OUTPUT:


<img width="1071" height="587" alt="image" src="https://github.com/user-attachments/assets/069f3343-6eb1-4e7d-9552-47ef21bf6246" />


![Screenshot_2024-11-20_162048 1](https://github.com/user-attachments/assets/29b647d1-f301-4297-8c10-d94e5d258f8a)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
