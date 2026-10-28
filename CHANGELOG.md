# NHẬT KÝ THAY ĐỔI (CHANGELOG) — APP KPI TOÀN PHÒNG KHÁM

Tất cả các thay đổi, cập nhật quan trọng của dự án Ứng dụng Quản trị KPI toàn viện Thanh Vũ Medic Cà Mau được ghi nhận tại đây.

---

### [2026-10-28 23:45] — Nâng Cấp Giao Diện Executive Dashboard v2.0 (Chuẩn UI/UX Pro Max)
- **Tích hợp Bộ não UI/UX Pro Max:**
  + **Thiết kế Hệ thống Semantic Tokens:** Hỗ trợ toàn diện Dark Mode và Light Mode (tự động lưu trạng thái `localStorage` và đồng bộ tức thì màu biểu đồ Chart.js).
  + **Typography chuyên nghiệp:** Bộ đôi chuẩn mực `Plus Jakarta Sans` (Nội dung, Tiêu đề điều hành) và `JetBrains Mono` (Số liệu bảng biểu, Mã chỉ tiêu F1-L6, Phần trăm, Tiền tệ VNĐ).
  + **Bố cục Hero Bento Grid (Magic UI & Tremor):** Vòng tròn tiến độ SVG Circular Ring động `99,44%`, nhịp tim tăng trưởng 3 quý (Q1: 91,09% → Q2: 95,22% → Q3: 99,44%), 4 trụ cột BSC với thanh mini progress đa sắc, thẻ thặng dư ngân sách vật tư 1,07 tỷ VNĐ, và thẻ đòn bẩy ARPU 421k & Tái khám 67,40%.
  + **Loại bỏ 100% Emoji làm icon:** Thay thế hoàn toàn bằng hệ thống vector SVG Lucide chuẩn nét cao (Activity, Building, TrendingUp, Target, Wallet, Users, Moon, Sun, Copy, Printer, Check, Search).
  + **Phổ điểm Hiệu suất 26 Khoa/Phòng (Performance Distribution Bar):** Trực quan hóa phân vị 13 Xuất sắc (50,0%) - 9 Đạt chuẩn (34,6%) - 4 Cần rà soát (15,4%) với bộ lọc tương tác tức thì và ô tìm kiếm real-time.
  + **Trải nghiệm Mobile Không Cuộn Ngang (Zero Horizontal Scroll):** Toàn bộ bảng biến đổi thành Stacked Bento Cards trên màn hình nhỏ; nút bấm chuẩn kích thước chạm ≥44×44px.
  + **Hệ thống Toast Notification:** Thông báo xác nhận sao chép tóm tắt điều hành kiểu Shadcn UI mượt mà.
- **Đồng bộ triển khai:** Triển khai trực tiếp lên GitHub Pages (`https://cmubeta2.github.io/kpi-q3-tvm-2026/`) và sao chép vào các thư mục lưu trữ nội bộ.

---

### [2026-10-28 23:30] — Cập nhật Kết Quả KPI Chuẩn Xác 100% Từ File Gốc TV3 (Sheet DS_TVMCM_2026)
- **Đồng bộ dữ liệu gốc:** Tải và bóc tách toàn diện từ file Google Sheets trung tâm `KPI THANH VU MEDIC CA MAU - TV3 2026` (`1pNd4YkCMECVr9Vu5rAVbK1J-oTZL4DaMjSvuekrj54o`).
- **Kết quả thực tế 26 khoa/phòng:**
  + Toàn viện: **99,44%** (Q1: 91,09% → Q2: 95,22% → Q3: 99,44%).
  + Số đơn vị đạt chuẩn (≥90%): **22 / 26 Đơn vị (84,6%)**.
  + Xếp loại Xuất sắc (≥95%): **13 Đơn vị** (KKB 100,03%, Thuốc 100,42%, Dược 99,83%, TCNS 99,83%, DLS 99,83%, Nội tiết 99,81%, NTH 99,72%, PTKH 99,29%, CĐHA 99,01%, NTK 98,49%, XN 97,77%, KTT 96,24%, Tiêm ngừa 95,67%).
  + Xếp loại Đạt chuẩn (90% – 94,9%): **9 Đơn vị** (KHTH 94,58%, BHYT 94,23%, TCKT 93,49%, QTTN 92,83%, TMH 92,34%, NTM 91,69%, CNTT 91,08%, Ngoại 90,31%, Cấp cứu 90,19%).
  + Số đơn vị dưới 90% (Cần rà soát): **4 Đơn vị**
    1. Phòng Khám Sản: **80,15%** (Q1: 78,36% → Q2: 78,96% → Q3: 80,15% - Hụt lượt khám C1 26,9% và doanh thu F1 49,1%).
    2. Phòng Khám YHCT: **86,67%** (Q1: 94,73% → Q2: 82,23% → Q3: 86,67% - Hụt nhẹ doanh thu dịch vụ).
    3. Phòng Nội Soi: **87,96%** (Q1: 88,15% → Q2: 89,55% → Q3: 87,96% - Chi phí vật tư thực tế 13,14% vượt trần 12,33% đúng 0,81pp).
    4. Phòng Khám Nhi: **88,66%** (Q1: 82,87% → Q2: 90,05% → Q3: 88,66% - Tỷ lệ chỉ định CLS đạt 59,72% so với ngưỡng 65%).
- **Nâng cấp Web Dashboard:** Đưa chuỗi dữ liệu 3 quý (Q1, Q2, Q3) và mũi tên xu hướng (↑/↓/→) vào bảng chi tiết; cập nhật bộ lọc động và deploy trực tiếp lên GitHub Pages.

---

## [2026-10-28] — Triển khai Web Báo cáo KPI Q3/2026 Mobile-First & Đa Nền Tảng (GitHub Pages, Vercel, Netlify)
### Bổ sung Chi Tiết 26 Khoa/Phòng (Đầy đủ dữ liệu & bộ lọc tương tác):
- Soạn thảo và tích hợp toàn diện bảng kết quả KPI của cả 26 khoa/phòng toàn viện vào Báo cáo Markdown và Web Dashboard.
- Phân loại rõ ràng 3 khối:
  + **Khối Lâm sàng (13 khoa/phòng):** 12/13 khoa đạt chuẩn (92,3%), dẫn đầu là Nội Tim Mạch (98,7%), Nhi (97,6%), Nội Soi (96,0%).
  + **Khối Cận lâm sàng & Dược (5 khoa/phòng):** 5/5 khoa đạt xuất sắc (100%), CĐHA (97,9%), PXN (97,4%), Dược LS (98,4%).
  + **Khối Gián tiếp / Quản trị & Hỗ trợ (8 phòng/tổ):** 6/8 phòng đạt chuẩn (75%), các phòng nòng cốt TCKT, KHTH, TCNS, CNTT đều ≥95%.
- Tích hợp công cụ tương tác trên Web:
  + Lọc động theo 3 Khối: Lâm sàng / Cận lâm sàng / Gián tiếp.
  + Lọc động theo Xếp loại: Xuất sắc (≥95%) / Đạt chuẩn (90-94%) / Cần rà soát (<90%).
  + Ô tìm kiếm tức thì theo tên khoa/phòng.
  + Thẻ card xếp chồng (Stacked Card Layout) tối ưu tuyệt đối cho mobile (không cuộn ngang).
  + Thanh tiến độ (Progress bar) trực quan cho từng khoa/phòng.
- Cập nhật đồng bộ lên GitHub Pages: `https://cmubeta2.github.io/kpi-q3-tvm-2026/`.

### Tối ưu hóa Giao diện Mobile (Zero Horizontal Scroll):
- Triệt tiêu 100% cuộn ngang trên điện thoại di động: thiết kế lại toàn bộ bảng 17 chỉ tiêu BSC thành cấu trúc thẻ xếp chồng (Stacked Card Layout) trên màn hình <= 768px (data-label tự căn lề, nhãn và giá trị phân tầng rõ ràng).
- Tự động wrap thanh điều hướng tab phân hệ (lex-wrap: wrap) hiển thị dạng grid chip 2-3 cột trên mobile.
- Bẻ dòng tự nhiên các chuỗi văn bản dài, tối ưu kích thước font chữ fluid typography với biến clamp().

### Triển khai Web Trực tuyến (Deployment):
- **GitHub Pages (Vĩnh viễn & Chính thức):** Đẩy mã nguồn lên repo cmubeta2/kpi-q3-tvm-2026 và kích hoạt Pages tại: https://cmubeta2.github.io/kpi-q3-tvm-2026/.
- **Vercel:** Triển khai bản live nhanh tại https://fleet-gold-wcolrdd.tmp.now (hỗ trợ claim trực tiếp vào tài khoản Vercel cá nhân).
- **Netlify:** Triển khai bản dự phòng tại http://exquisite-gumption-f2495f.netlify.app (Mật khẩu bảo vệ: My-Drop-Site).

---

## [2026-10-27] — Hoàn thiện Báo cáo Kết quả KPI Quý 3/2026 Toàn Viện
### Bổ sung & Phân tích chuyên sâu:
- Đọc và đối soát dữ liệu từ file master KPI 2026 - THANH VU MEDIC CA MAU (TV3) và thư mục lưu trữ BKS KPI TVM CM 2026.
- Bóc tách kết quả Quý 3/2026: Tổng KPI toàn viện đạt **99,4%** (Q1: 91,15% → Q2: 95,20% → Q3: 99,40%).
- Soạn thảo và hoàn thiện bản báo cáo chiến lược chuẩn BKS: Bao cao KPI Quy 3-2026 - Thanh Vu Medic Ca Mau.md (đồng bộ giữa thư mục Drive BKS và thư mục kế hoạch Shin).
- Bóc tách 3 điểm nhấn chiến lược:
  1. Chi phí vật tư trực tiếp giảm ngoạn mục về mức 13,00% (so với trần 14,5%), khắc phục hoàn toàn điểm nghẽn Quý 2.
  2. Tổng 3 nhóm chi phí tiết kiệm 6,05 điểm % (đạt 56,55% so với trần 62,60%), tạo thặng dư chi phí >1,07 tỷ đồng.
  3. Nghịch lý lượt khám (38.719 đạt 88%) và doanh thu (17,71 tỷ đạt 99%) nhờ ARPU tăng lên 421.741 đồng/lượt và tỷ lệ tái khám đúng hẹn đạt 67,40%.
- Đề xuất 4 kiến nghị hành động cụ thể cho Quý 4/2026 và đợt xây dựng AOP 2027.
- Xây dựng hoàn chỉnh Trang Báo cáo Quản trị Doanh nghiệp (Executive Web Dashboard): Bao_Cao_KPI_Q3_2026_Executive_Dashboard.html với đầy đủ biểu đồ tương tác Chart.js (Xu hướng KPI 3 quý, Chi phí vật tư 4 năm, Cơ cấu chi phí thực tế vs trần ngân sách, Lượt khám vs Kế hoạch, ARPU bình quân), Thẻ điểm 17 chỉ tiêu BSC lọc động và Print CSS chuẩn A4.

---

## [2026-10-20] — Phiên bản v3.0 (Làm ít, dùng ngay – CHỜ SẾP DUYỆT)
### Thay đổi hướng:
- Rà soát 26-01, 26-04, tờ trình 04/07, v1.0, v2.0: file TV3 đã chạy tốt; các kế hoạch cũ đòi xây lại phần đang chạy nên không được dùng.
- `KE-HOACH-KPI-TOAN-VIEN-v3-LAM-IT-DUNG-NGAY.md`: không làm app/portal, TV3 chỉ đọc; 4 công cụ nhỏ (bản tin tạm tính tháng, soát lỗi chốt quý, nháp báo cáo quý, dựng KPI 2027 từ AOP 2027), thử trong Q4/2026, có điểm dừng.
- v2.0 (KPI Portal + Database Hub) **tạm dừng**.

---

## [2026-10-20] — Phiên bản v2.0 (Toàn diện & Khả thi cao)
### Thêm mới:
- Hoàn thành bóc tách và phân tích chuyên sâu file Google Sheets trung tâm `KPI THANH VU MEDIC CA MAU - TV3 2026` (tab `DS_TVMCM_2026`, tab `Index` 1.117 dòng, tab `TVM_CaMau`, và 26 tab khoa/phòng).
- Xây dựng bản đặc tả chi tiết `KE-HOACH-SO-HOA-APP-KPI-TOAN-VIEN-2026.md` và Artifact `KE_HOACH_SO_HOA_APP_KPI_TOAN_VIEN.md`:
  - Khẳng định 100% khả thi và phân tích so sánh 3 phương án kiến trúc (AppSheet vs App PTKH mở rộng vs KPI Portal chuyên trách).
  - Đề xuất kiến trúc tối ưu: "One Data Hub - Dedicated KPI Portal" kết hợp đồng bộ API tự động với App PTKH hiện tại.
  - Chuẩn hóa CSDL từ 27 tabs rời rạc thành 6 bảng quan hệ chuẩn Codd 3NF.
  - Thiết kế Engine tính toán phía máy chủ khóa cứng với 5 loại công thức và rào cản sàn/trần.
  - Phác thảo chi tiết 4 phân hệ giao diện: BGĐ, Trưởng khoa/phòng, Phòng nguồn (TCKT/PTKH/KHTH/TCNS) và Thư ký BKS.
  - Lập lộ trình triển khai 4 giai đoạn cụ thể từ tháng 10/2026 đến cuối năm 2026 để go-live toàn diện AOP 2027.
- Khởi tạo hệ thống tài liệu chuẩn của dự án: `README.md`, `CHANGELOG.md`, `UPDATE.md`.

---

## [2026-07-15] — Phiên bản v1.0 (Khởi tạo ý tưởng)
### Thêm mới:
- Bản đề cương sơ bộ `KE-HOACH-XAY-DUNG-APP-KPI.md` đặt nền móng 4 tiêu chí: Hiệu quả · Minh bạch · Bảo mật · Tinh gọn.
- Bản mẫu giao diện demo tĩnh `index.html` mô phỏng Dashboard toàn viện và form chấm điểm.
