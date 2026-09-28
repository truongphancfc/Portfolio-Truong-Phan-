# Portfolio — Trường Phan

Mã nguồn của [truongphan-portfolio-interface.vercel.app](https://truongphan-portfolio-interface.vercel.app/). Đây là website tĩnh; không cần cài package hay chạy lệnh build.

## Sửa nội dung

- `index.html`: nội dung trang, gồm các mục `#growth-shopee`, `#growth-ads`, `#growth-ops` và portfolio thiết kế. Khi sửa chữ, cập nhật cả bản `data-vi` và `data-en`.
- `growth-preview.css`: giao diện dashboard Shopee, Meta và phần vận hành; có quy tắc cho điện thoại ở cuối file.
- `assets/`: ảnh, video và hai file CV công khai. Giữ nguyên tên file khi thay thế, hoặc sửa đường dẫn tương ứng trong `index.html`.
- `support.js` và `_ds/`: phần hiệu ứng và giao diện của portfolio gốc.

## Xem thử trên máy

Trong thư mục repository, chạy:

```bash
python3 -m http.server 8765
```

Mở `http://localhost:8765` để xem trang và kiểm tra cả bản tiếng Việt, tiếng Anh, điện thoại trước khi đưa lên GitHub.

## Cập nhật website

Repository đã kết nối với project Vercel. Mỗi commit trên nhánh `main` sẽ tự deploy production. Có thể sửa file trực tiếp trên GitHub hoặc làm việc trên máy:

```bash
git add .
git commit -m "Update portfolio"
git push origin main
```

Project Vercel: [truongphan-portfolio-interface](https://vercel.com/truongphancfcs-projects/truongphan-portfolio-interface).

## Dữ liệu hiệu suất

Dashboard công khai chỉ dùng các khoảng số liệu và chỉ số đã chuẩn hoá từ báo cáo thật. Không đưa CSV xuất từ Meta/Shopee, tên chiến dịch, shop, sản phẩm, ID tài khoản, ngân sách hay doanh thu gốc vào repository. `ROAS` trên trang là doanh thu được nền tảng ghi nhận chia cho chi phí quảng cáo, không phải lợi nhuận.
