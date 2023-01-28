Sau khi đã biết style cho các thẻ các bạn sẽ nhận ra một vấn đề rằng là nếu chúng ta style cho một thẻ thì toàn bộ các thẻ còn lại sẽ cũng được style như thế làm cho chúng ta khó kiểm soát và quản lý những thẻ của mình, nếu ta muốn chỉ có một thẻ p này màu đỏ những thẻ p kia lại là màu xanh vậy thì chúng ta sẽ làm như thế nào?
Khi gặp vấn đề đấy chúng ta sẽ dụng kiến thức Selector chính là bộ chọn giữa id và class:
    - Id là gì? Bạn có thể liên hệ đến MSSV hoặc CCCD thì đó chính là id mỗi con người chúng ta đều mang một số định danh hay những thứ đặc trưng chỉ chúng ta mới có. Vậy ID sẽ đóng góp những gì trong lập trình web này? ID đóng góp một vai trò quan trọng khi các bạn làm việc với các thành phần duy nhất có thể kể đến như: thanh điều hướng - Navbar, footer, những ô feedback,... đấy là những nơi mà mỗi website sẽ có duy nhất. Hãy search cho mình xem thanh điều hướng là gì? Footer là gì? Ô feedback lấy thông tin là gì? Và kiểm chứng xem chúng là duy nhất hay có phần giống như vậy nữa?
        + Cách đặt tên trong HTML:
            <h1 id="[TÊN ID]">KIT Schedule sắp hồi sinh</h1>
            Ví dụ ở đây mình có tên id là title thì sẽ viết như sau:
            <h1 id="title">KIT Schedule sắp hồi sinh</h1>
        + Cách gọi trong file css:
            Công thức:
            #[Tên id]{
                thuộc tính 1: giá trị 1;
                thuộc tính 2: giá trị 2;
            }
            => Ta thấy cách style cũng tương tự như khi chúng ta style cho thẻ và chỉ cần thêm DẤU THĂNG (#) trước tên

    - Class là gì? Class là bạn có thể dịch nghĩa theo tiếng việt là lớp vậy hãy tưởng tượng tại Học viện Kỹ thuật mật mã có những lớp hay còn gọi là phòng học như 101 TA2 thì ta thấy rằng cách sắp xếp hay bố trí phòng học đều tương tự khi các lớp AT18G, AT18A, CT06A, CT07A, ... vào học. Vậy từ việc trên ta có thể rút ra là class là những thành phần lặp đi lặp lại và có cấu trúc giống nhau mà ta chỉ cần định nghĩa một lần và có thể sử dụng cho toàn bộ các thẻ
        + Cách đặt tên trong HTML:
            <h1 class="[TÊN CLASS]">KIT Schedule sắp hồi sinh</h1>
            Ví dụ ở đây mình có tên id là text-red thì sẽ viết như sau:
            <h1 class="text-red">KIT Schedule sắp hồi sinh</h1>
        + Cách gọi trong file css:
            Công thức:
            .[Tên id]{
                thuộc tính 1: giá trị 1;
                thuộc tính 2: giá trị 2;
            }
            => Ta thấy cách style cũng tương tự như khi chúng ta style cho thẻ và chỉ cần thêm DẤU CHẤM (.) trước tên

Bài tập:
    Từ kiến thức trên hãy tạo 2 thẻ div với:
        + Thẻ div thứ nhất: id="lab__box__id"
        + Thẻ div thứ hai: class="lab__box__class"

    Từ đó hãy style 2 thẻ div với thông số sau:
        Rộng 280px
        Dài 450px
        Bo góc thẻ div 6px
        Màu: do các bạn tự chọn cho thể tìm trên Uigradient ,hoặc schemecolor
        Màu chữ là màu trắng
    Lưu ý:
        Phần chữ, nội dung và style của bài trước vẫn giữ nguyên