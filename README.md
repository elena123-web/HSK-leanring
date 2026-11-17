# 汉语小屋 — AI hội thoại theo từ vựng

Trang `ai-dialogue.html` tạo hội thoại mới bằng AI dựa trên từ bạn đã lưu trong `index.html`. Có thể chọn chủ đề, HSK, chiều luyện Trung–Việt/Anh và luyện dịch từng câu.

## Dùng thử

1. Mở `index.html` và thêm từ vựng. AI có thể dùng danh sách ở cùng trình duyệt/domain.
2. Mở `ai-dialogue.html` trên cùng domain và trình duyệt. Khi dùng GitHub Pages, đường dẫn là `https://<tên-tài-khoản>.github.io/<tên-repo>/ai-dialogue.html`.
3. Nhập OpenAI API key và model tương thích, chọn chủ đề/HSK/chiều dịch rồi nhấn **Sáng tác hội thoại**.
4. Nhấn loa để nghe tiếng Trung; phần luyện phía dưới cho phép dịch từng lượt và xem đáp án.

## Bảo mật và giới hạn

- API key chỉ nằm trong bộ nhớ của tab hiện tại, không ghi vào localStorage và sẽ mất khi tải lại trang. Tuy nhiên, khi gọi API trực tiếp từ trình duyệt, key vẫn được sử dụng ở client. Chỉ dùng key cá nhân có giới hạn ngân sách/quyền; không nhúng key cố định vào mã nguồn hoặc chia sẻ trang có key.
- Để triển khai công khai, chuyển lời gọi AI sang backend/serverless proxy có xác thực, giới hạn tốc độ và quản lý secret ở biến môi trường.
- Sổ từ dùng `localStorage`, vì vậy dữ liệu phải mở trên cùng trình duyệt và origin. Nếu trang học chưa có từ đã lưu, hãy thêm từ trước rồi bấm **Làm mới danh sách từ**.
