# 🌐 Creating a Basic Web Server with Node.js

## 🔥 Setting Up Your First Web Server

Node.js provides a built-in `http` module that allows you to create a simple HTTP server with minimal setup. This is a foundational step in server-side development, where you’ll handle requests and send responses.

![Basic Server](https://miro.medium.com/v2/resize:fit:1200/1*bO2vveanautRnwssj38w0Q.png)

---

### 📝 Steps to Create Your First Server

1. **Initialize Your Project Folder**: Create a new directory for your project, then open your terminal and navigate to it.

2. **Create `server.js` File**: This file will hold the code for your server.

3. **Add the Code**: Copy and paste the following code snippet into `server.js` to create a basic server.

---

## 📄 Code Example: Building a Simple Server

```javascript
// server.js
const http = require('http');

// Create an HTTP server
const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('👋 Hello from Node.js Server!');
});

// Define the port and start the server
server.listen(3000, () => {
  console.log('🚀 Server is running at http://localhost:3000/');
});
