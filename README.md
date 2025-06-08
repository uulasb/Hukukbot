# HukukBot - Turkish Legal AI Assistant 🏛️

An advanced AI-powered legal assistance platform for Turkish law, providing instant access to legal information and guidance through state of the art natural language processing.

🌐 Live Application
Access the application at: https://ulasbingol34--turkish-law-chatbot-fastapi-app.modal.run/

## 🌟 Features

- **AI-Powered Legal Assistant**: Uses DeepSeek R1's advanced reasoning capabilities to understand and answer complex legal questions in Turkish
- **Real-time Legal Database Access**: Integrated with proprietary API to search and retrieve Turkish court decisions
- **Source Citations**: All legal responses include proper citations
- **WebSocket Support**: Real-time chat interface with streaming responses
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Dark Mode Support**: Automatic theme switching based on user preferences
- **Docker Deployment**: Easy one-command deployment with Docker Compose

## 🏗️ Architecture

```
┌─────────────────┐     ┌──────────────────┐     ┌─────────────────┐
│   Web Frontend  │────▶│   Backend API    │────▶│   OpenRouter    │
│   (React/Vue)   │◀────│   (FastAPI)      │◀────│     AI API 
└─────────────────┘     └──────────────────┘     └─────────────────┘
                                │
                                ▼
                        ┌──────────────────┐
                        │ Legal Database   │
                        │     API          │
                        └──────────────────┘
```


## 📁 Project Structure

```
turkish-law-chatbot/
├── backend/
│   ├── app.py                 # FastAPI main application
│   ├── legal_database_client.py # Legal database integration
│   ├── deepseek_client.py     # OpenRouter/DeepSeek client
│   ├── config.py              # Configuration management
│   ├── requirements.txt       # Python dependencies
│   └── Dockerfile            
├── frontend/
│   ├── index.html             # Main HTML file
│   ├── app.js                 # JavaScript application
│   ├── styles.css             # Styling
│   └── Dockerfile            
├── legal-database-client/   # Legal database client library
├── docker-compose.yml         # Docker orchestration
├── nginx.conf                 # Nginx configuration
├── .env.example               # Environment variables example
└── README.md                  # This file
```

## ⚠️ Disclaimer

This chatbot provides general legal information based on Turkish court decisions and should not be considered as legal advice. For specific legal matters, please consult with a qualified Turkish lawyer.

---

**Version**: 1.0.0  
**Architecture**: Microservices  
**Deployment**: Cloud-native  
**Compliance**: GDPR, KVKK  

**Built with ❤️ using modern web technologies for the future of legal services and democracy in Turkey**
