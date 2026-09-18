<div align="center">

# 🔮 Discord Auto Orb

![Version](https://img.shields.io/badge/Version-v4.10.6-blue)
![Platform](https://img.shields.io/badge/Platform-Discord-5865F2?logo=discord&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

**Tự động hoàn thành Quest trên Discord - Nhận Orb, Avatar Decoration, In-game Rewards miễn phí!**

[📥 **Tải code (.zip)**](https://github.com/vVnK-wh0i4m/tool-discord-auto-orb/archive/refs/heads/main.zip) • [📦 **Clone repo**](https://github.com/vVnK-wh0i4m/tool-discord-auto-orb.git)

</div>

---

## ⚠️ Cảnh báo quan trọng

> **Công cụ này được cung cấp cho mục đích nghiên cứu và thử nghiệm.** Người dùng **chịu toàn bộ trách nhiệm** khi sử dụng.

> **Discord có thể phát hiện và xử lý tài khoản sử dụng tool tự động.** Hãy cân nhắc kỹ trước khi dùng.

---

## 📋 Mục lục

- [Giới thiệu](#-giới-thiệu)
- [Tính năng](#-tính-năng)
- [Yêu cầu hệ thống](#-yêu-cầu-hệ-thống)
- [Cài đặt Discord cho từng HĐH](#-cài-đặt-discord-cho-từng-hđh)
- [Hướng dẫn sử dụng](#-hướng-dẫn-sử-dụng)
- [Cấu hình](#-cấu-hình)
- [FAQ](#-câu-hỏi-thường-gặp)
- [Bản quyền](#-bản-quyền)

---

## 🌟 Giới thiệu

**Discord Auto Orb** là userscript JavaScript chạy trên Console của Discord, tự động hoàn thành các Quest để nhận phần thưởng miễn phí như Orb, Avatar Decoration, và In-game Rewards.

**Điểm nổi bật:**
- 🎯 Tự động hoàn thành Video Quest
- 🎮 Tự động hoàn thành Game/Stream Quest
- 🏆 Tự động hoàn thành Achievement Quest
- 📺 Tự động hoàn thành Activity Quest
- 🛡️ Anti-detection với random delay
- 🔔 Thông báo khi hoàn thành
- 🎨 Giao diện đẹp, dễ sử dụng

---

## 🚀 Tính năng

### 🎯 Auto Quest Completion

| Loại Quest | Mô tả |
|------------|--------|
| VIDEO | Tự động xem video, gửi progress từng giây |
| GAME | Giả lập process game, nhận heartbeat từ Discord |
| STREAM | Giả lập stream, tự động hoàn thành |
| ACHIEVEMENT | OAuth bypass qua Discord Says |
| ACTIVITY | Heartbeat loop giả lập tham gia activity |

### 🛡️ Anti-Detection

| Tính năng | Mô tả |
|-----------|--------|
| Random Delay | Nghỉ 1-30 phút ngẫu nhiên giữa các cycle |
| Rate Limit Handling | Tự retry khi bị Discord limit |
| Natural Cadence | Gửi progress theo nhịp tự nhiên |
| Cleanup | Dọn dẹp sạch sẽ khi dừng |

### 🎨 Giao diện

| Tính năng | Mô tả |
|-----------|--------|
| Dashboard | UI draggable, hiển thị tiến độ real-time |
| Quest Picker | Chọn quest muốn auto |
| Log System | Ghi lại mọi hoạt động |
| Sound Alert | Âm thanh khi hoàn thành |

---

## 💻 Yêu cầu hệ thống

| Thành phần | Yêu cầu |
|------------|----------|
| Trình duyệt | Chrome, Edge, Opera, Brave (Chromium-based) |
| Discord | Phiên bản Desktop hoặc Web |
| Mạng | Kết nối internet ổn định |

---

## 📥 Cài đặt Discord cho từng HĐH

### 🪟 Windows

**Tải Discord PTB cho Windows tại đây:** [Tải Discord PTB](https://ptb.discord.com/api/downloads/distributions/app/installers/latest?channel=ptb&platform=win&arch=x64)

**Hoặc tải Discord Canary:** [Tải Discord Canary](https://discord.com/api/download/canary?platform=win&arch=x64)

**Cài đặt:**
1. Chạy file `DiscordPTBSetup.exe` vừa tải
2. Làm theo hướng dẫn trên màn hình
3. Mở Discord PTB lên và đăng nhập tài khoản

---

### 🐧 Linux (Ubuntu/Debian)

**Tải Discord PTB cho Linux (Debian/Ubuntu) tại đây:** [Tải Discord PTB](https://discord.com/api/download/ptb?platform=linux&format=deb)

**Cài đặt:**
```bash
sudo dpkg -i discord-ptb-*.deb
sudo apt-get install -f
```

Mở Discord PTB lên và đăng nhập tài khoản.

---

### 🍎 macOS

**Tải Discord PTB cho macOS tại đây:** [Tải Discord PTB](https://discord.com/api/download/ptb?platform=osx)

**Cài đặt:**
1. Mở file `.dmg` vừa tải
2. Kéo icon Discord vào thư mục Applications
3. Mở Discord PTB lên và đăng nhập tài khoản

---

## 📖 Hướng dẫn sử dụng

> **LƯU Ý:** Hướng dẫn sử dụng này áp dụng cho TẤT CẢ các HĐH (Windows, Linux, macOS). Bạn chỉ cần mở tab Console và chạy tool theo các bước bên dưới.

### Bước 1: Mở tab Console

| HĐH | Phím tắt |
|------|----------|
| Windows | `Ctrl + Shift + I` → chọn tab **Console** |
| Linux | `Ctrl + Shift + I` hoặc `F12` → chọn tab **Console** |
| macOS | `Cmd + Option + I` → chọn tab **Console** |

### Bước 2: Bật Allow Pasting

Khi bạn mở Console lần đầu, Discord sẽ hiển thị cảnh báo:

**Ảnh 1 - Cảnh báo "Chờ Đã!" khi mở Console:**

![Console Warning](images/console-warning.png)

> ⚠️ **Đây là cảnh báo của Discord để bảo vệ bạn.** Đừng lo lắng!

**Ảnh 2 - Thông báo "allow pasting":**

![Allow Pasting Warning](images/allow-pasting-warning.png)

**Ảnh 3 - Gõ "allow pasting" vào Console:**

![Allow Pasting Typed](images/allow-pasting-typed.png)

**Làm theo các bước sau:**
1. Nhìn vào Console, bạn sẽ thấy dòng chữ cảnh báo màu vàng/orange
2. Gõ tay từ **`allow pasting`** vào ô Console (như ảnh 3)
3. Nhấn **Enter**
4. Bây giờ bạn có thể dán code vào Console rồi

> ⚠️ **QUAN TRỌNG:** PHẢI gõ chính xác `allow pasting` rồi nhấn Enter. Nếu KHÔNG gõ thì sẽ KHÔNG dán được code vào Console!

### Bước 3: Dán code và chạy

1. **Tải file** `discord-auto-orb.js` từ repo này
2. **Mở file** bằng text editor (VS Code, Notepad++,...)
3. **Copy TOÀN BỘ** nội dung file
4. **Dán** vào Console Discord
5. **Nhấn Enter** để chạy

### Bước 4: Chọn Quest

Tool sẽ hiện dashboard với danh sách quest có sẵn:

1. **Đọc kỹ** từng quest trước khi chọn
2. **Tick chọn** quest muốn auto
3. **Bật/tắt** các tùy chọn:
   - Auto-enroll: Tự động đăng ký quest
   - Auto-claim: Tự động nhận thưởng
   - Sound: Âm thanh thông báo
   - Random delay: Nghỉ ngẫu nhiên giữa các cycle
4. **Nhấn START** để bắt đầu

### Bước 5: Theo dõi tiến độ

Dashboard hiển thị real-time:
- 🟢 **Đang chạy** - Quest đang được hoàn thành
- ✅ **Hoàn thành** - Quest đã xong, nhấn CLAIM
- ❌ **Thất bại** - Quest bị lỗi, cần kiểm tra

---

## ⚙️ Cấu hình

### File `discord-auto-orb.js`

Mở file và tìm phần `CONFIG` ở đầu file:

```javascript
const CONFIG = {
    NAME: "vVnK-wh0i4m",           // Tên hiển thị
    VERSION: "v4.10.6",            // Phiên bản
    THEME: "#5865F2",              // Màu chủ đạo (Discord blurple)
    SUCCESS: "#3BA55C",            // Màu thành công
    WARN: "#faa61a",               // Màu cảnh báo
    ERR: "#f04747",                // Màu lỗi
    HIDE_ACTIVITY: false,          // Ẩn "Playing ..." khi chạy quest
    MAX_LOG_ITEMS: 60              // Số dòng log tối đa
};
```

### Các tùy chọn Runtime

| Tùy chọn | Mặc định | Mô tả |
|----------|----------|-------|
| `autoEnroll` | `true` | Tự động đăng ký quest mới |
| `autoClaim` | `false` | Tự động nhận thưởng |
| `playSound` | `false` | Phát âm thanh khi hoàn thành |
| `randomDelay` | `false` | Nghỉ 1-30 phút ngẫu nhiên |

---

## ❓ Câu hỏi thường gặp

### Tool không hoạt động?

1. **Kiểm tra Console** - Có lỗi đỏ không?
2. **Discord version** - Dùng PTB hoặc Canary, KHÔNG dùng Stable
3. **CSP Error** - Nếu gặp lỗi CSP, dùng Vencord plugin
4. **Reload** - Thử reload Discord và chạy lại

### Lỗi "Already running"?

- Có instance khác đang chạy
- Reload trang Discord rồi chạy lại

### Quest không hoàn thành?

- Kiểm tra Discord có hiển thị "Playing ..." không
- Thử bật `HIDE_ACTIVITY: false`
- Kiểm tra kết nối mạng

### Bị rate limit (429)?

- Tool tự retry với exponential backoff
- Nếu liên tục bị, tăng random delay
- Nghỉ vài phút rồi chạy lại

### Auto-claim không hoạt động?

- Có thể cần captcha
- Nhấn nút CLAIM thủ công trên dashboard
- Kiểm tra Discord Quests page

---

## 📜 Bản quyền

**MIT License** - Xem file [LICENSE](LICENSE) để biết chi tiết.

| ✅ Được phép | ❌ Không được phép |
|-------------|-------------------|
| Nghiên cứu | Vi phạm ToS Discord |
| Thử nghiệm | Gây hại tài khoản khác |
| Học tập | Thương mại hóa |

---

<div align="center">

**⭐ Star repo nếu thấy hữu ích! ⭐**

Made with ❤️ by vVnK

</div>
