# TvBox n8n

1. Cách thức triển khai như nào?
    1. Mua TVBox:
        1. Có sẵn hệ điều hành: Các bạn google tvbox armbian. Có 1 shop bán nhưng đang tạm hết hàng. Link : https://s.shopee.vn/5ptNWhvxSf
        2. Mua TVBox bình thường về, ví dụ Tx3 Mini Wifi sau đó cài Armbian. Cách cài: [https://armbian.io.vn/cach-cai-dat-armbian-tren-android-box/](https://armbian.io.vn/cach-cai-dat-armbian-tren-android-box/)
        3. Có 1 lưu ý là ko phải all TVBOX đều được, phải là ARM chip nằm trong list: [https://github.com/ophub/amlogic-s9xxx-armbian?tab=readme-ov-file&ref=armbian.io.vn#armbian-system-description](https://github.com/ophub/amlogic-s9xxx-armbian?tab=readme-ov-file&ref=armbian.io.vn#armbian-system-description)
        4. Mình mua bản cài sẵn Armbina
    2. Cắm vào màn hình qua HDMI, cắm thêm chuột phím và boot lên.
    3. Kêt nối wifi:
    
    ```python
    nmcli device wifi list
    nmcli device wifi connect "$SSID" password "$PASSWORD"
    ```
    
    d. Cài đặt SSH Server
    
    | sudo apt update |  |  |
    | --- | --- | --- |
    | sudo apt install openssh-server |  |  |
    | sudo systemctl status ssh |  |  |
    | sudo service ssh start |  |  |
    | ip a | view IP |  |
    
    e. Cài đặt:
    
    | n8n | curl -L https://bit.ly/n8n_install_noai_debian | sh |
    | --- | --- |
    | Bật Ngrok  | sh <(curl -L https://bit.ly/n8n_with_ngrok_pi) |
    |  |  |
2. Link mua TVBox:
- Có sẵn armbian: [https://s.shopee.vn/8zqLjoKSQh](https://s.shopee.vn/8zqLjoKSQh)
- Có sẵn armbian: [https://s.shopee.vn/5Kx3OENPc5](https://s.shopee.vn/5Kx3OENPc5)
- Chưa cài - Tx3 Mini 2G: [https://s.shopee.vn/5VGSGiLjc9](https://s.shopee.vn/5VGSGiLjc9)
- Chưa cài- H96Max 4G: [https://s.shopee.vn/3VVPBo00AK](https://s.shopee.vn/3VVPBo00AK)
- Chỉ là link tham khảo. Check kỹ danh sách tương thích bên trên.
