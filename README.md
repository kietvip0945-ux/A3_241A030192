# Lab A3: Thiết kế giao diện với XML Layout & Tài nguyên

Bài tập thực hành môn: Lập trình trên các thiết bị di động (INT4211)

## Thông tin sinh viên
- Họ và tên: Lê Hoàng Anh Kiệt
- MSSV: 241A030192

## Môi trường thử nghiệm
- Công cụ: Android Studio Ladybug | 2024.2.1
- Thiết bị: Android Emulator (Pixel LabA1 API 37.2 - sdk_gphone16k_x86_64)
- Hệ điều hành: Android 17 (API 37)

## Các thành phần đã hoàn thành
1. **Quản lý tài nguyên chuẩn:**
   - Tách toàn bộ chuỗi text sang `strings.xml`, màu sắc sang `colors.xml`, khoảng cách dùng `dimens.xml`.
   - Tạo các hình shape XML trong `res/drawable/` (`bg_header.xml`, `bg_avatar.xml`, `bg_stat.xml`).
2. **Giao diện chính (LinearLayout & FrameLayout):**
   - Dựng form đăng nhập theo đặc tả với ScrollView và LinearLayout.
   - Dùng FrameLayout để xếp đè ảnh đại diện tròn lên mép dưới ảnh bìa header.
   - Dùng `view_profile_card.xml` và nhúng vào màn hình bằng thẻ `<include>`.
   - Nút ĐĂNG NHẬP hiển thị Snackbar khi bấm.
3. **Bản dựng phẳng bằng ConstraintLayout:**
   - Tạo `ConstraintDemoActivity` với giao diện phẳng, sử dụng Guideline và các ràng buộc neo.
4. **Hỗ trợ màn hình ngang (layout-land):**
   - Tạo thư mục `res/layout-land/activity_main.xml` với bố cục chia 2 cột linh hoạt khi xoay ngang thiết bị.

## Kết quả kiểm tra (Checkpoints)
- **Checkpoint 1 (Màn hình dọc):** Đã kiểm tra giao diện dọc, nút Đăng nhập hiện Snackbar, Logcat in thông báo nạp `res/layout`.
- **Checkpoint 2 (Màn hình ngang):** Đã kiểm tra xoay ngang máy ảo, giao diện tự chia 2 cột từ `res/layout-land`, Logcat in dòng nạp layout-land thành công.
