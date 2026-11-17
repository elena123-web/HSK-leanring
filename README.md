# 汉语小屋 — Học tiếng Trung cùng AI

Ứng dụng học tiếng Trung nằm trên một trang duy nhất: `index.html`.

## Tính năng

- Thêm, tìm kiếm và xóa từ vựng; gắn nghĩa tiếng Việt/Anh và cấp HSK 1–6.
- Chọn chủ đề, cấp độ, số lượt và chiều dịch: Trung–Việt, Trung–Anh, Việt–Trung hoặc Anh–Trung.
- AI sáng tác hội thoại mới từ từ vựng đã lưu; hiển thị pinyin, bản dịch và phát âm.
- Luyện dịch từng lượt; AI đánh giá nội dung và đưa phản hồi, chấp nhận bản dịch tương đương.
- Dữ liệu từ vựng và tiến độ được lưu trong localStorage của trình duyệt.

## Chạy ứng dụng

Mở `index.html` trong trình duyệt hoặc chạy qua localhost/host tĩnh. Tính năng AI yêu cầu Internet và API key tương thích OpenAI; nhập key trong trang. Key chỉ giữ trong bộ nhớ của tab, nhưng gọi trực tiếp từ trình duyệt vẫn sử dụng key phía client. Với trang công khai hoặc dùng chung, hãy chuyển API call sang backend/serverless và giữ secret trong biến môi trường; không đưa key vào mã nguồn.

Từ vựng nằm trong localStorage nên chỉ khả dụng trên cùng trình duyệt và origin.
