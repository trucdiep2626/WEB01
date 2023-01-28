Tiếp tục với CSS Selector lần này chúng ta sẽ tìm hiểu thêm 1 phần gọi là CSS Combinators. Phần này giúp chúng ta có thể style cho các thành phần con của thẻ div. Vậy tại sao cần làm như thế? Khi chúng ta chọn phần tử con của một thẻ div chúng ta sẽ kiểm soát chúng hơn, và đôi khi mỗi phần tử con đấy lại cần mang một giá trị riêng biệt.

Ta có 4 loại CSS Combinators:
    + Sử dụng space - khoảng trắng
    + Sử dụng > - dấu lớn hơn
    + Sử dụng + - dấu cộng
    + Sử dụng ~ - dấu ngã

Trong phần này mình chỉ giải thích space và 3 phần còn lại các bạn tìm hiểu tại: https://www.w3schools.com/css/css_combinators.asp

Như các bạn đã biết khi muốn CSS ta cần gọi 1 class hoặc id để có thể style cho phần tử đấy như vậy ta sẽ tốn khá nhiều thời gian để đặt tên class và id có ý nghĩa cho 1 thẻ. Khi mà website chúng ta ngày càng phát triển thì phần tử hay thẻ ngày càng nhiều chúng ta không thể đặt hết tên cho chúng được vậy thì đã có hướng giải quyết khác đó chính là gọi đến phần tử con của một class.
    Cách gọi: 
        .[tên class] [tên thẻ]{
            thuộc tính 1: giá trị 1;
            thuộc tính 2: giá trị 2;
        }

    Ví dụ:
    file HTML:
        <div class="lab__box>
            <img src="[ĐƯỜNG DẪN CỦA ẢNH]" alt="[MIÊU TẢ CỦA ẢNH]">
            <h1>[Tiêu đề]</h1>
        </div>

    Vậy như chúng ta thấy hiện tại thẻ div có class tên là lab__box và nó chưa 2 phần tử con là thẻ img và thẻ h1. Nếu sử dùng kiến thức của 2 lab trước chúng ta cần phải đặt class cho 2 thẻ đấy và thế thì sẽ tốn khá nhiều thời gian nên bây giờ hãy áp dụng công thức ở trên xem nào:
        .lab__box img{
            width: 100%
            height: 100%;
        }

        .lab__box h1{
            color: red;
            font-size: 56px;
        }

    Sau khi áp dụng bạn sẽ thấy rằng ảnh của mình nó đang bị bể và bóp lại vậy chúng ta nên làm thế nào?

Bài tập:
    Hãy thêm 3 hình ảnh về nhân vật mà bạn yêu thích và từ những thuộc tính ở trên hãy làm 1 thẻ nhân vật bạn yêu thích
    Hãy tìm hiểu thuộc tính object-fit cách sử dụng và xem nó có những giá trị nào?
        + Cách sử dụng:
        + Giá trị contain:
        +
    Hãy xem lại ảnh final và ta thấy rằng 2 phần trên trái và và phải của ảnh đang được bo tròn lại bạn hãy làm cho nó bo tròn như vậy. Lưu ý: nếu sử dụng border-radius sẽ bo tròn ra 4 góc hãy nêu giải pháp của bạn?
        + Bo góc bên trái trên:
        + Bo góc bên phải trên:
    Và mỗi phần giới thiệu tên nhân vật cần viết hoa bạn hãy sử dụng thuộc tính của CSS để có thể làm thẻ h1 viết hoa (keyword: uppercase) bằng CSS Combinators mà không phải viết hoa tiêu đề ở file HTML