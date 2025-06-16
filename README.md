# Hệ Thống Quản Lý Quán Trà Sữa 🍵

[![GitHub license](https://img.shields.io/github/license/baohiep0401/milktea-project)](https://github.com/baohiep0401/milktea-project/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/baohiep0401/milktea-project)](https://github.com/baohiep0401/milktea-project/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/baohiep0401/milktea-project)](https://github.com/baohiep0401/milktea-project/issues)
[![GitHub Actions](https://github.com/baohiep0401/milktea-project/actions/workflows/ci.yml/badge.svg)](https://github.com/baohiep0401/milktea-project/actions)
[![Code Coverage](https://codecov.io/gh/baohiep0401/milktea-project/branch/main/graph/badge.svg)](https://codecov.io/gh/baohiep0401/milktea-project)
[![Dependencies](https://img.shields.io/david/baohiep0401/milktea-project)](https://david-dm.org/baohiep0401/milktea-project)

Một ứng dụng web full-stack hiện đại giúp quản lý quán trà sữa, được xây dựng với các công nghệ mới nhất và tuân thủ các thực tiễn tốt nhất trong phát triển phần mềm.

## 🎥 Video Demo

[Xem video demo trên YouTube](https://www.youtube.com/watch?v=RzO9qFbhss8)

## �� Tính Năng Nổi Bật

### Quản Lý Người Dùng
- 🔐 Đăng nhập đa nền tảng (Google, Facebook)
- 👥 Phân quyền chi tiết (Admin, Staff, Customer)
- 🔄 Quản lý hồ sơ và đặt lại mật khẩu

### Quản Lý Đơn Hàng
- 📱 Theo dõi đơn hàng realtime
- 💳 Thanh toán đa dạng (VNPAY, Stripe)
- ⭐ Hệ thống đánh giá và phản hồi

### Quản Lý Kho & Sản Phẩm
- 📊 Theo dõi tồn kho tự động
- 🚨 Cảnh báo tồn kho thấp
- 📈 Báo cáo chi tiết

### Phân Tích & Báo Cáo
- 📊 Dashboard trực quan
- 📈 Phân tích doanh thu
- 👥 Phân tích khách hàng

## 🛠️ Tech Stack

### Frontend
- React.js 18.2.0
- Material-UI (MUI) 5.11.4
- Redux Toolkit 1.9.3
- React Router 6.6.2
- Formik 2.2.9
- Axios 1.3.2

### Backend
- Node.js 14+
- Express.js
- Sequelize ORM
- MySQL 8.0
- JWT Authentication
- Docker

## 🚀 Bắt Đầu

### Yêu Cầu
- Node.js (v14+)
- MySQL 8.0
- Docker (tùy chọn)

### Cài Đặt

1. Clone repository
```bash
git clone https://github.com/baohiep0401/milktea-project.git
cd milktea-project
```

2. Cài đặt backend
```bash
cd be
npm install
# Cấu hình database trong config/config.json
npx sequelize db:migrate
npx sequelize db:seed:all
npm start
```

3. Cài đặt frontend
```bash
cd fe
npm install
npm start
```

## 📁 Cấu Trúc Dự Án

```
milktea-project/
├── be/                        # Backend
│   ├── assets/               # Tài nguyên tĩnh
│   │   ├── css/             # Stylesheets
│   │   ├── img/             # Hình ảnh
│   │   ├── js/              # JavaScript files
│   │   └── scss/            # SCSS files
│   ├── config/              # Cấu hình
│   │   ├── config.json      # Cấu hình database
│   │   ├── configfb.js      # Cấu hình Facebook
│   │   └── configpayment.js # Cấu hình thanh toán
│   ├── controllers/         # Logic xử lý
│   │   ├── account.controllers.js
│   │   ├── cart.controllers.js
│   │   ├── order.controllers.js
│   │   └── ...
│   ├── middlewares/         # Middleware
│   │   ├── auth.js
│   │   └── validate.js
│   ├── migrations/          # Database migrations
│   ├── models/              # Database models
│   │   ├── account.js
│   │   ├── cart.js
│   │   ├── order.js
│   │   └── ...
│   ├── public/              # Static files
│   ├── routers/             # API routes
│   │   ├── account.js
│   │   ├── cart.js
│   │   ├── order.js
│   │   └── ...
│   ├── seeders/             # Database seeders
│   ├── views/               # View templates
│   ├── .gitignore
│   ├── docker-compose.yml
│   ├── package.json
│   ├── README
│   └── server.js            # Entry point
│
├── fe/                       # Frontend
│   ├── public/              # Static files
│   │   ├── index.html
│   │   ├── favicon.ico
│   │   └── ...
│   ├── src/                 # Source code
│   │   ├── components/      # React components
│   │   │   ├── common/      # Shared components
│   │   │   ├── layout/      # Layout components
│   │   │   └── ...
│   │   ├── pages/          # Page components
│   │   │   ├── Home/
│   │   │   ├── Cart/
│   │   │   └── ...
│   │   ├── redux/          # State management
│   │   │   ├── actions/
│   │   │   ├── reducers/
│   │   │   └── store.js
│   │   ├── utils/          # Helper functions
│   │   ├── App.js
│   │   └── index.js
│   ├── .gitignore
│   ├── package.json
│   └── README.md
│
└── README.md                # Project documentation
```

## 💻 Phát Triển

### Quy Ước Code
- ESLint + Prettier
- Conventional Commits
- Git Flow workflow

### Quy Trình Git
1. Tạo branch từ `develop`
2. Commit theo chuẩn conventional commits
3. Tạo pull request
4. Code review
5. Merge vào `develop`

## 🧪 Kiểm Thử

```bash
# Backend tests
cd be
npm test

# Frontend tests
cd fe
npm test
```

## 📦 Triển Khai

### Docker
```bash
docker-compose up -d
```

### Thủ công
```bash
# Backend
cd be
npm run build
npm start

# Frontend
cd fe
npm run build
serve -s build
```

## 🔒 Bảo Mật
- JWT Authentication
- Password Hashing
- CORS Configuration
- Rate Limiting
- Input Validation
- SQL Injection Prevention
- XSS Protection

## 📚 Tài Liệu
- [Báo Cáo Chi Tiết](N19DCCN053.pdf)
- [Slide Thuyết Trình](https://www.canva.com/design/DAGqJ9Uesaw/O1BuZ_ftKC3BZSWJ-V-E7Q/edit)
- [API Documentation](docs/api.md)
- [Database Schema](docs/database.md)
- [Deployment Guide](docs/deployment.md)

## 🤝 Đóng Góp
1. Fork repository
2. Tạo branch mới (`git checkout -b feature/AmazingFeature`)
3. Commit thay đổi (`git commit -m 'Add some AmazingFeature'`)
4. Push lên branch (`git push origin feature/AmazingFeature`)
5. Tạo Pull Request

## 📄 Giấy Phép
MIT License - Xem [LICENSE](LICENSE) để biết thêm chi tiết.

## 📞 Liên Hệ
- GitHub: [@baohiep0401](https://github.com/baohiep0401)
- Email: baohiep0401@gmail.com

## 🙏 Ghi Nhận
- Cảm ơn tất cả contributors
- Cảm ơn cộng đồng mã nguồn mở

---

⭐️ Từ [Bảo Hiệp](https://github.com/baohiep0401)

## 📈 Lộ Trình Phát Triển
- [ ] Ứng dụng di động
- [ ] Gợi ý thông minh bằng AI
- [ ] Phân tích nâng cao
- [ ] Đa ngôn ngữ
- [ ] Giao diện tối (dark mode)

## 🔄 Lịch Sử Thay Đổi
### [1.0.0] - 2024-03-20
- Phát hành bản đầu tiên
- Hoàn thiện các tính năng cơ bản
- Thêm tài liệu hướng dẫn

## 📊 Hiệu Năng
- Thời gian tải trang: < 2s
- Thời gian phản hồi API: < 200ms
- Độ phủ kiểm thử: > 80%
- Điểm Lighthouse: > 90
- Tối ưu: tách code, lazy load, tối ưu ảnh, cache, index database

## 🛠️ Xử Lý Sự Cố
1. Lỗi kết nối database: kiểm tra thông tin, trạng thái DB, mạng
2. Lỗi build: xóa node_modules, cập nhật phụ thuộc, kiểm tra version Node.js

### FAQ
1. Làm sao để reset mật khẩu?
2. Cách cập nhật kho hàng?
3. Cách xuất báo cáo?
4. Thêm sản phẩm mới như thế nào?
5. Quản lý nhân viên ra sao?

## 📱 Hỗ Trợ Mobile
- Thiết kế responsive, mobile-first
- Hỗ trợ PWA: cài đặt, offline, push notification, background sync 