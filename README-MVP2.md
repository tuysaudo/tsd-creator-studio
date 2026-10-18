# TSD Creator Studio — MVP 2.0

Web app tĩnh, không yêu cầu build, server hoặc API key.

## Chạy thử
Mở `index.html` bằng trình duyệt hoặc deploy repo lên Cloudflare Pages / Netlify (publish directory: repository root, không có build command).

## Tính năng hiện có
- Script Studio: 4 bước Ý tưởng → Dàn ý → Viết truyện → Hoàn thiện.
- Form responsive cho desktop, tablet, mobile.
- Chọn thể loại, nhập tiêu đề, ý tưởng, thời lượng và phong cách.
- Sao chép prompt dàn ý và từng chương để sử dụng trên ChatGPT/Gemini.
- Quản lý nhiều chương, sửa nội dung, tự động lưu localStorage.
- Đếm từ, ước tính thời lượng audio, xuất TXT, sao lưu JSON.

## Giới hạn MVP
- **Không có API AI tích hợp**: người dùng sao chép prompt và dán kết quả thủ công.
- **Không có đăng nhập, đồng bộ đám mây, xuất MP3 hoặc tự đăng YouTube**.
- Dữ liệu chỉ lưu trong trình duyệt trên thiết bị đang dùng. Xóa dữ liệu trình duyệt có thể mất bản nháp; nên sao lưu JSON.
- Công thức 130 từ/phút chỉ là ước tính, không phải thời lượng chính xác.
- Các module khác trên sidebar là định hướng, chưa triển khai.

## Chi phí
Chạy dạng static site không phát sinh phí API AI cho chủ website. Hosting free tier phụ thuộc hạn mức của nhà cung cấp.

## Quy trình cập nhật
Nhánh tính năng `feat/creator-studio-mvp2`; đề nghị review trước khi merge vào `main`.
