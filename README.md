# 🔐 ZKShare - Zero-Knowledge File Sharing Platform

A secure, privacy-focused file sharing platform with end-to-end encryption using zero-knowledge architecture. Deployed with Kubernetes and automated CI/CD.

## 🌟 Features

- **Zero-Knowledge Encryption**: Files are encrypted client-side with RSA-OAEP-2048 and AES-256-GCM
- **Public Link Sharing**: Share files via password-protected public links with download limits
- **Secure File Sharing**: Share encrypted files with other users
- **Dark Mode**: Persistent theme preference with light/dark mode toggle
- **Real-time Notifications**: WebSocket-based notification system
- **Usage Tracking**: Monitor storage usage and file statistics
- **Key Backup Management**: Secure backup and recovery of encryption keys
- **Responsive UI**: Modern, mobile-friendly interface built with React and Tailwind CSS
- **Kubernetes Deployment**: Production-ready container orchestration
- **CI/CD Pipeline**: Automated builds and deployments with GitHub Actions

## 🏗️ Architecture
 
### Backend (Go Microservices)
- **API Gateway** (Port 8000): Routes requests to appropriate services
- **Auth Service** (Port 8001): User authentication and JWT management
- **File Service** (Port 8002): File upload, download, and storage
- **Metadata Service** (Port 8003): File metadata and sharing management
- **Subscription Service** (Port 8004): User subscription management
- **Notification Service** (Port 8005): Real-time notifications via WebSocket

### Frontend (React)
- **React 19** with Vite
- **Tailwind CSS** for styling
- **shadcn/ui** component library
- **Client-side encryption** with Web Crypto API
- **Dark mode** with persistent localStorage
