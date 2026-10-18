# TSD Creator Studio — React Web App MVP 2.1

Ứng dụng React + Vite, triển khai Netlify qua GitHub. Không còn là bản HTML demo độc lập.

## Chạy trên máy
```bash
npm install
npm run dev
npm run build
```

## Netlify
Đã có `netlify.toml`: build `npm run build`, publish `dist`, SPA redirects. Mỗi lần push lên nhánh triển khai sẽ tự build theo cấu hình CI/CD của Netlify.

## Tính năng
- Quản lý nhiều dự án, chọn dự án, tạo/xóa, tự động lưu localStorage, sao lưu/khôi phục JSON.
- Script Studio 4 bước có kiểm soát điều kiện chuyển bước.
- Dàn ý theo quy tắc; dựng các chương từ dàn ý; biên tập nội dung trực tiếp.
- Chọn thể loại, phong cách, ngôi kể; ước tính số từ và thời lượng; xuất TXT.
- AI tùy chọn: người dùng nhập Gemini API key **trong phiên**, chọn viết từng chương. Key không lưu vào localStorage, không đi qua server của chủ website.

## Giới hạn quan trọng
- Dàn ý và nội dung ban đầu chỉ là bản thảo theo quy tắc, không phải AI sáng tác hoàn chỉnh.
- Chức năng Gemini cần API key cá nhân hợp lệ, truy cập mạng, model có sẵn và hạn mức; không bảo đảm miễn phí hoặc hoạt động với mọi tài khoản.
- Nội dung và key được gửi trực tiếp từ trình duyệt tới Gemini khi bấm tạo; không nên sử dụng khóa bí mật nhạy cảm trong trình duyệt chia sẻ.
- Không có cloud sync, tài khoản Google/Apple, xuất MP3 hoặc đăng YouTube.
- Dữ liệu lưu trong localStorage, xóa cache có thể mất; nên sao lưu JSON định kỳ.
- Cần UAT thực tế trên iPad, desktop và kiểm tra các lỗi trình duyệt trước khi coi là production-ready.
