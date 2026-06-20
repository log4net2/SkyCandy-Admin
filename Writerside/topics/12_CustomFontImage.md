# Custom Font Image
- Custom Font Image dùng để thay thế một kí tự bất kì thành hình ảnh để làm icon cho scoreboard hoặc customhub sau này.
- Kí tự thường được dùng nhất là tiếng trung quốc vì khá nhiều và không ảnh hưởng đến các kí tự trong tiếng anh và tiếng việt. Có thể dùng các ngôn ngữ khác không thuộc bảng chữ cái Lating
- Để tránh member dùng kí tự đó chat thì sẽ dùng các kí tự trong [Private Use Area](https://en.wikipedia.org/wiki/Private_Use_Areas)
## Tạo Thư Mục
- Để thêm CustomFont thì ta tiến hành tạo thư mục tại `plugins/MagicPacks/fonts` 
![image_36.png](image_36.png)

## Tạo Tệp Chứa Icon
- Trước tiên tạo một file tên `icon` sẽ là nơi chứa các bức ảnh với định dạng `.png`
- Các bức ảnh có kích thước tối đa sẽ là 300x300 pixel nên hãy cắt ảnh trước khi ném vào
![image_37.png](image_37.png)
![image_38.png](image_38.png)

## Tạo Cấu Hình Icon Đã Ném Lên
- Cấu hình sẽ chứa tên hình ảnh. Nếu ảnh thêm là `icon_mine.png` thì cấu hình sẽ là `icon_mine`
- Để thay thế kí tự nào thì ta sửa `symbol: <kí tự cần thay thế>`
- Để thay đổi chiều cao của hình thì ta thêm hoặc bớt `y_position: <số dương hoặc âm>`
- Để thay đổi kích thước của hình thì ta thêm hoặc bớt `scale_ratio: <số dương hoặc âm>`
- Lưu ý là `y_position` phải lớn hơn `scale_ratio` nếu sai là toàn bộ Custom Font Image đã thêm sẽ lỗi hết

Ví Dụ:
```yaml
font_images:
  icon_mine:
    symbol: "耐"
    y_position: 9
    scale_ratio: 8
```
Có Thể Thên Nhiều Font:
```yaml
font_images:
  icon_mine:
    symbol: "耐"
    y_position: 9
    scale_ratio: 8
  a:
    symbol: "✔"
    y_position: 200
    scale_ratio: 190
  plate_coin:
    symbol: "\uE000"
    y_position: 95
    scale_ratio: 29
```
- File cấu hình `config.yml` vừa tạo sẽ nằm chung thư mục với `icon`
![image_39.png](image_39.png)

## Xây Dựng Gói Pack
- Khi đã xong thì ta vào game và chạy lệnh **/magicpack build**
- Ta có thể xem toàn bộ Custom Image Font bằng lệnh **/magicpack font**
![image_40.png](image_40.png)
![image_41.png](image_41.png)
![image_42.png](image_42.png)
![image_45.png](image_45.png)
