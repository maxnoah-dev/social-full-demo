# Social Demo Project

Demo project với Frontend (React + TypeScript) và Backend (Express.js + Node.js) kết nối với MySQL.

## Cấu trúc dự án

```
social-full-demo/
├── fe/                 # Frontend React + TypeScript
├── be/                 # Backend Express.js + Node.js
└── database.sql        # MySQL database schema
```

## Setup

### 1. Database

Chạy file `database.sql` trong MySQL để tạo database và tables:
```bash
mysql -u root -p < database.sql
```

### 2. Backend

```bash
cd be
npm install
cp .env.example .env
# Cập nhật thông tin database trong .env
npm run dev
```

Backend chạy tại: http://localhost:3001

### 3. Frontend

```bash
cd fe
npm install
npm start
```

Frontend chạy tại: http://localhost:3000

## API Endpoints

- `GET /api/health` - Health check
- `GET /api/users` - Lấy danh sách users
- `GET /api/posts` - Lấy danh sách posts
- `POST /api/posts` - Tạo post mới

## Features

- Hiển thị danh sách users
- Hiển thị danh sách posts
- Tạo post mới
- Kết nối Frontend và Backend
- Sử dụng MySQL database
