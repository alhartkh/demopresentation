# Webframes for building apps in python 

---

## Khalid Alharthi

### I specialize in wasting time in trivial stuff
### Misk Dsi
### Team 3

<!-- .slide: style="text-align: left;"> -->
<i class="fas fa-envelope"></i>  alhartkh@gmail.com<br>
<i class="fab fa-github"></i><a href="https://github.com/alhartkh">  github.com/alhartkh</a>

---

## Objectives
<!-- .slide: style="text-align: left;"> -->
* Define webframes (aka web frameowkrs or web development framework "WDF")
* Understand the difference between frameworks & libraries
* Understand the difference between websites & webapps
* Contrast the types of frameowkrs
* Classify Python webframes types
* Compare Python popular webframes  
* Construct a simple webapp using Flask 

---

## Agenda
<!-- .slide: style="text-align: left;"> -->
- Background<br>
- Demonistration<br>
- Conclusion<br>
- Q&A<br>

---

## Background 

---

## What are web frames?
<!-- .slide: style="text-align: left;"> -->
"A web development framework is a set of resources and tools for software developers to build and manage web applications, web services and websites"<br>

<font size="4"><a href="https://searchcontentmanagement.techtarget.com/definition/web-development-framework-WDF">https://searchcontentmanagement.techtarget.com/definition/web-development-framework-WDF</a></font> 

---

## What is the difference between a framework and a library?
## & 
## What is the the difference between a website and a webapp?

---

## Difference between libraries and frameworks
<!-- .slide: style="text-align: left;"> -->
- **Library** : It performs a set of  specific and well-defined operations. Examples : Network protocols, compression, image manipulation, string utilities, regular expression evaluation, math etc<br>
- **Framework**: It is known to be a skeleton where the application defines the content of the operation by filling out the skeleton. The framework only defines the concept but an application further defines the functionality that is useful for end-users<br>

------

- **Inversion of control**: When we call a method from a library, we are in control. But in framework, the control is inverted i.e. the framework calls us<br>

<font size="4"><a href="https://www.geeksforgeeks.org/software-framework-vs-library/">https://www.geeksforgeeks.org/software-framework-vs-library/</a></font> 

------

- **Library Examples** : Network protocols, compression, image manipulation, string utilities, regular expression evaluation, math etc<br>
- **Framework Examples**:  Web application system, Plug-in manager, GUI system<br>

---

### Difference between a website and a webapplication
<img src="images/AppVsSite_Comparison.png" width="700" height="500"/>

---

### Difference between front-end and back-end frameworks
<!-- .slide: style="text-align: left;"> -->
- **Back-End** :<br>
<font size="6">- The frontend is the part of the website visible to the users.<br></a></font> 
<font size="6">- Backend Languages: Python, JavaScript, PHP, Ruby, .NET<br></a></font> 
<font size="6">- Backend frameworks: Django, Ruby On Rails, Express, Spring, ASP.NET Core<br></a></font> 
- **Front-End** :<br>
  <font size="6">- The frontend is the part of the website visible to the users.<br></a></font> 
  <font size="6">- Frontend Languages: HTML, CSS, JavaScript, JQuery<br></a></font> 
  <font size="6">- Frontend Frameworks: React, Vue, BootStrap, Ember, Angular<br></a></font> 

<font size="4"><a href="https://www.monocubed.com/top-python-frameworks/">https://www.monocubed.com/top-python-frameworks/</a></font> 
 
---
 
### Types of python web frameworks 
<!-- .slide: style="text-align: left;"> -->
1. **Full Stack Framework** : Full stack are one of the best Python web application frameworks, known as one-stop-solution for fulfilling all kinds of app building requirements.<br>
2. **Micro-Framework**: These kinds of web frameworks are known as the lightweight framework (non full stack framework) because they do not offer additional patterns and functionalities compared to a full stack framework.<br>
3. **Asynchronous Framework** : Asynchronous web frameworks are now taking over its place as a microframeworks that allows a user to handle large sets of concurrent connections.<br>

<font size="4"><a href="https://www.monocubed.com/10-most-popular-web-frameworks/">https://www.monocubed.com/10-most-popular-web-frameworks/</a></font> 

---

## Examples

<!-- .slide: style="text-align: left;"> -->
1. **Full Stack Framework**:<br>
      - Django<br>
      - Pyramid<br>
2. **Micro-Framework**:<br>
      - Bottle<br>
      - CherryPy<br>
      - Falcon<br>
      - Flask<br>
3. **Asynchronous Framework**:<br>
      - AIOHTTP<br>
      - Tornado<br>

---

## Demonistration

---

### Process Steps
<!-- .slide: style="text-align: left;"> -->
- **Step 1**: Install Flask
- **Step 2**: Create Directory and Script
- **Step 3**: Create HTML Script
- **Step 3**: Write HTML Index Script (Optional)
- **Step 4**: Write Python Script
- **Step 5**: Run Code

---

### Step 1: Install Flask

```
! pip3 install flask 
```

---

### Step 2: Create Directory and Script

<pre><code>mkdir webapp
cd webapp
touch app.py
cd ..
mkdir templates
touch index.html
</pre></code>

---

### Step 3: Write HTML Index Script (Optional)

<pre><code>mkdir webapp
cd webapp
touch app.py
</pre></code>

---

### Step 4: Write Python Script

<pre><code data-line-numbers="1|3|7-9|13-15|18-19">from flask import Flask, render_template
# Starting the app by calling Flask
app = Flask(__name__)
# First: Start the root website from the "/", the first page
# Second: Name the route "index"
# Third: Reference the index.html file
@app.route('/')
def index():
    return render_template('index.html')
# First: Start the website from the "/ar", the second page
# Second: Name the route "/ar"
# Third: Reference the ar.html file
@app.route('/ar')
def ar():
    return render_template('ar.html')
# Run the web server and the app
# '0.0.0.0' ==> The web app is accissible by any device on the local network
if __name__ == '__main__':
    app.run(debug=True, host='0.0.0.0')
</pre></code>

---

### Step 5: Run Code (Terminal)

<pre><code>python3 app.py
> Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
> Restarting with stat
> Debugger is active!
> Debugger pin code: ***-***-***
</pre></code>


## http://127.0.0.1:5000/

---

## Conclusion

---

### What We Learned Today
<!-- .slide: style="text-align: left;"> -->
* What webframes are and thier different types
* That webisites and webframes are not same thing
* The fundemental difference between librareis and frameworks
* That Python has webframes and each serve a different function  
* How to create a simple webapp using Python's Flask webframe

---

### Q&A

<img src="images/Q&A.jpeg" width="700" height="500"/>

---


