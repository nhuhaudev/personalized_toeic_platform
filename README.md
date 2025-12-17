# Hướng dẫn chạy dự án

Dưới đây là các lệnh đơn giản để chạy toàn bộ hệ thống.

## 1. Cài đặt

Mở terminal tại thư mục gốc và chạy lần lượt các lệnh sau để cài đặt thư viện cho cả 3 phần:

```bash
cd backend && npm install
cd ../frontend && npm install
cd ../admin && npm install
cd ..
```

## 2. Cấu hình

Đảm bảo bạn đã tạo các file `.env` (backend) và `.env.local` (frontend, admin) dựa trên các file mẫu `env.example` hoặc hướng dẫn trước đó.

## 3. Chạy dự án

Bạn cần mở 3 cửa sổ terminal riêng biệt cho mỗi phần:

**Terminal 1 (Backend):**
```bash
cd backend
npm run dev
```

**Terminal 2 (Frontend):**
```bash
cd frontend
npm run dev
```

**Terminal 3 (Admin):**
```bash
cd admin
npm run dev
```

Hệ thống sẽ chạy tại:
- Frontend: http://localhost:3000
- Admin: http://localhost:3001
- Backend: http://localhost:4000
