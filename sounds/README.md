# 🔊 TOEIC LIAM - Sound Assets

## 📁 Cấu Trúc Thư Mục

```
sounds/
├── general/              # Âm thanh chung
│   ├── click.mp3         # Click button
│   ├── success.mp3       # Thành công
│   ├── error.mp3         # Lỗi
│   ├── levelup.mp3       # Lên level
│   ├── coin.mp3          # Nhận xu
│   ├── open.mp3          # Mở menu/modal
│   └── close.mp3         # Đóng menu/modal
│
├── quiz/                 # Trắc nghiệm
│   ├── correct.mp3       # ✅ Trả lời đúng
│   ├── wrong.mp3         # ❌ Trả lời sai
│   ├── tick.mp3          # ⏱️ Đếm giờ
│   └── complete.mp3      # 🎉 Hoàn thành
│
├── flashcard/            # Thẻ từ vựng
│   ├── flip.mp3          # 🔄 Lật thẻ
│   ├── next.mp3          # ➡️ Thẻ tiếp
│   ├── prev.mp3          # ⬅️ Thẻ trước
│   └── complete.mp3      # 🎉 Hoàn thành bộ thẻ
│
├── memory/               # Game ghép thẻ
│   ├── flip.mp3          # 🔄 Lật thẻ
│   ├── match.mp3         # ✅ Ghép đúng
│   ├── miss.mp3          # ❌ Ghép sai
│   └── win.mp3           # 🏆 Thắng game
│
├── runner/               # Game Bắn Vịt
│   ├── start.mp3         # ▶️ Bắt đầu
│   ├── move.mp3          # 🏃 Di chuyển
│   ├── jump.mp3          # ⬆️ Nhảy
│   ├── speedup.mp3       # ⚡ Tăng tốc
│   ├── gameover.mp3      # 💀 Game over
│   └── shoot.mp3         # 🔫 Bắn
│
├── archery/              # Game Space Defender
│   ├── draw.mp3          # 🏹 Kéo cung
│   ├── release.mp3       # 🚀 Bắn
│   ├── hit.mp3           # 🎯 Trúng đích
│   ├── miss.mp3          # ❌ Trượt
│   ├── hint.mp3          # 💡 Gợi ý
│   └── bullseye.mp3      # 🎯 Trúng tim
│
├── notification/         # 🔔 Thông báo (MỚI!)
│   ├── system.mp3        # 📢 Thông báo hệ thống
│   ├── reminder.mp3      # ⏰ Nhắc nhở học
│   ├── assignment.mp3    # 📚 Giao bài tập
│   ├── achievement.mp3   # 🏆 Thành tích
│   ├── warning.mp3       # ⚠️ Cảnh báo
│   ├── invite.mp3        # 🎮 Lời mời PvP
│   └── message.mp3       # 💬 Tin nhắn
│
└── music/                # 🎵 Nhạc nền
    ├── general.mp3       # Nhạc chung
    ├── archery.mp3       # Nhạc Space Defender
    ├── memory.mp3        # Nhạc Memory
    └── runner.mp3        # Nhạc Duck Hunt
```

---

## 🚀 Cách Cài Đặt

### Cách 1: Chạy Script (Nhanh)
```bash
cd sounds/
chmod +x download_sounds.sh
./download_sounds.sh
```

### Cách 2: Thủ Công
1. Tải file MP3 từ [Freesound.org](https://freesound.org)
2. Đặt vào đúng thư mục với đúng tên file

---

## 🔧 Cách Sử Dụng Trong Code

```javascript
// Âm thanh game
playSound('quiz', 'correct');      // Quiz - đúng
playSound('memory', 'match');      // Memory - ghép đúng
playSound('runner', 'shoot');      // Runner - bắn

// Âm thanh thông báo
playSound('notification', 'system');      // Thông báo hệ thống
playSound('notification', 'reminder');    // Nhắc nhở học
playSound('notification', 'assignment');  // Giao bài tập
playSound('notification', 'achievement'); // Thành tích
playSound('notification', 'warning');     // Cảnh báo
playSound('notification', 'invite');      // Lời mời PvP

// Nhạc nền
playMusic('runner');   // Bật nhạc Runner
playMusic('archery');  // Bật nhạc Space
stopMusic();           // Tắt nhạc
```

---

## 🎨 Cách Thay Đổi Âm Thanh

1. **Chuẩn bị file**: Format MP3, 128-192kbps
2. **Đổi tên file**: Giữ nguyên tên (vd: `correct.mp3`)
3. **Đặt vào thư mục**: Thay thế file cũ
4. **Refresh app**: Âm thanh mới sẽ được dùng

---

## 📊 Bảng Tham Chiếu Nhanh

| Game/Feature | Folder | Files |
|--------------|--------|-------|
| Chung | `general/` | click, success, error, levelup, coin, open, close |
| Quiz | `quiz/` | correct, wrong, tick, complete |
| Flashcard | `flashcard/` | flip, next, prev, complete |
| Memory | `memory/` | flip, match, miss, win |
| Runner | `runner/` | start, move, jump, speedup, gameover, shoot |
| Archery | `archery/` | draw, release, hit, miss, hint, bullseye |
| **Notification** | `notification/` | system, reminder, assignment, achievement, warning, invite, message |
| Music | `music/` | general, archery, memory, runner |

---

## 🔗 Nguồn Âm Thanh Miễn Phí

- [Freesound.org](https://freesound.org) - CC license
- [Mixkit](https://mixkit.co/free-sound-effects/)
- [Pixabay](https://pixabay.com/sound-effects/)
- [Zapsplat](https://www.zapsplat.com)
- [OpenGameArt](https://opengameart.org)

---

*Cập nhật: December 2024*
