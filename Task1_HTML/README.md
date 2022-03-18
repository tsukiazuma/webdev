# Mục lục
- HTML và vai trò của HTML
- Cấu trúc HTML
- Các thẻ khai báo thông tin web cơ bản
- Các thẻ định dạng chữ viết và văn bản
- Thẻ tạo liên kết và liên kết neo
- Chèn tập tin kỹ thuật số vào web
- Tạo danh sách (List)
- Tạo form nhập liệu

## HTML và vai trò của HTML
HTML:
- Là chữ viết tắt của cụm từ HyperText Markup Language
- Là ngôn ngữ đánh dấu siêu văn bản
- Người sáng lập: Tim Berners-Lee
Vai trò: HTML giúp chia khung sườn, tạo nên bố cục của trang web, định dạng các yếu tố siêu văn bản bao gồm ảnh, video, infographic và nhiều một vài thành phần khác.

## Cấu trúc HTML
### HTML bao gồm 4 yếu tố chính:
- Thẻ khai báo loại tập tin/tài liệu.
- Thẻ đóng và mở tài liệu HTML.
- Thẻ đóng và mở phần thông tin website.
- Thẻ đóng và mở phần nội dung website.

#### Thẻ khai báo loại tập tin:
```php
<!DOCTYPE html>
<html>
</html>
```
- Trong đó, <!DOCTYPE> làm cho trình duyệt web biết được website đang sử dụng phiên bản ngôn ngữ đánh dấu (hay còn gọi markup language) nào.

#### Thẻ đóng và mở tài liệu HTML:
- Thẻ html có nhiệm vụ khai báo cho trình duyệt biết rằng những nội dung bên trong cặp thẻ này là HTML.
- Thẻ html còn có thuộc tính lang để tùy chọn mã ngôn ngữ mà website sử dụng
  
#### Thẻ đóng và mở phần thông tin website:
- Thẻ head chứa phần khai báo thông tin website như meta, title - tên website, style - khai báo CSS, script - khai báo javascript và một số thông tin khác.

#### Thẻ đóng và mở phần nội dung website:
- Thẻ body là phần thân của website, nó chứa toàn bộ nội dung của website.

## Các thẻ khai báo thông tin web cơ bản
### Thẻ title: 
- Có tác dụng khai báo tên cho trang web
- Ví dụ:
    ```php
    <meta charset="utf-8" />
    ```

### Thẻ meta
- Có điểm đặc biệt là dùng /> để đóng thẻ thay vì thẻ đóng.
- Luôn được khai báo kèm theo ít nhất là một thuộc tính và mỗi thuộc tính phải luôn có giá trị.
  - Thuộc tính charset: có nhiệm vụ khai báo cho trình duyệt biết bảng mã ký tự siêu văn bản bên trong tài liệu.
  - Thuộc tính name: luôn đi với thuộc tính content
  - Ví dụ:
    ```php
    <meta name="author" content="Ngoc Nam" />
    ```
  - Thuộc tính name hỗ trợ một số giá trị như:
    - author: Khai báo tên tác giả của tài liệu.
    - description: Khai báo mô tả của tài liệu.
    - keyword: Khai báo từ khóa của tài liệu, các từ khóa này sẽ giúp tìm kiếm văn bản hoặc máy tìm kiếm website dò tìm (Hiện tại rất ít dùng thuộc tính này).

## Các thẻ định dạng chữ viết và văn bản
### Tiêu đề và đoạn văn bản:
- Thẻ p dùng để khai báo các đoạn văn bản và mỗi đoạn sẽ cách nhau một khoảng nhất định.
- Ví dụ:
    <p>Đây là đoạn văn bản thứ 1</p>
    <p>Đây là đoạn văn bản thứ 2</p>

- Thẻ h dùng khai báo các tiêu đề và có 6 cấp độ.

### Các thẻ định dạng chữ viết:
- strong: In đậm chữ viết.
- i: In nghiêng chứ viết.
- u: Gạch chân chữ viết.
- strike: Gạch ngang chữ viết.
- em: Nhấn mạnh câu.
- code: Định dạng cho một đoạn mã nào đó.
- hr: Thước kẻ ngang trên tài liệu.
- mark: Tô sáng chữ viết.
- quote: Trích dẫn
- pre: Hiển thị ra đúng định dạng khi soạn mà không cần chỉnh sửa
- Ví dụ:
    <p>Tên:<strong>Trần Ngọc Nam</strong>, trường <i>Hutech</i>, lớp <u>18DTHD3</u>. Hiện đang là thực tập sinh của <strike>HPT Cyber Security</strike>.</p>

    <hr>

    <p>Tình trạng bản thân<code>FA</code>.</p>

    <p>Điểm trung bình hiện tại: <em>3.70</em>.</p>

    <p><mark>Câu nói thích nhất trong Naruto</mark></p>

    <p>
        <quote>
            <p>Shinra Tensei!</p>
            <title>Pain - Nagato</title>
        </quote>
    </p>

    <pre>
    Itami o kanjiru
    itami o kangaeru
    itami o uketore
    itami o shire
    itami o shiranu mono ni
    honto no heiwa wakaran
    koko yori
    Sekai ni itami o
    Shinra Tensei!
    </pre>

### Các thuộc tính style để định dạng chữ viết:
- color: màu chữ.
- background: màu nền.
- size: kích thước chữ.
- font-family: font chữ.
- text-align: căn lề chữ.

## Thẻ tạo liên kết và liên kết neo
### Thẻ liên kết - a:
- Tạo ra các đừng liên kết trong HTML.
- Các thuộc tính thường dùng:
  - href: Địa chỉ của tài liệu muốn liên kết đến.
  - title: Tiêu đề của liên kết.
  - target: Xác định nơi mở tài liệu như _blank mở trong của sổ mới, _self (giá trị mặc định) mở trong cửa sổ hiện tại, _self mở trong nội dung trang hiện tại, _parent mở trên khung trình duyệt mẹ của nó.
  - Ví dụ:
    <p>Mở trong cửa sổ mới <a href="https://www.facebook.com/ngocnam.12.01" title="Ngọc Nam" target="_blank">link facebook</a></p>
    <p>Mở trong cửa sổ hiện tại <a href="https://www.facebook.com/ngocnam.12.01" title="Ngọc Nam" target="_self">link facebook</a></p>
    <p>Mở trong nội dung trang hiện tại <a href="https://www.facebook.com/ngocnam.12.01" title="Ngọc Nam" target="_self">link facebook</a></p>
    <p>Mở trên khung trình duyệt mẹ của nó <a href="https://www.facebook.com/ngocnam.12.01" title="Ngọc Nam" target="_parent">link facebook</a></p>

### Liên kết neo
- Dẫn đến vị trí được đánh dấu trên trang web.
- Khu vực neo sẽ đánh dấu bằng id.
- thuộc tính href của thẻ a sẽ chữ # + id dùng để đánh dấu trước đó.
- Ví dụ: đoạn này copy văn bản dài quá nên em bỏ qua nhá -_-.