# E-commerce UI Improvement

## 1. Giới thiệu

Đây là dự án cải tiến giao diện người dùng (UI) cho một phần của website thương mại điện tử Hasaki.vn. Sau khi khảo sát trải nghiệm mua sắm thực tế, tôi nhận thấy khu vực thẻ sản phẩm (Product Card) trên trang chủ hiển thị khá rối mắt do có quá nhiều nhãn dán khuyến mãi. Do đó, tôi đã thiết kế lại thẻ sản phẩm theo hướng tối giản, giúp khách hàng dễ dàng tập trung vào thông tin quan trọng nhất: hình ảnh sản phẩm và giá cả.

## 2. Website tham khảo

- **Tên website:** Hasaki.vn
- **URL:** https://hasaki.vn/
- **Nhóm sản phẩm:** Chăm sóc da mặt (Dược mỹ phẩm, chăm sóc da nhạy cảm).
- **Khách hàng mục tiêu:** Người có làn da nhạy cảm, có nhu cầu tìm mua sản phẩm chính hãng với giá tốt.
- **Khu vực đã khảo sát:** Trang chủ, Danh mục sản phẩm, Chi tiết sản phẩm, Tìm kiếm, Giỏ hàng.

### Bảng khảo sát chi tiết 5 khu vực giao diện:

| Khu vực                  | Chức năng đang cung cấp                                                              | Điểm hợp lý                                                                                                | Điểm có thể cải thiện                                                                                              | Đề xuất cải tiến                                                                                            |
| :----------------------- | :----------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------- |
| **1. Trang chủ**         | Hiển thị Flash Deal đếm ngược, tab danh mục, thẻ sản phẩm có nút thêm nhanh vào giỏ. | Đồng hồ đếm ngược và nhãn báo "số lượng có hạn" tạo hiệu ứng FOMO tốt. Giá sale nổi bật.                   | Thẻ sản phẩm bị nhồi nhét quá nhiều nhãn dán (Freeship, giờ sale, % giảm) làm che khuất hình ảnh.                  | Thiết kế lại thẻ sản phẩm tối giản hơn. Gom các nhãn thành icon nhỏ đặt gọn ở góc ảnh để không gây rối mắt. |
| **2. Danh mục sản phẩm** | Menu phân loại theo ngành hàng dạng tab ngang (Chăm sóc da mặt, trang điểm...).      | Tab đang chọn đổi màu cam nổi bật. Nút "Thêm" giúp menu gọn gàng.                                          | Danh mục xổ xuống có các ngành không liên quan (Tai nghe, Camera). Thiếu bộ Lọc và Sắp xếp trong trang Flash Deal. | Bổ sung nút Lọc (theo loại da, thương hiệu) và loại bỏ các ngành hàng không phải thế mạnh cốt lõi.          |
| **3. Chi tiết sản phẩm** | Hiển thị ảnh, giá, mô tả, thành phần, HDSD, đánh giá, hỏi đáp.                       | Thiết kế dạng tab (Mô tả, Thành phần...) giúp trang gọn gàng. Hiển thị rõ số tiền tiết kiệm được.          | Ảnh thực tế từ khách hàng khá nhỏ. Giao diện lọc đánh giá (5 sao, 4 sao) bị nhạt nhòa, khó bấm.                    | Phóng to khu vực ảnh feedback của khách. Đổ màu nền cho các nút lọc đánh giá để tăng tính tương tác.        |
| **4. Tìm kiếm**          | Ô tìm kiếm trung tâm. Dropdown gợi ý ngay logo thương hiệu lớn và ngành hàng hot.    | Việc có sẵn logo thương hiệu giúp khách có da nhạy cảm truy cập nhanh vào hãng quen thuộc mà không cần gõ. | Dropdown gợi ý còn hiển thị ngành hàng công nghệ. Thiếu khu vực "Lịch sử tìm kiếm gần đây".                        | Thêm phần "Lịch sử tìm kiếm" để cá nhân hóa, bỏ các gợi ý ngành hàng không liên quan đến làm đẹp.           |
| **5. Giỏ hàng**          | Hiển thị danh sách món hàng, quà tặng kèm, tạm tính, mã giảm giá và nút Đặt hàng.    | Bố cục 2 cột rõ ràng. Minh bạch về quà tặng kèm, cho phép khách tự tick chọn quà.                          | Text mô tả quà tặng quá dài làm thẻ sản phẩm bị phình to. Thiếu ô nhập mã giảm giá trực tiếp tại giỏ.              | Rút gọn mô tả quà tặng bằng thanh gập (accordion). Bổ sung ô nhập mã voucher ngay trên phần Tạm tính.       |

_(Lưu ý thêm: Trong luồng Đặt hàng/Checkout, hệ thống có yêu cầu xác thực số điện thoại bằng mã OTP qua SMS. Đây là một điểm UX rất tốt để bảo mật và chống giao hàng sai địa chỉ)._

## 3. Chức năng

_(Ghi chú: Phần này điền sau khi bạn code xong Nhiệm vụ 3)_

- Hiển thị danh sách sản phẩm mẫu với hình ảnh, tên và giá.
- Bố cục responsive, tự động điều chỉnh số cột (hiển thị 4 cột trên PC, 2 cột trên Mobile).
- Hiệu ứng hover nổi bật thẻ sản phẩm.

## 4. Công nghệ

- HTML5
- CSS3

## 5. Cách chạy

Mở file `index.html` bằng trình duyệt web bất kỳ (Chrome, Edge, Safari...).

## 6. Cải tiến đã thực hiện

_(Ghi chú: Cập nhật sau khi code xong)_

- **Vấn đề ban đầu:** Thẻ sản phẩm trên Hasaki có quá nhiều text và nhãn dán đè lên ảnh.
- **Thay đổi:** Tôi đã viết lại cấu trúc thẻ sản phẩm, di chuyển phần % giảm giá thành một badge nhỏ ở góc. Loại bỏ các text không cần thiết để tạo không gian trắng (white space) giúp giao diện sang trọng và tập trung vào sản phẩm hơn.

## 7. Hỗ trợ từ AI

Tôi đã sử dụng AI (Gemini) để đóng vai trò như một người hướng dẫn (mentor). AI giúp tôi phân tích sâu hơn về mặt UX (trải nghiệm người dùng) của Hasaki, gợi ý cách lập bảng khảo sát khoa học. Tuy nhiên, toàn bộ dữ liệu khảo sát đều dựa trên ảnh chụp thực tế do tôi tự trải nghiệm và cung cấp.
