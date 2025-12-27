# Hướng dẫn Cấu trúc Thư mục Âm thanh (Sound Structure)

Để cập nhật âm thanh cho game, bạn hãy tổ chức thư mục `sounds` theo cấu trúc sau để khớp với code mới:

## 1. Cấu trúc Thư mục (Folder Structure)

Bạn cần tạo các folder bên trong thư mục `sounds` của dự án:

```text
sounds/
├── common/             <-- Dùng cho các âm thanh chung (General)
│   ├── click.mp3       (Tiếng click nút)
│   ├── success.mp3     (Thông báo thành công)
│   ├── error.mp3       (Thông báo lỗi)
│   ├── levelup.mp3     (Lên cấp)
│   ├── coin.mp3        (Nhận xu)
│   ├── open.mp3        (Mở modal)
│   └── close.mp3       (Đóng modal)
│   ├── next.mp3        (Chuyển tiếp)
│   └── prev.mp3        (Quay lại)
│
├── game_runner/        <-- Game Chạy (Runner)
│   ├── start.mp3       (Bắt đầu chạy)
│   ├── move.mp3        (Di chuyển trái/phải)
│   ├── speedup.mp3     (Tăng tốc)
│   └── gameover.mp3    (Thua cuộc)
│
├── game_archery/       <-- Game Bắn Cung (Archery)
│   ├── draw.mp3        (Kéo cung)
│   ├── release.mp3     (Bắn tên)
│   ├── hit.mp3         (Trúng đích)
│   ├── miss.mp3        (Trượt)
│   └── hint.mp3        (Dùng gợi ý)
│
├── game_memory/        <-- Game Lật Thẻ (Memory)
│   ├── flip.mp3        (Lật thẻ)
│   ├── match.mp3       (Ghép đúng)
│   ├── miss.mp3        (Ghép sai)
│   └── win.mp3         (Hoàn thành màn)
│
├── game_quiz/          <-- Game Trắc nghiệm (Quiz)
│   ├── correct.mp3     (Chọn đúng)
│   ├── wrong.mp3       (Chọn sai)
│   └── tick.mp3        (Tiếng đồng hồ đếm ngược)
│
└── music/              <-- Nhạc nền (Background Music)
    ├── general.mp3     (Nhạc sảnh chờ)
    ├── runner.mp3      (Nhạc game Runner)
    ├── archery.mp3     (Nhạc game Archery)
    └── memory.mp3      (Nhạc game Memory)
```

## 2. Cách cập nhật Code

Sau khi đã chép file vào đúng thư mục, bạn cần sửa đường dẫn trong file `toeicliam (11).html`.
Tìm đến phần `SoundManager` (khoảng dòng 1370) và sửa object `assets`:

```javascript
/* Tìm đoạn này trong SoundManager */
assets: {
    common: {
        // Sửa link CDN thành đường dẫn nội bộ (Local Path)
        click: './sounds/common/click.mp3',   // <-- Sửa như thế này
        success: './sounds/common/success.mp3',
        // ... (cập nhật hết các dòng còn lại)
    },
    game_runner: {
        start: './sounds/game_runner/start.mp3',
        // ...
    },
    // Làm tương tự với các mục khác...
}
```

**Lưu ý:**
- File âm thanh nên dùng định dạng `.mp3` để nhẹ và tương thích tốt nhất.
- Kiểm tra chính xác tên file và tên folder (viết thường, không dấu).
