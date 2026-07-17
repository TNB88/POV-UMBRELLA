# POV-UMBRELLA API data

Repo này chỉ phục vụ dữ liệu API online cho bản POV và Umbrella đã chỉnh sửa. Kodi tải tệp `debrid_keys.json` từ nhánh `main`; không có mã nguồn plugin trong repo này.

## Cách dùng

1. Tạm chuyển repo sang **Public**.
2. Sửa `debrid_keys.json`: thay hai dòng `DAN_API_KEY_...` bằng key thật rồi commit lên nhánh `main`.
3. Mở POV hoặc Umbrella → My Services/Accounts → **Nhập mã nhận API online (POV + Umbrella)**.
4. Nhập tên, ví dụ `teo`. Plugin kiểm tra Real-Debrid/TorBox rồi ghi key cho cả hai plugin.
5. Chuyển repo về **Private** sau khi dùng xong. Khi repo Private, Kodi không tải được dữ liệu mới cho tới khi mở Public lại.

API key được lưu trực tiếp theo yêu cầu. Bất kỳ ai cũng có thể đọc key khi repo đang Public; việc chuyển repo về Private không xóa key khỏi lịch sử Git.

## Thêm người khác

Sao chép khối `teo`, đổi thành tên mới và điền hai API key tương ứng. Tên nhập trong Kodi không phân biệt chữ hoa/chữ thường.
