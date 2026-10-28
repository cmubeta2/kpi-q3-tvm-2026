# KẾ HOẠCH NÂNG CẤP VÀ CÁC BƯỚC TIẾP THEO (UPDATE.md)

Tài liệu này định hình lộ trình thực hiện các phiên bản nâng cấp tiếp theo của dự án KPI Portal toàn phòng khám.

> **⏸ 20/10/2026:** các bước v2.1–v2.3 dưới đây TẠM DỪNG – chờ Sếp duyệt hướng v3.0 (`KE-HOACH-KPI-TOAN-VIEN-v3-LAM-IT-DUNG-NGAY.md`).

---


> **🚀 CẬP NHẬT 28/10/2026 (Nâng cấp Executive Dashboard v2.0 - Chuẩn UI/UX Pro Max):**
> - Đã nâng cấp toàn diện giao diện Web Báo cáo Điều hành lên tầm cao mới theo tiêu chuẩn UI/UX Pro Max:
>   + Tích hợp Dark Mode / Light Mode thông minh tự động đảo màu Chart.js.
>   + Bố cục Hero Bento Grid (Magic UI) và KPI Metric Cards (Tremor) với vòng tròn tiến độ SVG Circular Ring 99,44%.
>   + Phổ điểm phân vị 13 Xuất sắc - 9 Đạt chuẩn - 4 Cần rà soát cho 26 khoa phòng kèm bộ lọc và tìm kiếm tức thì.
>   + Sử dụng 100% SVG Lucide Icons, bộ phông Plus Jakarta Sans + JetBrains Mono, thông báo Toast Shadcn UI.
>   + Zero horizontal scroll: Tối ưu 100% màn hình điện thoại (Stacked cards).
>   + Website trực tuyến vĩnh viễn: https://cmubeta2.github.io/kpi-q3-tvm-2026/
> - Kế hoạch giai đoạn tới: Tích hợp Database Hub và API xuất báo cáo điều hành tự động cho Ban Giám Đốc.

> **🌐 CẬP NHẬT 28/10/2026 (Triển khai Web Dashboard & Tối ưu Mobile):**
> - Website báo cáo điều hành KPI Quý 3 đã được hoàn thiện giao diện Mobile-first không cuộn ngang và triển khai live trên Internet:
>   + **Cập nhật 28/10 23:30:** Đã đối soát và nạp kết quả chuẩn xác 100% từ file gốc TV3 (sheet DS_TVMCM_2026) cho 26 khoa/phòng kèm chuỗi so sánh Q1, Q2, Q3 và phân tích nguyên nhân 4 khoa <90%.
>   + Đã bổ sung phân hệ đánh giá chi tiết 26 khoa/phòng với bộ lọc khối (Lâm sàng, CLS, Gián tiếp), lọc xếp loại và tìm kiếm nhanh.
>   + Link chính thức (GitHub Pages): https://cmubeta2.github.io/kpi-q3-tvm-2026/
>   + Link Vercel: https://fleet-gold-wcolrdd.tmp.now
>   + Link Netlify: http://exquisite-gumption-f2495f.netlify.app (Mật khẩu: My-Drop-Site)
> - Kế hoạch nâng cấp tiếp theo: Tích hợp công cụ tự động xuất báo cáo PDF chuẩn in ấn A4 bằng 1 click từ giao diện web.

> **📌 CẬP NHẬT 27/10/2026 (Báo cáo Quý 3 hoàn tất):** 
> - Đã hoàn thành bản phân tích và báo cáo KPI Quý 3/2026 (Bao cao KPI Quy 3-2026 - Thanh Vu Medic Ca Mau.md) và Trang Dashboard Điều Hành Doanh Nghiệp tương tác (Bao_Cao_KPI_Q3_2026_Executive_Dashboard.html) với kết quả đạt đỉnh 99,4%.
> - Trọng tâm giai đoạn kế tiếp: Giám sát kế hoạch về đích Q4/2026 (mục tiêu 17,24 tỷ DVYT) và kích hoạt Công cụ 4 (Dựng KPI 2027 từ AOP 2027) trong tháng 11–12/2026 theo đúng khung v3.

## 1. VIỆC CẦN THỰC HIỆN TRONG PHIÊN BẢN KẾ TIẾP (v2.1 — Khởi tạo Database Hub)

- [ ] **Bước 1 — Phê duyệt kế hoạch tổng thể:** Chốt 3 quyết định lớn với Sếp (Mô hình App độc lập hay tích hợp, rào cản sàn/trần công thức, phân quyền phòng nguồn).
- [ ] **Bước 2 — Khởi tạo Google Sheets CSDL chuẩn mới (Database Hub):**
  - Dựng 6 tab: `DM_KhoaPhong`, `DM_ChiSo`, `KH_ChiSo`, `TH_ChiSo`, `DM_NguoiDung_Quyen`, `NHATKY_Audit`.
  - Cấu hình ID tự sinh và định dạng chuẩn.
- [ ] **Bước 3 — Viết Script chuyển đổi (Migration Tool):**
  - Đọc dữ liệu từ file master hiện tại (`1pNd4YkCMECVr9Vu5rAVbK1J-oTZL4DaMjSvuekrj54o`).
  - Đổ 1.117 dòng chỉ số lịch sử và kế hoạch Q1, Q2, Q3, Q4/2026 sang Database Hub.
  - Chạy đối soát số liệu tự động giữa Hub mới và Sheet cũ.

---

## 2. VIỆC CẦN THỰC HIỆN Ở PHIÊN BẢN v2.2 (MVP Core Engine & Dashboard BGĐ)

- [ ] Khởi tạo dự án Apps Script Web App `KPI_Portal_TVM` với clasp + Git.
- [ ] Xây dựng thư viện tính toán máy chủ `CalculationEngine.gs`.
- [ ] Dựng Dashboard Ban Giám đốc với chế độ xem dữ liệu thực tế Q1, Q2, Q3.
- [ ] Xây dựng bảng nhiệt hiển thị sức khỏe 26 khoa/phòng.

---

## 3. VIỆC CẦN THỰC HIỆN Ở PHIÊN BẢN v2.3 (Phân hệ Nhập liệu & Ký duyệt)

- [ ] Phân hệ Trưởng khoa/phòng nộp minh chứng Drive và nhập giải trình.
- [ ] Phân hệ 4 phòng nguồn (`TCKT`, `PTKH`, `KHTH`, `TCNS`) cấp số liệu batch.
- [ ] Workflow ký duyệt điện tử 2 pha + thông báo qua Bot Telegram & 🔔 App.
- [ ] Module sinh Báo cáo Quý tự động (PDF tóm tắt).
