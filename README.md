# POV-UMBRELLA API data

Repo này chỉ phục vụ dữ liệu API online cho bản POV và Umbrella đã chỉnh sửa. Kodi tải tệp `debrid_keys.json` từ nhánh `main`; không có mã nguồn plugin trong repo này.

## Cách dùng

1. Tạm chuyển repo sang **Public**.
2. Mở POV hoặc Umbrella → My Services/Accounts → **Nhập mã nhận API online (POV + Umbrella)**.
3. Nhập mã nhận. Một bản ghi có thể chứa cả Real-Debrid và TorBox; plugin kiểm tra từng dịch vụ rồi ghi key cho cả hai plugin.
4. Chuyển repo về **Private** sau khi dùng xong. Khi repo Private, Kodi không tải được dữ liệu mới cho tới khi mở Public lại.

API key không được ghi dạng chữ thường. Tệp dữ liệu dùng bản ghi mã hóa PBKDF2-HMAC-SHA256; chỉ người có mã nhận mới giải mã được nội dung.

## Thêm hoặc đổi dữ liệu

Chạy công cụ `create_debrid_record.py` ở thư mục làm việc trên máy, nhập mã nhận và key trong cửa sổ hỏi riêng. Công cụ chỉ ghi bản mã hóa vào `debrid_keys.json`; sau đó commit/push riêng tệp này lên nhánh `main`. Không dán key vào chat, lệnh PowerShell hoặc README.

Tệp mẫu hiện đang để `records` rỗng vì chưa có API key thật được cung cấp.
