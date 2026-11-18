#  [Bài thực hành 2] Xây dựng chuỗi Prompt viết bài PR sản phẩm công nghệ
## BƯỚC 1: Phân tích khách hàng & Nỗi đau (Context Discovery)
**Mục tiêu: Tạo nền tảng dữ liệu thô chuẩn xác để các bước sau bám sát, tránh viết lan man.**
*plaintext* 
Đóng vai Chuyên gia Nghiên cứu Thị trường B2B. Tôi sắp ra mắt sản phẩm [Tên sản phẩm - Giải pháp AI Chatbot tự động hóa CSKH & Chốt đơn cho doanh nghiệp SME]. 

Hãy phân tích đối tượng khách hàng mục tiêu (Chủ doanh nghiệp, Trưởng phòng CSKH/Marketing) và liệt kê 5 nỗi đau (Pain points) lớn nhất họ đang gặp phải khi vận hành thủ công.

Yêu cầu định dạng đầu ra (Bắt buộc dùng cấu trúc JSON hoặc Markdown liệt kê rõ ràng để làm đầu vào cho bước sau):
- Đối tượng mục tiêu: [Mô tả ngắn gọn]
- Danh sách 5 Pain Points: [Tên nỗi đau] -> [Hệ quả thực tế] -> [Cách AI Chatbot giải quyết]
- Từ khóa SEO chính: [3-5 từ khóa]
## BƯỚC 2: Thiết lập Dàn ý chuẩn SEO (Structure & Planning)
**Mục tiêu: Kế thừa dữ liệu từ Bước 1 để dựng khung bài viết 1000 - 1500 từ có tính logic cao.**
*plaintxt*
Đóng vai Biên tập viên Nội dung PR cấp cao. Dựa trên dữ liệu nghiên cứu khách hàng dưới đây:
"""
[DÁN TOÀN BỘ OUTPUT CỦA BƯỚC 1 VÀO ĐÂY]
"""

Hãy lập dàn ý chi tiết cho một bài PR chuyên sâu (dài 1000 - 1500 từ) giới thiệu giải pháp AI Chatbot trên. 

Yêu cầu cấu trúc đầu ra bắt buộc:
1. Headline: Đề xuất 3 tiêu đề giật tít, đánh trúng pain point lớn nhất.
2. Lead (Mở bài - ~150 từ): Gợi mở vấn đề và hứa hẹn giải pháp.
3. Thân bài (Chia thành 3-4 thẻ H2, mỗi H2 có 2 thẻ H3): Mỗi phần phải giải quyết trực tiếp các Pain Points đã nêu ở dữ liệu đầu vào. Ghi rõ số từ dự kiến cho từng mục.
4. Kết bài & CTA (~100 từ): Tổng kết giá trị và kêu gọi đăng ký dùng thử.
5. Quy định giọng điệu (Tone of voice): Chuyên nghiệp, tin cậy, khách quan, hướng tới giải pháp (B2B).  
## Bước 3: Prompt 3 – Viết bài chi tiết & Tối ưu SEO
Mục đích: Triển khai nội dung đầy đủ từ dàn ý ở Bước 2. (Để tránh viết hời hợt hoặc quá dài gây đứt gãy, ta yêu cầu AI viết theo dàn ý đã chốt).

Mẫu Prompt:

"Dựa vào dàn ý chi tiết ở Bước 2, hãy viết hoàn chỉnh bài PR sản phẩm [Tên AI Chatbot] (độ dài 1000 - 1500 từ).
Ràng buộc kỹ thuật:

Giữ xuyên suốt giọng điệu chuyên nghiệp, tin cậy, khách quan của báo chí công nghệ.

Chèn tự nhiên các từ khóa SEO: AI Chatbot cho doanh nghiệp, tự động hóa CSKH, giải pháp AI.

Phân bổ rõ ràng các thẻ tiêu đề H1, H2, H3 như dàn ý.

Đoạn mở đầu (Lead) phải đánh trúng ngay nỗi đau khách hàng; đoạn kết có CTA mạnh mẽ."
## Quy tắc xử lý đứt gãy ngữ cảnh (Khi AI bị ngắt giữa chừng)
Khi bài viết quá dài (chạm giới hạn token), AI thường dừng đột ngột giữa câu. Bạn dùng câu lệnh điều khiển sau để nối tiếp mượt mà mà không bị lặp chữ hay đổi giọng văn:

Câu lệnh tiếp tục (Continuation Prompt):

"Bạn đã bị ngắt quãng ở câu: '[Dán 5-10 từ cuối cùng của đoạn bị ngắt]'.
Hãy viết tiếp tục nội dung còn lại của bài viết theo đúng dàn ý ở Bước 2.
Quy tắc bắt buộc:

Nối tiếp trực tiếp vào ngay sau cụm từ trên, KHÔNG viết lại tiêu đề hay lặp lại đoạn đã viết.

Giữ nguyên văn phong chuyên nghiệp, tin cậy như các phần trước.