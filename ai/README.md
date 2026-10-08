# AI Assistant App

A simple, interactive AI Assistant web application built with vanilla HTML, CSS, and JavaScript.

## Features

- 💬 Clean chat interface with message history
- 📱 Responsive design for mobile and desktop
- ⚡ Real-time message sending
- 🎨 Modern UI with gradient background
- 🚀 Easy to extend with API integrations

## File Structure

```
ai/
├── index.html      # Main HTML file
├── styles.css      # Styling and layout
├── app.js          # Application logic
└── README.md       # Documentation
```

## Getting Started

1. Open `index.html` in your web browser
2. Type a message in the input field
3. Click "Send" or press Enter to send your message
4. The AI Assistant will respond

## Current Features

- Basic message display and chat interface
- Simple pattern-based responses
- Conversation history tracking
- Keyboard support (Enter to send)

## Future Enhancements

- [ ] Integration with AI APIs (OpenAI, Google, etc.)
- [ ] User authentication
- [ ] Save conversation history
- [ ] Multiple conversation threads
- [ ] Custom AI personality settings
- [ ] Voice input/output support
- [ ] Dark mode theme
- [ ] Message editing and deletion

## API Integration

To connect this app to a real AI service:

1. Update the `generateResponse()` method in `app.js`
2. Add your API endpoint and authentication
3. Handle API responses and errors

Example:
```javascript
async generateResponse(userMessage) {
    const response = await fetch('YOUR_API_ENDPOINT', {
        method: 'POST',
        headers: {
            'Content-Type': 'application/json',
            'Authorization': 'Bearer YOUR_API_KEY'
        },
        body: JSON.stringify({ message: userMessage })
    });
    
    const data = await response.json();
    return data.reply;
}
```

## License

This project is open source and available under the MIT License.
