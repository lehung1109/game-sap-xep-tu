# Game Sắp Xếp Từ

Một trò chơi giáo dục giúp trẻ em học tiếng Anh bằng cách sắp xếp các từ thành câu hoàn chỉnh.

## Cách sử dụng

1. Mở file `index.html` trong trình duyệt web
2. Game sẽ tự động load các cấp độ từ file `levels.json`
3. Sắp xếp các từ từ ngân hàng từ vào hàng trả lời để tạo thành câu đúng
4. Sử dụng các nút:
   - **Làm mới**: Reset cấp độ hiện tại
   - **Phát âm (EN)**: Nghe phát âm câu tiếng Anh
   - **Gợi ý**: Nhận gợi ý (tối đa 2 lần)
   - **Kiểm tra**: Kiểm tra câu trả lời
   - **Câu tiếp theo**: Chuyển sang cấp độ tiếp theo

## Cấu trúc file JSON

File `levels.json` chứa danh sách các cấp độ với cấu trúc:

```json
[
  {
    "id": "unique_id",
    "vn": "Câu tiếng Việt với emoji",
    "en": "Câu tiếng Anh tương ứng",
    "tokens": ["Các", "từ", "riêng", "biệt"]
  }
]
```

### Các trường:

- **id**: Định danh duy nhất cho cấp độ
- **vn**: Câu tiếng Việt hiển thị cho người chơi
- **en**: Câu tiếng Anh để phát âm
- **tokens**: Mảng các từ tiếng Anh để sắp xếp

## Tính năng

- Hỗ trợ kéo thả (drag & drop) để sắp xếp từ
- Phát âm tiếng Anh tự động
- Gợi ý thông minh
- Hiệu ứng âm thanh và hình ảnh
- Giao diện responsive
- Hỗ trợ chế độ tối (dark mode)

## Thêm cấp độ mới

Để thêm cấp độ mới, chỉ cần thêm object vào mảng trong file `levels.json`:

```json
{
  "id": "new_level",
  "vn": "Con thích học tiếng Anh 📚",
  "en": "I like learning English.",
  "tokens": ["I", "like", "learning", "English"]
}
```

Game sẽ tự động nhận diện và hiển thị cấp độ mới.
