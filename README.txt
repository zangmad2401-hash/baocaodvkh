SFINANCE QA AUTO REPORT

Cách dùng offline:
1. Mở thư mục dist.
2. Bấm đúp index.html bằng Chrome hoặc Edge.
3. Có thể bấm "Tải file Excel mẫu" ngay trên web. Luôn giữ file
   QA_Data_Report.xlsx cùng thư mục với index.html khi đưa lên GitHub Pages.
4. Chọn QA_Data_Report.xlsx.
5. Điều chỉnh tạm các KPI/nhận xét và xem dashboard Power BI-style.
6. Bấm Tạo PowerPoint.

Các điều chỉnh trên web không ghi ngược vào file Excel. Website lưu bản tổng hợp
gần nhất trong localStorage của trình duyệt (không lưu dữ liệu thô của từng khách hàng).

Đưa lên GitHub Pages:
1. Đưa toàn bộ nội dung thư mục dist lên repository.
2. Trong Settings > Pages, chọn Deploy from a branch.
3. Chọn branch chứa index.html và thư mục /(root).

Dữ liệu Excel được xử lý trong trình duyệt và không gửi lên máy chủ.

LƯU Ý VỀ CHIA SẺ DỮ LIỆU GIỮA NHIỀU NGƯỜI
- GitHub Pages là website tĩnh. localStorage chỉ giúp cùng một máy/trình duyệt xem lại
  báo cáo gần nhất; người dùng ở máy khác không tự thấy dữ liệu đó.
- Để mọi người cùng thấy báo cáo gần nhất, cần kết nối một cơ sở dữ liệu có xác thực
  (ví dụ Supabase). Chỉ nên lưu snapshot KPI/bảng tổng hợp, không lưu Excel raw,
  số điện thoại, số hợp đồng hoặc dữ liệu định danh.
