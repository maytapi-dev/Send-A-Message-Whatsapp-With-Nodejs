# 💬 WhatsApp Text Messaging API for JavaScript | Send Text Messages via WhatsApp API

> **Professional WhatsApp API Integration** - Send text messages programmatically using JavaScript/Node.js with Maytapi's powerful WhatsApp API. Perfect for web applications, chatbots, and enterprise automation solutions.

[![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Node.js](https://img.shields.io/badge/Node.js-16%2B-green.svg)](https://nodejs.org/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![WhatsApp API](https://img.shields.io/badge/WhatsApp-API-25D366.svg)](https://maytapi.com/)
[![Maytapi](https://img.shields.io/badge/Powered%20by-Maytapi-orange.svg)](https://maytapi.com/)

## 🌟 Overview

This JavaScript/Node.js library provides seamless integration with **WhatsApp API** for sending text messages programmatically. Designed specifically for modern web applications, chatbots, marketing automation platforms, and enterprise communication systems that require reliable WhatsApp messaging capabilities.

**Perfect for:** Customer notifications, automated responses, marketing campaigns, order confirmations, and real-time business communication workflows.

## 🔗 Essential Links & Resources

| Resource | Description | Link |
|----------|-------------|------|
| 🌐 **Official Website** | Maytapi WhatsApp API Platform | [Visit Site](https://maytapi.com/) |
| 🔐 **Developer Console** | API management and configuration | [Login Portal](https://console.maytapi.com/login) |
| 💰 **Pricing & Plans** | Flexible pricing for all business sizes | [View Pricing](https://maytapi.com/whatsapp-api-pricing) |
| 📖 **API Documentation** | Complete developer documentation | [Read Docs](https://maytapi.com/whatsapp-api-documentation) |

## ⭐ Key Features & Capabilities

### 💬 **Text Messaging Methods**
- ✅ **Simple Text Sending** - Send plain text messages instantly
- ✅ **Rich Text Formatting** - Support for bold, italic, and special characters
- ✅ **Emoji Support** - Full Unicode emoji compatibility
- ✅ **Bulk Text Broadcasting** - Send to multiple recipients simultaneously
- ✅ **Message Templates** - Predefined message formats

### 🛠️ **Developer-Friendly Features**
- ✅ **Modern JavaScript/ES6+** - Built with latest JavaScript standards
- ✅ **Promise-based API** - Full Promise and async/await support
- ✅ **Comprehensive Error Handling** - Detailed error messages and stack traces
- ✅ **TypeScript Support** - Full TypeScript definitions included
- ✅ **URL-based Text Sending** - Send text from external sources
- ✅ **Base64 Text Encoding** - Support for encoded text content

### 🔒 **Security & Performance**
- ✅ **Secure Token Authentication** - Token-based security
- ✅ **HTTPS Encryption** - All communications secured with TLS
- ✅ **Rate Limiting** - Built-in request throttling
- ✅ **Retry Mechanisms** - Automatic retry with exponential backoff
- ✅ **Input Sanitization** - XSS and injection protection
- ✅ **Message Validation** - Character limit and format checking

---

## 📦 Installation
```bash
npm install whatsapp-text-api
```

## 🔧 Usage Example
```javascript
const WhatsAppAPI = require('whatsapp-text-api');

// Initialize the API
const api = new WhatsAppAPI({
  productId: "YOUR_PRODUCT_ID",
  phoneId: "YOUR_PHONE_ID",
  apiToken: "YOUR_API_TOKEN"
});

// Send a text message via URL
api.sendTextMessage({
  to: "1234567890",
  textUrl: "https://example.com/text.jpg",
  caption: "Check out this text!"
})
.then(response => {
  console.log("Message sent successfully:", response);
})
.catch(error => {
  console.error("Message sending failed:", error);
});

// Send a text message from Base64 data
api.sendTextFromBase64({
  to: "1234567890",
  base64Data: "data:image/...",
  caption: "Base64 text message"
})
.then(response => {
  console.log("Base64 message sent:", response);
});
```

## 🔒 Authentication
Ensure you have the following credentials:
- Product ID
- Phone ID
- API Token

## 📝 Methods
- `sendTextMessage()`: Send text via URL
- `sendTextFromBase64()`: Send text using Base64 encoding

## 🔍 Error Handling
The library provides comprehensive error logging and throws detailed error messages.

## 📜 License
MIT License

## 🤝 Support
For issues or questions, please open a GitHub issue.
