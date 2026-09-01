# Báo cáo dự án Home Credit phase 1

## 1. Mục tiêu dự án

- Tìm hiểu xem tôi có thể làm được những gì khi đứng trước 1 dataset lớn, khi bộ công cụ hầu như chưa có gì. 
- Tìm hiểu về domain rủi ro trong lĩnh vực tài chính tiêu dùng

## 2. Những gì đã làm

- Phân tích rủi ro vỡ nợ ra làm những tiêu chí: Độ tuổi, thu nhập, trình độ học vấn, các gói vay, thời gian đi làm,...
 - Xử lý outlier ở độ tuổi

## 3. Dữ liệu cho thấy điều gì?

- Rủi ro về học vấn: 
    - Nhóm có trình độ cấp 2 và cấp 3 thường bùng nợ nhiều hơn so với các nhóm có trình độ cao hơn. Tỷ lệ bùng nợ của nhóm có trình đô học vấn cấp 2 là 10.93%, và nhóm cấp 3 là 8,94%, cao hơn trung bình (8,04%)
    - Vì sao lại như vậy?
        - Nhóm học vấn thấp thường sẽ phải làm các công việc phổ thông, thu nhập thấp và thiếu tính ổn định, đồng thời kết hợp việc thiếu kĩ năng quản lý tài chính cá nhân, dẫn đến mất khả năng trả nợ
        - Nhóm học vấn cao: sở hữu công việc chuyên môn, thu nhập cao, dòng tiền ổn định, có nhận thức tài chính tốt hơn, ít có khả năng vay quá khả năng chi trả của bản thân

- Rủi ro về thu nhập: 
    - Thu nhập cao giúp giảm khả năng vỡ nợ. Nhóm 10% thu nhập cao nhất thì chỉ có 6.2% người vỡ nợ.
    - Tỷ lệ nợ trên thu nhập càng cao thì khả năng vỡ nợ càng cao. Tuy nhiên nó xuất hiện ở các điểm dị biệt (median là 3.27). 
    - Nếu để mốc chặn cho vay ở mức 3-5 lần thu nhập thì sẽ giảm rủi ro vỡ nợ. 


- Rủi ro về độ tuổi: 
    - Nhóm 21-40 tuổi có tỷ lệ vỡ nợ cao vượt mức trung bình, đỉnh điểm nằm ở tuổi 21-25. Từ sau 40 tuổi, rủi ro vỡ nợ giảm mạnh. 
    - Vì sao? Tuổi trẻ 21-40 thường là những người mới tham gia thị trường lao động, thu nhập thấp nhưng lại muốn sắm nhiều. Dòng tiền không ổn định dẫn đến mất khả năng trả nợ. Còn nhóm 40 đổ lên, thu nhập bền vững, sẽ giảm khả năng vỡ nợ hơn. 

- Rủi ro theo số năm làm việc:
    - Dữ liệu được chia làm 3 nhóm chính. Nhóm Mới đi làm (<= 5 năm) chiếm phần đông nhưng có tỷ lệ vỡ nợ cao nhất (10.5%).
    - Ngược lại, thâm niên càng cao rủi ro càng giảm: Nhóm Lâu năm (>5 năm) rủi ro chỉ 6.3%. Đặc biệt, nhóm Ngoại lai (Outlier - chủ yếu là người nghỉ hưu) lại là nhóm an toàn nhất toàn hệ thống với chỉ 5.3%.

    - Nguyên nhân: 
        -  Mới đi làm: Thường là người trẻ, nhu cầu tiêu dùng cao (mua xe, điện thoại, kết hôn) nhưng luồng tài chính chưa vững vàng, công việc dễ biến động.
        - Lâu năm: Công việc và chức vụ đã ổn định, dòng tiền đều đặn, đã quen với việc quản lý chi tiêu.
        - Người nghỉ hưu: Có nguồn thu nhập cố định và an toàn tuyệt đối (lương hưu của Nhà nước). Tâm lý tài chính thận trọng và ít chịu áp lực chi tiêu bốc đồng như người trẻ.

- Tỷ lệ vay Cash Loans nhiều hơn so với Revolving Loans (Vay trả góp). Và số lượng người vỡ nợ cũng cao hơn hẳn. 
    - Nguyên nhân là do Cash Loans là khoản vay theo kiểu 1 cục, điều kiện đầu vào nới lỏng hơn, thu hút nhóm khách hàng đang có thu nhập bấp bênh.
    - Còn thẻ tín dụng thì sẽ thẩm định khắt khe hơn. Và nếu KH bùng nợ thẻ tín dụng, thường sẽ có lịch sử nợ xấu kéo dài.

## 4. Giải pháp đề xuất :
- Thẩm định kĩ lưỡng các khoản vay có tỷ lệ nợ trên thu nhập cao.

- Áp dụng mô hình chấm điểm tín dụng nghiêm ngặt hơn cho các nhóm vay tiền mặt. 

-  Đối với nhóm trẻ, người mới đi làm: cần cân nhắc cho vay số tiền dựa trên 3-5 lần thu nhập. Đồng thời kiểm tra lịch sử trả nợ, công việc, thu nhập, bằng cấp, số năm làm việc. Nếu 6-12 tháng đủ uy tín trả nợ thì sẵn sàng tăng thêm hạn mức.

- Đối với nhóm trung niên (40 tuổi trở lên): Có thể cân nhắc cho vay số tiền lớn hơn, dựa trên thu nhập và số năm làm việc ổn định. Thiết kế các gói bán chéo các sản phẩm thẻ tín dụng, thiết kế gói vay ưu đãi lãi suất, thủ tục nhanh.