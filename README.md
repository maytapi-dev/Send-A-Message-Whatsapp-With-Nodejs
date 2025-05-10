# WhatsApp Text Messaging API
Effortlessly send text messages via WhatsApp using Maytapi's powerful API.

## 🚀 Features
- Send text messages with ease
- Support for URL-based and Base64 encoded text
- Flexible messaging options
- Comprehensive error handling

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
