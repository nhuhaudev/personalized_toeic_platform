# Backend

## Cài đặt & Chạy

```bash
# 1. Cài đặt thư viện
npm install

# 2. Chạy server (Development)
npm run dev
```

Server chạy tại: `http://localhost:4000`

## Cấu hình (.env)

Tạo file `.env` với các biến môi trường sau (lấy từ file thực tế):

```env
# Server Configuration
PORT=4000
NODE_ENV=Development

# Database
MONGODB_URI=mongodb+srv://user:pass@cluster.mongodb.net/toeic_web

# JWT Secrets
JWT_ACCESS_SECRET=your_access_secret
JWT_REFRESH_SECRET=your_refresh_secret
RESET_SECRET=your_reset_secret

# URLs
BACKEND_URL=http://localhost:4000
CLIENT_URL=http://localhost:3000
ADMIN_URL=http://localhost:3001

# Google OAuth
GOOGLE_CLIENT_ID=your_client_id
GOOGLE_CLIENT_SECRET=your_client_secret

# Email Configuration
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your_email
SMTP_PASS=your_password
MAIL_FROM="toeic.prep<your_email>"

# PayOS Configuration
PAYOS_CLIENT_ID=your_id
PAYOS_API_KEY=your_key
PAYOS_CHECKSUM_KEY=your_checksum

# AWS S3
AWS_REGION=ap-southeast-2
AWS_S3_BUCKET=project.toeic
AWS_S3_PREFIX=community/
AWS_ACCESS_KEY_ID=your_aws_key
AWS_SECRET_ACCESS_KEY=your_aws_secret

# LiveKit Cloud
LIVEKIT_API_KEY=your_lk_key
LIVEKIT_API_SECRET=your_lk_secret
LIVEKIT_HOST=https://your-project.livekit.cloud
LIVEKIT_WS_URL=wss://your-project.livekit.cloud

# System & AI
COURSES_PREFIX=Khoá học TA/
COURSES_DEV_SEED=1
GROQ_API_KEY=your_groq_key
GROQ_MODEL=llama-3.3-70b-versatile
GROQ_BASE_URL=https://api.groq.com/openai/v1

# Logic Config
PROGRESS_ELIGIBILITY_MINUTES=7200
PRACTICE_INACTIVITY_DAYS=3
PRACTICE_NUDGE_COOLDOWN_HOURS=1
PARTS_COLL=practice_parts
STIMULI_COLL=practice_stimuli

# Deploy / Admin
DEPLOY_WEBHOOK_TOKEN=your_token
ADMIN_EMAIL=your_email
```
