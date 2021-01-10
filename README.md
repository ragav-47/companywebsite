# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Stark Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/2.png' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
    <h1 id="title">
        Stark Private Limited
    </h1>
    </div>
    <div class="menu">
        <div class="menuitem"><a class="a" href="/home">Home</a></div> 
        <div class="menuitem"><a class="a" href="/products">Products</a></div> 
        <div class="menuitem"><a class="a" href="/people">People</a></div>
        <div class="menuitem"><a href="/contact">Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2021 Stark Private Limited, Developed by Ragav.
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/stark.jpeg" alt="Building">
    <div class="contenttext">
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>Sata hdd</li>
        <li>Sata ssd </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1 style="text-align: center;">
        <strong>Our Premium Products</strong>
    </h1>
    <br>
    <br>
    <br>
    <br>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
                <a href="https://www.amazon.in/DATA-Premier-2666Mhz-A1Price-A1Products/dp/B07GRFYM22/">
            <img src="/static/img/c1.PNG" alt="product image" width="150" height="100">
            </a>
            </div>
           <div class="itemname"><b>4GB DDRA4 laptop memory</b></div>
           <div class="itemprice"><b>Price: Rs.1698.00</b> </div>
           <br>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
                <a href="https://www.amazon.in/Western-Digital-WD10EZEX-Desktop-7200rpm/dp/B0711YN12S/">
            <img src="/static/img/hdd.png"  alt="product image" width="150" height="100">
            </a>
            </div>
         <div class="itemname"><b>Western Digital HDD WD10EZEX 1TB SATA 6Gb/s Desktop 7200rpm 64MB Cache Bare Drive</b></div>
            <div class="itemprice"><b>Price: Rs.3559.00 </b></div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <a href="https://www.amazon.in/MSRKart-OPTICAL-LIQUID-LEVEL-SENSOR/dp/B08KF4P9DZ/">
            <img src="/static/img/levelsensor.png" alt="product image" width="150" height="100">
            </a>
            </div>
           <div class="itemname"><b>Optical liquid level sensor</b></div>
           <div class="itemprice"><b>Price: Rs.2395.00</b></div>
        </div>
        <hr/>
        <br/>
        <br/>
        <div class="productitem">
            <div class="itemimage">
                <a href="https://www.amazon.in/Crucial-BX500-240GB-2-5-inch-CT240BX500SSD1/dp/B07G3YNLJB/">
            <img src="/static/img/harddrive.jpg" alt="product image" width="150" height="100">
            </a>
            </div>
          <div class="itemname"><b>SATA HDD DRIVE</b></div>
          <div class="itemprice"><b>Price: Rs.2500.00</b></div>
        </div>
        <div class="productitem">
            <div class="itemimage"><a href="https://www.amazon.in/SanDisk-Class-Memory-Adapter-SDSQUAR-032G-GN6MA/dp/B073JWXGNT/">
            <img src="/static/img/mchip.jpg" alt="product image" width="150" height="100">
            </a>
            </div>
          <div class="itemname"><b>SanDisk 32GB Class 10 Micro SDHC Memory Card with Adapter (SDSQUAR-032G-GN6MA)</b></div>
         <div class="itemprice"><b>Price: Rs.399.00</b></div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <a href="https://www.amazon.in/JAIN-AUTOMATION-Inductive-Proximity-Sensor/dp/B07RBF2JRS/">
            <img src="/static/img/sensor.png" alt="product image" width="150" height="100">
            </a>
            </div>
           <div class="itemname"><b>Proximity sensor</b></div>
          <div class="itemprice"><b>Price: Rs.280</b></div>
        </div>
        <hr/>
        <br/>
        <br/>
        <div class="productitem">
            <div class="itemimage">
                <a href="https://www.amazon.in/Helea-Appliances-Compatible-Google-Assistant/dp/B07XTF8HPP/">
            <img src="/static/img/switch.jpg" alt="product image" width="150" height="100">
            </a>
            </div>
          <div class="itemname"><b>Helea 10A Wi-Fi Smart Plug, for Low Power Appliances (Type D) Compatible with Alexa & Google Assistant</b></div>
          <div class="itemprice"><b>Price : Rs.899.00</b></div>
        </div>
        <div class="productitem">
            <div class="itemimage"><a href="https://www.amazon.in/Robodo-Electronics-MO49-Measuring-Counter/dp/B0787HRQ27">
            <img src="/static/img/sensorgroove.png" alt="product image" width="150" height="100">
            </a>
            </div>
          <div class="itemname"><b>Robodo MO49 Speed Measuring Sensor Counter Motor Test Groove Coupler Module for Arduino</b></div>
          <div class="itemprice"><b>Price : Rs.204.00</b></div>
        </div>
        <div class="productitem">
            <div class="itemimage"><a href="https://www.amazon.in/Western-Digital-WDS240G2G0A-240GB-Internal/dp/B076Y374ZH/">
            <img src="/static/img/sata.jpg" alt="product image" width="150" height="100">
            </a>
            </div>
           <div class="itemname"><b>Western Digital WD Green 240 GB 2.5 inch SATA III Internal Solid State Drive (WDS240G2G0A)</b> </div>
           <div class="itemprice"><b>Price : Rs.2524.00</b></div>
        </div>
        <hr/>
        <br/>
        <br/>
        <div class="productitem">
            <div class="itemimage"><a href="https://www.amazon.in/ASUS-ZenWiFi-AX-XT8-BLACK/dp/B084CGXVMZ/">
            <img src="/static/img/wifi2.png" alt="product image" width="150" height="100">
            </a>
            </div>
          <div class="itemname"><b>ASUS ZenWiFi</b></div>
          <div class="itemprice"><b>Price : Rs.48490.00</b></div>
        </div>
        <div class="productitem">
            <div class="itemimage"><a href="https://www.amazon.in/D-Link-DIR-819-Wireless-AC750-Router/dp/B07SBTGP16/ref=sr_1_1?dchild=1&keywords=D-link+Dir-819+750+Mbps+Router&qid=1610277157&sr=8-1">
            <img src="/static/img/broadband.webp" alt="product image" width="150" height="100">
            </a>
            </div>
           <div class="itemname"><b>D-link Dir-819 750 Mbps Router</b></div>
          <div class="itemprice"><b>Price : Rs.1,399.00</b></div>
        </div>
        <div class="productitem">
            <div class="itemimage"><a href="https://www.amazon.in/2-5-inch-Internal-Solid-State-WDS100T2B0A/dp/B073SBQMCX/">
            <img src="/static/img/ssd.jpg" alt="product image" width="150" height="100">
            </a>
            </div>
           <div class="itemname"><b>Western Digital Blue 1TB Internal Solid State Drive</b></div>
           <div class="itemprice"><b>Price :Rs.13,985.00</b></div>
        </div>
    </div>
    </div>
{% endblock  %}
```
### people.html
```
{% extends "website/base.html" %}

{% block content %}
    <h1 id="Ex">Executives</h1>
    <div class="row">
            <div class="column">
                <h2>Bill gates</h2>
                <img src="/static/img/bill-gates.jpeg" alt="executive image" width="250" height="300">
                <P>Designation:Founder</P>
            </div>
            <div class="column">
                <h2>Sundar Pichai</h2>
                <img src="/static/img/sundar.PNG" alt="executive image" width="250" height="300">
                <p>Designation: Chief Executive Officer (CEO)</p>
            </div>
            <div class="column">
                <h2>Emma watson </h2>
                <img src="/static/img/emma.PNG" alt="executive image" width="250" height="300">
                <p>Designation: Chief Financial Officer</p>
            </div>
            <div class="column">
                <h2>Robert Drowney JR </h2>
                <img src="/static/img/robert.PNG" alt="executive image" width="250" height="300">
                <p>Designation: Director of Engineering Sector</p>
            </div>
            <div class="column">
                <h2>Scarlett johanson </h2>
                <img src="/static/img/scarlett.PNG" alt="executive image" width="250" height="300">
                <p>Designation: Director of Technical Sector</p>
            </div>
            <div class="column">
                <h2>Chris evans </h2>
                <img src="/static/img/chris.PNG" alt="executive image" width="250" height="300">
                <p>Designation: Director of Safety and Security</p> 
            </div>
    </div>
{% endblock  %}
```
### contact.html
```
{% extends "website/base.html" %}

{% block content %}
   <img src="/static/img/4.png" alt="contact">
    <h1 class="contact">
        <strong><u>CONTACT US</u></strong> 
    </h1>
    <hr>
    <h2 class="contact">
        <strong>ADDRESS:</strong>© Stark pvt,Mountain View, California, United-States
            <br/>
        <strong>EMAIL ID:</strong>starkprivatelimited@gmail.com
            <br/>
        <strong>CONTACT NO:</strong>9876543217
    </h2>
    <hr>
{% endblock  %}
```
## OUTPUT:
![output](./static/img/output1.png)

![output](./static/img/output2.png)

![output](./static/img/output3.png)

![output](./static/img/output4.png)

## CODE VALIDATION REPORT:
![output](./static/img/validate1.png)

![output](./static/img/validate2.png)

![output](./static/img/validate3.png)

![output](./static/img/validate4.png)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://ragav.student.saveetha.in:8000/ HTML code is validated.