# BÁO CÁO ĐIỀU HÀNH KPI TOÀN VIỆN QUÝ 3/2026 — THANH VŨ MEDIC CÀ MAU

Executive Management Dashboard v2.0 (UI/UX Pro Max Edition) — Phòng khám Đa khoa Thanh Vũ Medic Cà Mau (TV3)

## 🌐 Đường Dẫn Trực Tuyến (Live Web)
- **Website chính thức (GitHub Pages - Vĩnh viễn):** [https://cmubeta2.github.io/kpi-q3-tvm-2026/](https://cmubeta2.github.io/kpi-q3-tvm-2026/)
- **Vercel Deploy:** [https://fleet-gold-wcolrdd.tmp.now](https://fleet-gold-wcolrdd.tmp.now)
- **Netlify Deploy:** [http://exquisite-gumption-f2495f.netlify.app](http://exquisite-gumption-f2495f.netlify.app) (Mật khẩu: `My-Drop-Site`)

---

## 🎨 Điểm Nhấn Kiến Trúc UI/UX Pro Max v2.0
1. **Design Tokens & Dark/Light Mode:**
   - Hệ màu ngữ nghĩa y tế tiêu chuẩn: Primary Sky (`#0284c7`), Success Emerald (`#059669`), Warning Amber (`#d97706`), Danger Red (`#dc2626`).
   - Nút chuyển Dark Mode / Light Mode lưu trạng thái `localStorage` và tự động cập nhật màu biểu đồ Chart.js (trục tọa độ, lưới grid, tooltip).
2. **Typography Chuyên Sâu:**
   - `Plus Jakarta Sans`: Đảm bảo độ rõ ràng, quyền uy của văn bản điều hành.
   - `JetBrains Mono`: Dành riêng cho số liệu bảng biểu, mã chỉ tiêu (F1-L6), tỷ lệ phần trăm và các chỉ số tiền tệ để ngăn nhảy giật bố cục khi lọc.
3. **Hero Bento Grid & Tremor Metrics:**
   - Vòng tròn tiến độ SVG Circular Ring `99,44%` với hiệu ứng nét vẽ mượt mà.
   - 4 Thanh đo trụ cột Balanced Scorecard (Tài chính 99,0%, Khách hàng 96,0%, Vận hành 99,5%, Phát triển 100,0%).
   - Thẻ theo dõi thặng dư chi phí vật tư: Tiết kiệm **1,07 tỷ VNĐ** (13,00% vs trần 14,50%).
   - Thẻ đòn bẩy chất lượng: ARPU **421.741 VNĐ** (+11,1%) & Tỷ lệ tái khám đúng hẹn **67,40%** (+12,4pp).
4. **Phổ Điểm Hiệu Suất 26 Khoa/Phòng:**
   - Thanh phân bổ phổ điểm: 13 Xuất sắc (50%) - 9 Đạt chuẩn (34,6%) - 4 Cần rà soát (15,4%).
   - Bộ lọc khối (Lâm sàng, Cận lâm sàng, Gián tiếp) và ô tìm kiếm tức thì.
5. **Chuẩn Mực Vector SVG (Không dùng Emoji làm icon):**
   - 100% biểu tượng hệ thống sử dụng Lucide SVG vector sắc nét.
6. **Triệt Tiêu 100% Cuộn Ngang (Zero Horizontal Scroll):**
   - Tối ưu 100% di động: Bảng dữ liệu tự động chuyển thành các thẻ Bento xếp chồng trên smartphone.
   - Kích thước vùng chạm tương tác chuẩn $\ge 44 	imes 44\text{px}$.
7. **Tương Tác Nâng Cao & Toast Notification:**
   - Nút sao chép tóm tắt điều hành với Toast notification phong cách Shadcn UI.
   - Print CSS chuyên nghiệp tối ưu xuất PDF/in ấn trên khổ giấy A4.
