PHẦN 1: PHÂN TÍCH HẬU QUẢ VÀ VI PHẠM BẢO MẬT
Hành động của An được xem là vi phạm nghiêm trọng "Quy tắc Cờ Đỏ Bảo mật" (Red Flag Security Rules) vì các lý do sau:
Sử dụng chế độ chia sẻ công khai không kiểm soát ("Anyone with the link"):
Khi để chế độ này, bất kỳ ai có đường dẫn đều có thể truy cập tài liệu mà không cần xác thực danh tính. Điều này biến một tài liệu nội bộ, nhạy cảm (danh sách thông tin khách hàng) thành một tài liệu trôi nổi trên không gian mạng nếu link vô tình bị rò rỉ hoặc bị phát tán.
Lạm dụng quyền chỉnh sửa cao nhất (Editor) cho đối tượng bên ngoài:
An cấp quyền Editor cho một cộng tác viên bên ngoài tổ chức. Quyền này cho phép người đó không chỉ chỉnh sửa nội dung mà còn có thể xóa toàn bộ dữ liệu, làm thay đổi cấu trúc file hoặc vô tình tiếp tay cho kẻ xấu phá hoại khi tài khoản/thiết bị của cộng tác viên đó gặp rủi ro bảo mật.
Thiếu lớp kiểm soát truy cập định danh (Identity-based Access Control):
Thay vì chia sẻ trực tiếp tới email cá nhân/tổ chức cụ thể của cộng tác viên, An lại dùng đường link mở, dẫn đến việc mất quyền kiểm soát hoàn toàn đối với những ai đang đọc hoặc thao tác trên dữ liệu.
PHẦN 2: THIẾT LẠP LẠI CẤU TRÚC PHÂN QUYỀN CHUẨN (SỬA LỖI)
Để đảm bảo an toàn tuyệt đối cho dữ liệu doanh nghiệp, An cần thiết lập lại hệ thống phân quyền theo chuẩn bảo mật sau:
Mức quyền phù hợp cho cộng tác viên:
Chỉ định quyền Commenter (Người bình luận) hoặc Viewer (Người xem) nếu họ chỉ cần đọc và góp ý.
Nếu bắt buộc phải để họ chỉnh sửa một phần nội dung, chỉ cấp quyền Editor giới hạn theo từng phần cụ thể và theo dõi lịch sử chỉnh sửa chặt chẽ, tuyệt đối không cấp quyền toàn cục trên các tài liệu cốt lõi.
Chế độ chia sẻ an toàn 100%:
Chia sẻ giới hạn theo email cá nhân/tổ chức (Restricted / Specific people): Chỉ cho phép chính xác địa chỉ email của cộng tác viên đó được phép truy cập.
Không sử dụng chế độ công khai “Anyone with the link” cho các tài liệu chứa dữ liệu nhạy cảm của khách hàng.
Tính năng cần bật để ngăn chặn rò rỉ:
Chặn quyền chia sẻ lại của người xem/biên tập viên (Disable options for editors to change permissions and share): Bật tùy chọn ngăn không cho cộng tác viên tự ý mời thêm người lạ hoặc chuyển tiếp quyền truy cập cho bên thứ ba.
Bật tính năng hết hạn quyền truy cập (Access Expiration): Đặt thời hạn tự động thu hồi quyền (ví dụ: sau khi kết thúc dự án hoặc sau vài ngày) để tránh việc tài liệu bị truy cập vĩnh viễn không cần thiết.