# TOEIC AI Platform 

A comprehensive, AI-powered platform designed to revolutionize TOEIC preparation. This system provides an interactive learning experience, real-time communication, and intelligent performance analysis. 

Built with a robust microservices-inspired architecture, the project is divided into three main applications: a user-facing **Frontend**, a powerful **Backend**, and a secure **Admin** dashboard.

## Features

- **AI-Powered Learning**: Integrates OpenAI and Groq APIs for intelligent question generation, automated grading, and personalized feedback.
- **Real-time Interaction**: Leverages Socket.io and LiveKit for seamless real-time chat, notifications, and live audio/video streaming for online classes.
- **Secure Payment Gateway**: Integrates PayOS for seamless and secure payment processing.
- **Role-based Access Control**: Distinct interfaces and permissions for Students, Teachers, and Administrators.
- **Interactive Dashboards**: Data visualization using Chart.js and Recharts to track student progress and platform metrics.

## Technology Stack

### Frontend (User Application)
- **Framework:** Next.js 15 (React 19)
- **Styling:** Tailwind CSS, Framer Motion (Animations)
- **Real-time:** Socket.io-client, LiveKit Components
- **Data Visualization:** Chart.js, Recharts
- **Content:** React Markdown, Next-intl (i18n)

### Backend (RESTful API)
- **Runtime:** Node.js, Express.js (TypeScript)
- **Database:** MongoDB (Mongoose)
- **Authentication:** JWT, Passport.js (Google OAuth2.0)
- **Real-time:** Socket.io, LiveKit Server SDK
- **AI Integrations:** OpenAI, Groq SDK
- **Storage:** AWS S3
- **Payment:** PayOS

### Admin Dashboard
- **Framework:** Next.js 15
- **Styling:** Tailwind CSS
- **Notifications:** SweetAlert2
- **Icons:** Lucide React, React Icons

## Project Structure

```text
websites/
├── frontend/      # Next.js web application for end-users
├── backend/       # Express/Node.js backend API
├── admin/         # Next.js admin dashboard
├── deploy.sh      # Deployment script
└── ecosystem.config.js # PM2 configuration for process management
```

## Getting Started

### Prerequisites
- Node.js (v20+)
- MongoDB
- AWS S3 Bucket
- LiveKit Server

### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd websites
   ```

2. **Setup Backend:**
   ```bash
   cd backend
   npm install
   # Create a .env file with required environment variables
   npm run dev
   ```

3. **Setup Frontend:**
   ```bash
   cd frontend
   npm install
   # Create a .env.local file
   npm run dev
   ```

4. **Setup Admin:**
   ```bash
   cd admin
   npm install
   # Create a .env.local file
   npm run dev
   ```

## Environment Variables

You will need to configure environment variables for each application in their respective `.env` files. Key variables include:
- `MONGODB_URI`
- `JWT_SECRET`
- `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`
- `OPENAI_API_KEY`, `GROQ_API_KEY`
- `LIVEKIT_API_KEY`, `LIVEKIT_API_SECRET`
- `PAYOS_CLIENT_ID`, `PAYOS_API_KEY`, `PAYOS_CHECKSUM_KEY`

## Contributing
Contributions, issues, and feature requests are welcome! Feel free to check [issues page](#).

## License
This project is licensed under the ISC License.
