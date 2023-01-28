Sau khi các bạn đã dần làm quen với các thẻ HTML thì chúng ta sẽ tiếp đến với phần CSS. 

Vậy CSS là gì? Như đã nói ở buổi đầu tiên thì một trang web cơ bản bao gồm 3 thành phần HTML, CSS, JS và chúng ta cũng đã liên tưởng nó như một con người HTML chính là bộ khung xương, còn CSS sẽ là nơi giúp con người có da, có thịt, trang điểm đẹp hơn và làm cho chúng ta xinh đẹp rạng ngời. Vậy tóm lại CSS chính là thành phần giúp website chúng ta đẹp hơn.
Chúng ta sẽ sử dụng CSS như thế nào?
    CSS có tất cả 3 cách dùng:
        - Inline - trong thẻ muốn style. Việc sử dụng CSS ngay tại thẻ giúp chúng ta làm CSS nhanh hơn và dễ làm quen hơn:
            + Cách viết: Chúng ta có thẻ p và chúng ta sẽ viết như sau:
                <p style="color:red;"></p>
                => Các thẻ khác sẽ được viết tương tự như thế
            + Ưu điểm: viết nhanh dễ dàng
            + Nhược điểm: khó quản lý
        - Internal - viết trong thẻ head. Chúng sẽ lồng nó trong thẻ head và được viết trong cặp thẻ style:
            + Cách viết: 
                <head>
                    <style>
                        p{
                            color: red;
                        }
                    </style>
                </head>
            + Ưu điểm: có thể viết cùng file HTML 
            + Nhược điểm: tuy nhiên khó quản lý với sửa lỗi code
        - External - viết ra 1 file css riêng biệt với tên là style.css. Chúng ta sẽ tạo 1 file tên là style.css và viết ra style trong file đấy:
            + Cách viết:
                +) Đầu tiên chúng ta cần liên kết file css vào trong file HTML vì bản chất 2 file đấy là tách biệt nhau nếu không liên kết thì những thay đổi hay điều chỉnh từ file css sẽ không được cập nhật. Và file CSS được xem như phần mở rộng vậy nên chúng ta sẽ liên kết file ở thẻ head và ta sẽ sử dụng thẻ link
                <head>
                    <link rel="stylesheet" href="[TÊN FILE]" />
                </head>
                +) Ví dụ ở đây mình có file css tên là style.css thì sẽ viết đường link liên kết như sau:
                    <link rel="stylesheet" href="[TÊN FILE]" />
                +) Lưu ý:
                    Đuôi mở rộng của file css là .css 
                    Cách gõ nhanh: các bạn chỉ cần gõ chữ link sau đó sẽ thấy phần gợi ý và tìm gợi ý là link:css và chọn vào đấy và nhập tên file

Vậy sau khi đã có kiến thức căn bản về cách liên kết cũng như style css vậy bây giờ chúng ta hãy đến phần bài tập ở các lab nào        