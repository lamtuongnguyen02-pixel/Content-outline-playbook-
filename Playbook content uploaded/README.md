# 📊 Content Outline Playbook - AI-Powered Content Strategy Tool

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-active-brightgreen.svg)
![Version](https://img.shields.io/badge/version-2.0-orange.svg)

## 🚀 Giới Thiệu

**Content Outline Playbook** là một công cụ quản lý nội dung toàn diện được xây dựng để giúp:

- 📋 **Xây dựng Chiến lược Nội dung** với hệ thống Pillar (Trụ cột)
- 🎯 **Phân loại Angles** (Góc tiếp cận) theo tâm lý khách hàng
- 🤖 **Sinh Tiêu đề** tự động bằng Claude AI
- 📅 **Lên Kế hoạch Bài Viết** theo lịch trình chi tiết
- 📊 **Theo dõi Tiến độ** với hệ thống quản lý task
- 💾 **Lưu trữ & Export** dữ liệu dễ dàng

---

## ✨ Tính Năng Chính

### 1️⃣ **Hệ Thống Pillar (5 Cột Nội dung)**
- ✅ Xác định 5 trụ cột nội dung chính
- ✅ Gán màu sắc nhận diện riêng cho mỗi Pillar
- ✅ Quản lý từ khoá chính & mục tiêu
- ✅ Tính toán tỷ lệ bài viết tối ưu
- ✅ Export & Import cấu hình Pillar

### 2️⃣ **Ma Trận Content Angles**
- ✅ Tạo 4-8 góc tiếp cận per Pillar
- ✅ Phân tích tâm lý & hành vi khách hàng
- ✅ Link tự động đến Pillar tương ứng
- ✅ Quản lý độ ưu tiên (Viral/Chuyển đổi/Chuyên sâu)
- ✅ Tích hợp Google Search để research
- ✅ **Nút "Tạo bài"** để chuyển sang Planner

### 3️⃣ **AI Generator - Sinh Tiêu đề Thông Minh**
- 🤖 **Claude AI Integration** - Tích hợp API Anthropic
- ✅ Sinh 5 tiêu đề viral per request
- ✅ Cá nhân hóa theo Pillar + Angle đã chọn
- ✅ Mẫu có sẵn cho backup khi AI offline
- ✅ Copy & thêm trực tiếp vào Planner
- ⚠️ Xử lý lỗi thông minh với hướng dẫn fallback

### 4️⃣ **Kế Hoạch Lên Bài (Planner)**
- 📅 Quản lý timeline bài viết (hôm nay/tuần này/tháng này)
- 🎨 Chọn format: Video/Carousel/Bài chuyên sâu/Livestream
- 🔄 Liên kết tự động từ Ma trận Angles
- 📊 Tính toán tỷ lệ Pillar thực tế
- ✏️ Chỉnh sửa nhanh inline
- 🗑️ Quản lý trạng thái (Nháp/Đã xuất/Hoàn thành)

### 5️⃣ **Dashboard & Analytics**
- 📈 Thống kê bài viết theo tháng/quý
- 🎯 Kiểm tra tỷ lệ Pillar vs Kế hoạch
- 📊 Xu hướng nội dung theo thời gian
- 🔔 Notifications cho bài viết sắp đến hạn

### 6️⃣ **Data Management**
- 💾 **Auto-save** vào Browser LocalStorage
- 📥 **Export JSON** - Lưu backup toàn bộ dữ liệu
- 📤 **Import JSON** - Phục hồi từ backup
- 🔄 **Sync History** - Lịch thay đổi chi tiết
- 🎛️ **Cấu hình Ứng dụng** - Tuỳ chỉnh màu sắc, ngôn ngữ

---

## 🎯 Quick Start

### Cách 1: Chạy Trên GitHub Pages (Recommended)

1. **Truy cập trực tiếp**: [yourusername.github.io/content-outline-playbook](https://yourusername.github.io/content-outline-playbook)
2. **Không cần cài đặt** - Chạy ngay trong trình duyệt
3. **Dữ liệu lưu trên máy tính** bạn (Browser LocalStorage)

### Cách 2: Chạy Local (Phát triển)

```bash
# 1. Clone repository
git clone https://github.com/yourusername/content-outline-playbook.git
cd content-outline-playbook

# 2. Dùng Live Server (VS Code) hoặc Python
# Với Python 3:
python -m http.server 8000

# Với Python 2:
python -m SimpleHTTPServer 8000

# 3. Mở browser: http://localhost:8000
```

> ⚠️ **Lưu ý**: Không chạy file trực tiếp từ `file://` vì sẽ lỗi LocalStorage

---

## 📖 Hướng Dẫn Sử Dụng

### 📋 Bước 1: Setup Pillars

1. Tìm tab **"Xây dựng Playbook"**
2. Nhập 5 trụ cột nội dung (VD: Sức khỏe, Dinh dưỡng, Lifestyle, Y tế, Công trình)
3. Chọn màu sắc nhận diện cho mỗi Pillar
4. Nhập từ khoá chính & mục tiêu
5. Lưu (tự động save)

### 🎯 Bước 2: Tạo Ma Trận Angles

1. Mở tab **"Ma Trận Content Angles"**
2. Chọn Pillar → Nhấn **"+ Thêm Angle"**
3. Điền:
   - **Góc tiếp cận**: VD "FOMO / Sợ Già"
   - **Tâm lý**: Mô tả nhu cầu khách hàng
   - **Hook**: Tiêu đề mẫu
   - **Kênh**: TikTok/Reels/YouTube/etc
   - **Độ ưu tiên**: Cao/Trung bình/Thấp
4. Lưu

### 🤖 Bước 3: Sinh Tiêu đề AI

1. Chọn 1 Pillar + 1 Angle
2. Nhấn **"AI Tạo tiêu đề"**
3. Chờ Claude AI sinh 5 tiêu đề
4. **Copy** hoặc **Lên bài** trực tiếp vào Planner

### 📅 Bước 4: Lên Kế hoạch Bài Viết

**Cách 1 - Từ Ma trận**:
- Nhấn **"Tạo bài"** trên mỗi Angle
- Tự động thêm vào Planner

**Cách 2 - Manual**:
- Tab "Kế hoạch Lên bài" → **"+ Thêm bài"**
- Nhập tiêu đề, chọn Pillar, format, ngày xuất bản

### 📊 Bước 5: Quản lý & Theo dõi

1. **Chỉnh sửa inline**: Double-click vào ô bất kỳ
2. **Thay đổi trạng thái**: Từ "Nháp" → "Đã xuất" → "Hoàn thành"
3. **Xem Analytics**: Tab "Dashboard" để kiểm tra tỷ lệ
4. **Export dữ liệu**: Nút "Export JSON" để backup

---

## 🔧 Tích Hợp Claude AI

### Yêu cầu

Để sử dụng tính năng **AI Generator**, bạn cần:

1. **Tài khoản Anthropic**: https://console.anthropic.com
2. **API Key**: Tạo tại console.anthropic.com/account/keys

### Cấu hình

1. Mở ứng dụng → Tab **"Cài đặt"**
2. Nhập **API Key Anthropic** vào ô **"Claude API Key"**
3. Test bằng cách nhấn **"Test Kết nối"**
4. Lưu

### Nếu API Key không hoạt động?

- ✅ Dùng **"Mẫu có sẵn"** (Legacy mode)
- ✅ Nhấn **"Tạo bài"** từ Ma trận Angles
- ✅ Hệ thống sẽ gợi ý các phương án backup tự động

---

## 📁 Cấu Trúc Thư Mục

```
content-outline-playbook/
├── index.html                 # ← File HTML chính (3000+ dòng)
├── README.md                  # Hướng dẫn này
├── .gitignore                 # Git ignore file
├── LICENSE                    # MIT License
└── docs/
    ├── SETUP.md              # Hướng dẫn setup chi tiết
    ├── FEATURES.md           # Danh sách tính năng đầy đủ
    ├── API_INTEGRATION.md    # Hướng dẫn tích hợp API
    └── TROUBLESHOOTING.md    # Xử lý sự cố
```

---

## 💾 Lưu Trữ Dữ Liệu

### LocalStorage (Mặc định)
- **Vị trí**: Browser của bạn
- **Dung lượng**: ~10MB per domain
- **Tự động lưu**: Mỗi khi bạn thay đổi dữ liệu
- **Công cụ**: DevTools → Application → LocalStorage

### Export/Import
```
Nút "Export JSON" → Tải file backup
Nút "Import JSON" → Phục hồi từ file cũ
```

### Backup Tự động
- Lịch sử tất cả thay đổi được lưu trong **"History"** tab
- Có thể rollback về phiên bản cũ

---

## 🔒 Bảo Mật

- ✅ **100% chạy trên Client** - Không gửi dữ liệu lên server
- ✅ **API Key lưu LOCAL** - Không lưu lên GitHub
- ✅ **LocalStorage mã hoá** - Không ai khác truy cập được
- ⚠️ **Lưu ý**: Nếu xoá browser data → Mất dữ liệu LOCAL

---

## 🐛 Xử lý Sự Cố

### Lỗi 1: "Uncaught Error" hoặc "SyntaxError"
```
→ Giải pháp: Xoá cache & reload (Ctrl+Shift+Del)
```

### Lỗi 2: AI Generator không hoạt động
```
→ Giải pháp: 
  1. Kiểm tra API Key đã nhập chưa
  2. Kiểm tra API Key có hợp lệ không
  3. Dùng "Mẫu có sẵn" để backup
  4. Dùng "Tạo bài từ Angle" thay thế
```

### Lỗi 3: Dữ liệu bị mất
```
→ Giải pháp:
  1. Check tab "History" để xem thay đổi
  2. Import file backup JSON
  3. Dùng "Rollback to Previous" (nếu có)
```

### Lỗi 4: LocalStorage full (>10MB)
```
→ Giải pháp:
  1. Export JSON để backup
  2. Xoá dữ liệu cũ (Archive)
  3. Reload ứng dụng
```

---

## 📈 So Sánh Vs. Cách Làm Manual

| Tính năng | Playbook | Manual |
|----------|----------|--------|
| Sinh tiêu đề AI | ✅ Auto | ❌ 30 phút/tiêu đề |
| Quản lý Pillar | ✅ Visual | ❌ Excel phức tạp |
| Research link | ✅ Google Search tích hợp | ❌ Tab khác |
| Tracking tỷ lệ | ✅ Real-time | ❌ Tính tay |
| Backup dữ liệu | ✅ Auto + Export | ❌ Dễ mất |
| Collaboration | ⚠️ Sắp có | ❌ Share file khó |

---

## 🚀 Roadmap (Coming Soon)

- [ ] 🌐 **Cloud Sync** - Lưu trữ trên Supabase/Firebase
- [ ] 👥 **Team Collaboration** - Chia sẻ & comment
- [ ] 📊 **Advanced Analytics** - Dashboard chi tiết hơn
- [ ] 🎨 **Design System** - Template bài viết tích hợp
- [ ] 🤖 **More AI Models** - Hỗ trợ GPT-4, Gemini
- [ ] 📱 **Mobile App** - iOS/Android version
- [ ] 🔌 **API Integration** - Kết nối Notion, Google Sheets
- [ ] 🌍 **Multi-language** - Hỗ trợ nhiều ngôn ngữ

---

## 📞 Hỗ Trợ & Liên Hệ

- 📧 **Email**: support@example.com
- 💬 **Discord**: [Server Community](https://discord.gg/xxx)
- 🐛 **Report Issues**: [GitHub Issues](https://github.com/yourusername/content-outline-playbook/issues)
- 💡 **Feature Request**: [GitHub Discussions](https://github.com/yourusername/content-outline-playbook/discussions)

---

## 📄 License

MIT License - Tự do sử dụng & chỉnh sửa cho mục đích cá nhân/thương mại

```
Copyright (c) 2024 Content Outline Playbook

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

## 🙏 Cảm Ơn

Được xây dựng bằng ❤️ bằng:
- 🎨 **Tailwind CSS** - Styling
- 🤖 **Claude AI (Anthropic)** - AI Integration
- 💾 **Browser LocalStorage** - Data Management
- 📊 **Vanilla JavaScript** - Core Logic

---

**Made with ❤️ for Content Creators & Marketers**

Last Updated: 2024
