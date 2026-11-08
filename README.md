# 🏥 TTA_PediaInfect-clinical (v4.0 Enterprise — Full RBAC & 60 Clinical Cases)
**Hệ sinh thái Trí tuệ Lâm sàng & Đồng hành Nhi khoa (Pediatric Clinical & Diagnostic Intelligence Platform)**

- **Đơn vị triển khai:** BỆNH VIỆN NHI HÀ NỘI — ĐƠN NGUYÊN DI TRUYỀN VÀ SINH HỌC PHÂN TỬ
- **Chịu trách nhiệm chuyên môn & Bản quyền hệ thống:** ThS. Trần Tuấn Anh (`anhtran.nihbt@gmail.com`)
- **Database Google Sheets chính thức (`[CSDL_PediaInfect_Clinical_HNH]`):** https://docs.google.com/spreadsheets/d/133wiY_agfPHAGx2NRr01oyot2ssmPSd54xEcvf21iX8/edit
- **Database Phả hệ Di truyền (`[CSDL_PhaHe_DiTruyen_NSGC]`):** https://docs.google.com/spreadsheets/d/1AfSU8iW4mR0sK8-ld6Vv8PZmCbwqCebAonfjmOvlNvo/edit
- **Google Apps Script Project (`PediaInfect-clinical`):** https://script.google.com/d/1ZB0wp01-W6r0L-4ol6arhIW36zSaiW8UioV5EbYPZ58TgYQ58P-E9Y4g/edit

## 🚀 Các nâng cấp trọng tâm trong Phiên bản v4.0
1. **Quản trị Phân quyền Tài khoản (`Allowed_Users`) Toàn diện (CRUD & RBAC):**
   - Tài khoản Primary Admin (`anhtran.nihbt@gmail.com`) có biểu mẫu trực quan ngay tại **Mục 4** để **Thêm mới / Sửa thông tin / Đổi mật khẩu / Phân quyền Khoa (`Department`) & Phạm vi dữ liệu (`Data_Scope`) / Tích chọn 6 quyền chi tiết (`Permissions_JSON`) / Gia hạn `Access_Expires_At` / Khóa - Mở khóa / Xóa User**.
   - Tích hợp sẵn 4 nút mẫu phân quyền nhanh (`Bác sĩ Khoa SCOPE_DEPT`, `Chuyên gia SHPT SCOPE_LAB`, `Bác sĩ Nội trú SCOPE_ASSIGNED`, `Quản trị Toàn viện SCOPE_ALL`) và đồng bộ 2 chiều với Google Sheets `CSDL_PediaInfect_Clinical_HNH`.
2. **Liên kết Truy cập nhanh (1-Click Quick Links) vào Database `CSDL_PediaInfect_Clinical_HNH`:**
   - Gắn nút mở trực tiếp bảng tính Google Sheets `CSDL_PediaInfect_Clinical_HNH` ngay trên Thanh Header (khi đăng nhập Admin), trên Banner Quản trị tối cao, tại Mục 1 (Cấu hình REST API) và tại tiêu đề Mục 4 (`Allowed_Users`).
3. **Thư viện 60 Ca bệnh Lâm sàng & Sinh học phân tử Điển hình (`BN01` – `BN60`):**
   - Bao phủ 6 nhóm chuyên khoa: Hô hấp & Kháng thuốc (16 ca), Truyền nhiễm & Dịch bệnh theo mùa (12 ca), Thần kinh - TKTW (11 ca), Tiêu hóa - Gan mật (10 ca), Sơ sinh - NICU - Hồi sức - Tiết niệu (12 ca), và Chuyên đề Bẫy Biện giải Sinh học Phân tử & Di truyền Dược lý (`MT-RNR1 m.1555A>G`, `G6PD Viangchan`, `ciHHV-6`, bài xuất chủng vắc-xin Rotavirus, mẫu tỵ hầu lẫn nước bọt...).
   - Hỗ trợ tìm kiếm tức thì theo Mã bệnh nhi, tên bệnh, tác nhân PCR, đột biến gen kháng thuốc (`23S rRNA A2063G/A2064G`, `mecA`, `blaNDM-1`, `blaOXA-23`) và lọc theo từng chuyên khoa.
