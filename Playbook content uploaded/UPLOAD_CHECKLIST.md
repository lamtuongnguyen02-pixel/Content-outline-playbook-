# ⚡ 1-Click Upload Checklist

**Muốn upload nhanh nhất? Làm theo list này!**

---

## 📋 Trước Upload (5 phút)

- [ ] Kiểm tra file `index.html` hoạt động local (dùng Live Server)
- [ ] Export JSON backup (Cài đặt → Export)
- [ ] Kiểm tra không có lỗi console (F12 → Console)
- [ ] Kiểm tra API Key (nếu dùng) không hardcode trong code

---

## 🚀 Upload Thực Tế (Chọn 1 cách)

### Cách A: Dùng GitHub Web (Dễ Nhất - 3 bước)

- [ ] Tạo repo mới: https://github.com/new
  - Tên: `content-outline-playbook`
  - Public ✓
- [ ] Upload file:
  - [ ] Nhấn "Add file" → "Upload files"
  - [ ] Drag & drop: `index.html`, `README.md`, `LICENSE`, `.gitignore`
  - [ ] Commit
- [ ] Enable GitHub Pages:
  - [ ] Settings → Pages → Source: `main` → Save
  - [ ] Chờ 1-2 phút

### Cách B: Dùng Git Command (Pro - 5 bước)

```bash
# 1. Tạo local repo
mkdir content-outline-playbook
cd content-outline-playbook
git init

# 2. Copy file vào folder
# (index.html, README.md, LICENSE, .gitignore, docs/)

# 3. Commit
git add .
git commit -m "Initial commit"

# 4. Push (copy lệnh từ GitHub)
git remote add origin https://github.com/yourusername/content-outline-playbook.git
git branch -M main
git push -u origin main

# 5. Enable Pages (GitHub web)
# Settings → Pages → main → Save
```

- [ ] Repo tạo
- [ ] Local files committed
- [ ] Push lên GitHub
- [ ] GitHub Pages enabled

---

## ✅ Sau Upload (Kiểm Tra)

- [ ] Vào: `https://yourusername.github.io/content-outline-playbook`
- [ ] Ứng dụng load đầy đủ (không lỗi)
- [ ] Có thể tạo Pillar + Angle
- [ ] Có thể export/import dữ liệu
- [ ] LocalStorage hoạt động (F12 → Application → LocalStorage)

---

## 🎉 Xong!

**Ứng dụng của bạn đã live trên internet!**

- ✅ Không cần server local
- ✅ Share URL trên social
- ✅ Backup code tự động
- ✅ Có thể dev thêm feature

---

## 🆘 Nếu Gặp Lỗi

| Lỗi | Giải pháp |
|-----|----------|
| "404 Not Found" | Chờ 2-3 phút, clear cache (Ctrl+Shift+Del) |
| "GitHub Pages not enabled" | Settings → Pages → Chọn `main` branch |
| "Permission denied" | Dùng SSH key hoặc GitHub CLI |
| "LocalStorage not working" | Chạy dùng server (không `file://`) |
| "AI Generator error" | Setup API Key hoặc dùng Mẫu có sẵn |

**→ Xem chi tiết**: `GITHUB_UPLOAD_GUIDE.md`

---

## 📞 Need Help?

- 📚 Full Guide: `GITHUB_UPLOAD_GUIDE.md`
- 🔧 Setup Guide: `docs/SETUP.md`
- 🤖 API Guide: `docs/API_INTEGRATION.md`

---

**Good luck! 🚀**
