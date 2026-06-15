- `IP address` : Là chuỗi mã định danh như địa chỉ nhà, giúp các thiết bị nhận diện gồm IPv4(32bit, 4octet) và IPv6(128bit)
  + `IP Public` : Khi truy cập internet, số này sẽ được cấp phát theo nhà mạng
  + `IP Private` : Giúp phân biệt các thiết bị trong mạng LAN
- `MAC address` : Địa chỉ phần cứng 
- `Ping` : Độ trễ khi gửi dữ liệu
- `LAN` : Hệ thống mạng nội bộ (Ví dụ wifi nhà riêng, trường gồm nhiều học sinh -> trường là mạng LAN)
  + Star Topology : Chi phí đắt, có khả năng mở rộng kết nối tốt, hỏng khi Switch hỏng(khó)
  + Bus Topology : Chi phí rẻ, nhưng khi nhiều thiết bị hoặc gửi nhiều gói tin cùng lúc chậm, hỏng khi trục Backbone hỏng(dễ)
  + Ring Topology : Chi phí trung bình, hiệu năng ổn định, hỏng khi một máy bị tắt hoặc đoạn cáp bị đứt(dễ)
- `Switch` : Giúp kết nối các thiết bị trong cùng mạng LAN
- `Router` : Kết nối mạng LAN với internet
- `Subnet` : Mạng con, khi phân chia thành mạng con dễ quản lý, bảo trì, tối ưu hiệu năng 
- `Network address` : Địa chỉ mạng , định danh cho cả đoạn subnet
- `Host address` : Định danh cho thiết bị cụ thể
- `Cổng gateway` : Nơi dữ liệu ra hoặc vào mạng LAN đi qua
- `ARP` : Chuyển IP address -> MAC address để switch có thể truyền dữ liệu giữa các thiết bị trong cùng mạng LAN
  + `ARP cache` : Ghi nhớ việc IP addres -> MAC address để ko phải lặp lại nhiều lần
- `DHCP` : Cấp IP private cho thiết bị khi kết nối vào mạng LAN
- `Mô hình OSI` : Physical -> Data Link -> Network -> Transport -> Session -> Presentation -> Application
