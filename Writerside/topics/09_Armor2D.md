# Model Giáp (2D)
## Lưu Ý
- Để thêm được vật phẩm ta cần tệp tin hình ảnh sẽ ở định dạng ảnh `.png` 
- Với nỏ giáp 2D thì cũng sẽ có các lớp layer sau
- Với mũ 3D thì có thể thêm như item bình thường

| Đuôi File    | Thông Tin                                                                       |
|--------------|---------------------------------------------------------------------------------|
| _layer_1.png | Là lớp layer để hiển thị texture mũ và áo (Không có khi mặc sẽ không hiện giáp) | 
| _layer_2.png | Là lớp layer để hiển thị texture quần và giày (Không có khi mặc sẽ không hiện giáp)                                  | 
| icon.png     | File này là texture chính để hiện trong túi đồ và có thể đặt tên tự do          |


## Tạo Thư Mục
- Để thêm model vật phẩm ta tiến hành tạo thư mục trong `plugins/MagicPacks/items` và có thể tạo tự do
![image_31.png](image_31.png)

## Tạo Cấu Hình
- Cấu hình sẽ chứa tên model, loại vật liệu và số custom model id
- Tên vật liệu có thể tìm chính xác tại [Bukkit Material](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/Material.html)
- Lưu cấu hình thành `config.yml`, Định dạng đuôi phải là `.yml` nếu khác sẽ không hoạt động được
```yaml
CustomName: "&eGiày Wukong"
Material: diamond_boots
CustomModelID: 1
```
![image_28.png](image_28.png)
## Ném File PNG
- Khi đã tạo xong cấu hình thì ta ném ba tệp hình ảnh `.png` với bốn trạng thái lên cùng thư mục chứa `config.yml`
- Đối với tệp hình ảnh `.png` là layer thì nhớ sửa đuôi như `_layer_1.png`, `_layer_2.png`
![image_32.png](image_32.png)
- 
## Xây Dựng Gói Pack
- Khi đã ném xong thì ta vào game và chạy lệnh **/magicpack build**
- Ta có thể xem và lấy vật phẩm đó bằng lệnh **/magicpack all**
![image_33.png](image_33.png)

**LÀM TƯƠNG TỰ VỚI MŨ, ÁO, QUẦN VÀ GIÀY. NẾU THIẾU LAYER KHI MẶC TRONG TÚI ĐỒ SẼ KHÔNG HIỆN MÀ CHỈ HIỆN TEXTURE GIÁP** 