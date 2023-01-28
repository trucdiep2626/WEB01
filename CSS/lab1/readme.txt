Đến với bài đầu tiên làm quen với CSS chúng ta sẽ làm quen với khái niệm Selector. Theo google dịch Selector chính là bộ chọn vậy thì mình cũng có thể tưởng tượng ra rằng với Selector chúng ta sẽ có thể chọn những thành phần mà ta muốn style cho chúng. Bắt đầu làm quen với bài lab chúng ta sẽ làm quen dần với Selector dựa trên tên tag:

Theo như bài đọc đầu tiên ta có 3 cách style cho mỗi thẻ hay phần tử mà mình muốn làm cho đẹp hơn. Vậy ta cần lưu ý cấu trúc khi style trong thẻ head và file css như sau:
    - Cấu trúc:
        [tên thẻ]{
            thuộc tính 1: giá trị 1;
            thuộc tính 2: giá trị 2;
        }
        => Khi nhìn sơ qua và nói theo ngôn ngữ người ta có thể nói như sau: nếu muốn style cho một thẻ ta chỉ cần gọi tên thẻ ra và bao quanh chúng bằng 2 dấu ngoặc nhọn, bên trong dấu ngoặc nhọn ta sẽ có 2 thành phần chính là thuộc tính và giá trị được cách nhau bởi dấu hai chấm (:) và mỗi thuộc tính khác nhau lại phân cách nhau bằng DẤU CHẤM PHẨY (;).

    - Ví dụ 1: nếu bây giờ mình style cho thẻ p với màu sắc là đỏ và kích cỡ chữ 26px thì ta sẽ viết như sau:
        p{
            color: red; // thuộc tính là màu, giá trị là màu đỏ và cách với thuộc tính thứ 2 là dấu chấm phẩy 
            font-size: 26px; // thuộc tính là kích cỡ chữ, giá trị là 26px và cách nhau với thuộc tính kế tiếp là dấu chấm phẩy
        }
    - Ví dụ 2: nếu bây giờ mình style cho thẻ h1 với màu sắc là blue và kích cỡ chữ 48px thì ta sẽ viết như sau:
        h1{
            color: blue;
            font-size: 48px;
        }

Ngược lại với style trong thẻ head và style trong file css riêng thì việc mà chúng ta style trong thẻ sẽ dựa vào thuộc tính style trong thẻ đó. Cách làm như sau
    - Ví dụ 1: nếu bây giờ mình style cho thẻ p với màu sắc là đỏ và kích cỡ chữ 26px thì ta sẽ viết như sau:
        <p style="color: red; font-size: 26px;">KIT CÓ ANH TÊN GIANG ĐẸP TRAI DẠY JAVA</p>
    => Vậy ta thấy việc style chỉ dựa trên thuộc tính style và những cấu trúc, thành phần thuộc tính bên trong đấy vẫn không thay đổi

LƯU Ý:
    Khi một dự án ngày càng được phát triển đồng nghĩa càng lớn thì chúng ta không nên viết CSS vào trong file HTML hay viết style vào thẻ như trên mà phải tách ra thành file riêng để tiện cho công việc quản lý cũng như kiểm soát

Bài tập: Từ 2 thẻ h1 và thẻ p bạn hãy tạo cho mình 1 đoạn tiêu đề và đoạn mô tả. Từ 2 đoạn ấy hãy style theo yêu cầu sau:
    Hãy liên kết file style.css vào trong index.html
    Mình có 3 ô đã được dựng sẵn bạn hãy:
        + Ô 1: hãy style cho nó bằng phương pháp inline - trong thẻ
        + Ô 2: hãy style cho nó bằng phương pháp internal - trong file html 
        + Ô 3: hãy style cho nó bằng phương pháp external - file css
    Hãy làm theo các thông số sau cho từng ô:
        h1:
            - Màu chữ là màu đỏ
            - Kích cỡ chữ là 58px
            - Hãy tìm hiểu thẻ i và lồng vào thẻ h1 để làm chữ in nghiêng. Vậy nếu làm như thế sẽ mất khá nhiều thời gian bạn hãy tìm hiểu về thuộc tính font-style và xem nó có những giá trị nào để giúp chúng ta tiết kiệm thời gian hơn:
            Câu trả lời:
                + Cách viết: 
                + Giá trị: normal:
                + Giá trị italic:
                + Giá trị oblique:
            - 
        p:
            - width sẽ bằng 80%
            - Tất cả các chữ đều được căn giữa. Bạn hãy tìm hiểu về thuộc tính text-align và xem nó có những value nào và sử dụng ra sao, ý nghĩa?
            Câu trả lời
                + Cách viết:
                + Giá trị center:
                + Giá trị justify: 
                + Giá trị end:
                + Giá trị left:
                + Giá trị right: 

TỔNG KẾT:
    Đã tìm hiểu qua được thẻ i là một thẻ in nghiêng 1 đoạn văn bản hay text.
    Thuộc tính font size để thay đổi kích cỡ chữ
    Thuộc tính ......... để thay đổi màu chữ
    ........................................