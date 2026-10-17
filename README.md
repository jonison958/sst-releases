# sst-releases

Kho lưu trữ này dùng để quản lý các bản phát hành (release) liên quan đến dự án "sst".

> Lưu ý: Đây là README mẫu. Bạn có thể chỉnh sửa nội dung phía dưới để phù hợp với mục đích thực tế của repo.

## Mục lục

- [Mục đích](#mục-đích)
- [Nội dung](#nội-dung)
- [Cách sử dụng](#cách-sử-dụng)
- [Cách đóng góp](#cách-đóng-góp)
- [Quy trình phát hành](#quy-trình-phát-hành)
- [Liên hệ](#liên-hệ)

## Mục đích

Tóm tắt ngắn gọn mục đích của repo: lưu trữ các gói/phát hành, note release, hoặc file assets liên quan đến các phiên bản của dự án "sst".

## Nội dung

Mặc định repository có thể chứa:
- Thư mục `releases/` hoặc `assets/` chứa file phát hành
- File markdown mô tả release notes cho từng phiên bản
- Script hoặc pipeline để tạo release tự động (nếu có)

## Cách sử dụng

1. Nếu bạn là maintainer, thêm file phát hành vào thư mục phù hợp (ví dụ `releases/v1.0.0/`) kèm theo `CHANGELOG.md` hoặc `notes.md`.
2. Nếu repo dùng GitHub Releases, tạo release qua giao diện GitHub hoặc sử dụng GitHub CLI:

   gh release create v1.0.0 ./releases/v1.0.0/* --title "v1.0.0" --notes-file ./releases/v1.0.0/notes.md

3. Đối với người dùng: kiểm tra thư mục `releases/` hoặc tab Releases để tải các artifacts.

## Cách đóng góp

1. Fork repository
2. Tạo branch mới `feature/your-change`
3. Gửi pull request mô tả thay đổi

Hoặc mở issue nếu bạn muốn đề xuất thay đổi lớn.

## Quy trình phát hành (mẫu)

- Bump version trong file cấu hình (nếu có)
- Cập nhật `CHANGELOG.md` hoặc `notes.md`
- Tạo tag git: `git tag -a vX.Y.Z -m "Release vX.Y.Z"`
- Push tag và tạo Release trên GitHub

## Liên hệ

Nếu cần hỗ trợ, mở issue hoặc liên hệ @jonison958.

---

Nếu bạn muốn, tôi có thể:
- Tùy chỉnh README bằng thông tin cụ thể hơn (mục đích chính xác của repo, ví dụ các lệnh, CI/CD, hoặc mẫu release note). 
- Thêm template cho `CHANGELOG.md` hoặc script tạo release tự động.

Cho tôi biết bạn muốn thêm gì — tôi sẽ cập nhật ngay.