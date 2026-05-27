# 📤 Hướng Dẫn Upload Lên GitHub

## 🎯 Mục Đích

Đẩy ứng dụng Content Outline Playbook lên GitHub để:
- ✅ Chạy trên GitHub Pages (không cần server)
- ✅ Backup code & version control
- ✅ Dễ share & collaborate
- ✅ Public hoặc private tuỳ ý

---

## 📋 Yêu Cầu Trước

- ✅ Tài khoản GitHub (free)
- ✅ Git cài đặt trên máy
- ✅ Terminal/Command Prompt
- ✅ File `index.html` + `README.md`

---

## 🚀 Phương Pháp 1: Upload Qua GitHub Web (Dễ Nhất)

### Bước 1: Tạo Repository Mới

1. Truy cập: https://github.com/new
2. Đặt tên: `content-outline-playbook`
3. **Description**: "AI-powered Content Strategy Tool"
4. **Public** (hoặc Private)
5. ✅ **Add README.md** (optional, vì bạn có rồi)
6. Nhấn **"Create repository"**

### Bước 2: Upload File

1. Vào repo vừa tạo
2. Nhấn **"Add file"** → **"Upload files"**
3. Drag & drop hoặc chọn:
   - `index.html`
   - `README.md`
   - `LICENSE`
   - `.gitignore`
4. Nhấn **"Commit changes"**

### Bước 3: Enable GitHub Pages

1. Vào **Settings** (tab)
2. Tìm **"Pages"** (bên trái)
3. **Source**: Chọn `main` branch
4. Nhấn **"Save"**
5. Chờ 1-2 phút

### ✅ Hoàn Tất!

App sẽ chạy tại: `https://yourusername.github.io/content-outline-playbook`

---

## 🛠️ Phương Pháp 2: Upload Qua Git Command (Recommended)

### Bước 1: Cài Đặt Git

**Windows**: https://git-scm.com/download/win  
**Mac**: `brew install git`  
**Linux**: `sudo apt install git`

### Bước 2: Config Git (Lần Đầu)

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Bước 3: Tạo Repository Local

```bash
# Tạo folder mới
mkdir content-outline-playbook
cd content-outline-playbook

# Init git repository
git init

# Tạo branch chính
git branch -M main
```

### Bước 4: Copy File Vào Folder

Copy những file này vào folder:
```
content-outline-playbook/
├── index.html
├── README.md
├── LICENSE
├── .gitignore
└── docs/
    ├── SETUP.md
    ├── API_INTEGRATION.md
    └── (các file khác)
```

### Bước 5: Commit Files

```bash
# Add tất cả files
git add .

# Commit
git commit -m "Initial commit: Content Outline Playbook"
```

### Bước 6: Tạo Repository Trên GitHub

1. Truy cập: https://github.com/new
2. Đặt tên: `content-outline-playbook`
3. **Không** chọn "Initialize with README" (bạn có rồi)
4. Nhấn **"Create repository"**

### Bước 7: Push Lên GitHub

Sao chép lệnh từ GitHub (nó sẽ như thế này):

```bash
# Thêm remote
git remote add origin https://github.com/yourusername/content-outline-playbook.git

# Push
git branch -M main
git push -u origin main
```

**Lưu ý**: Thay `yourusername` bằng username GitHub của bạn

### Bước 8: Enable GitHub Pages

1. Vào repo trên GitHub
2. **Settings** → **Pages**
3. **Source**: `main` branch
4. Nhấn **"Save"**

### ✅ Hoàn Tất!

Mở: `https://yourusername.github.io/content-outline-playbook`

---

## 📱 Chỉnh Sửa & Update

### Update Local Changes

```bash
# Chỉnh sửa file (VD: index.html)
# ...

# Commit
git add .
git commit -m "Fix: Thêm tính năng X"

# Push lên GitHub
git push origin main
```

### Pull Changes Từ GitHub

```bash
git pull origin main
```

---

## 📂 Cấu Trúc Repository Hoàn Chỉnh

```
content-outline-playbook/
├── index.html              # File HTML chính (3000+ dòng)
├── README.md               # Tài liệu tổng quan
├── LICENSE                 # MIT License
├── .gitignore              # Các file ignore
├── docs/
│   ├── SETUP.md            # Hướng dẫn setup
│   ├── API_INTEGRATION.md  # API guide
│   ├── FEATURES.md         # Danh sách tính năng
│   └── TROUBLESHOOTING.md  # Xử lý sự cố
└── assets/ (optional)
    ├── screenshots/        # Ảnh demo
    └── templates/          # Template backup
```

---

## 🔧 Hữu Ích: Git Commands

```bash
# Kiểm tra status
git status

# Xem commit history
git log

# Revert commit cuối cùng
git revert HEAD

# Create branch mới (để dev feature)
git checkout -b feature/new-feature

# Merge branch
git merge feature/new-feature

# Delete branch
git branch -d feature/new-feature

# Xem remote
git remote -v
```

---

## 🆘 Troubleshooting

### "Permission denied" khi push

**Giải pháp**:
```bash
# 1. Tạo SSH key (nếu chưa)
ssh-keygen -t ed25519 -C "your.email@example.com"

# 2. Add SSH key vào GitHub
# Settings → SSH and GPG keys → New SSH key

# 3. Thay URL
git remote set-url origin git@github.com:yourusername/content-outline-playbook.git

# 4. Push
git push origin main
```

Hoặc dùng **GitHub CLI**:
```bash
gh repo create content-outline-playbook --source=. --remote=origin --push
```

### GitHub Pages không update

**Giải pháp**:
1. Kiểm tra branch đúng là `main`
2. Clear cache: Ctrl+Shift+Del
3. Xoá và tạo lại branch (advanced)
4. Chờ 2-5 phút rebuild

### File HTML không render

**Giải pháp**:
1. Kiểm tra file tên chính xác `index.html`
2. Kiểm tra nằm ở root folder
3. Kiểm tra GitHub Pages setting

---

## 🌐 Custom Domain (Optional)

Nếu muốn chạy trên domain riêng (VD: `contentplanner.com`):

1. **Mua domain** (GoDaddy, Namecheap, etc.)
2. **Vào GitHub repo** → **Settings** → **Pages**
3. **Custom domain**: Nhập domain
4. **Update DNS** tại domain provider:
   - Type: `A` hoặc `CNAME`
   - Points to: IP GitHub Pages
5. Chờ propagate (5-48 giờ)

---

## 📊 Public vs Private Repository

### Public (Recommended)
- ✅ Anyone có thể thấy code
- ✅ Good for portfolio
- ✅ Easier to share
- ✅ GitHub Pages free

### Private
- ✅ Chỉ bạn có thể thấy
- ✅ Good for personal use
- ⚠️ GitHub Pages cần Pro plan

---

## 🔐 Bảo Mật

### ⚠️ KHÔNG commit những file này

```
.env                    # Environment variables
config.secret.js        # API Keys
credentials.json        # Private keys
node_modules/          # Dependencies
*.log                  # Log files
.DS_Store              # OS files
```

Đây là lý do có `.gitignore`!

### ✅ Làm Đúng

- Lưu API Keys trong **LocalStorage** (browser), không file
- Dùng **.gitignore** để exclude private files
- Nếu accident commit secret, regenerate ngay

---

## 🎉 Hoàn Tất!

### Checklist Final

- [ ] Repository tạo trên GitHub
- [ ] Tất cả file đã push lên
- [ ] GitHub Pages enabled
- [ ] App chạy ở URL GitHub Pages
- [ ] Có thể access mà không cần local server
- [ ] Share URL với người khác

### URLs Bạn Sẽ Có

```
GitHub Repo:     https://github.com/yourusername/content-outline-playbook
GitHub Pages:    https://yourusername.github.io/content-outline-playbook
(Edit):          https://github.com/yourusername/content-outline-playbook/edit/main/index.html
```

---

## 📞 Liên Hệ Help

- 📚 GitHub Docs: https://docs.github.com
- 🐛 GitHub Issues: Report bugs tại repo
- 💬 GitHub Discussions: Q&A
- 🆘 Email support: support@example.com

---

**Now your app is live on the internet! 🌍✨**
