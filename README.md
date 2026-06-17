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
- `ARP` : Chuyển IP address -> MAC address để `switch` có thể truyền dữ liệu giữa các thiết bị trong cùng mạng LAN
  + `ARP cache` : Ghi nhớ việc IP addres -> MAC address để ko phải lặp lại nhiều lần
- `DHCP` : Cấp IP private cho thiết bị khi kết nối vào mạng LAN
- `NIC` : Phần cứng giúp thiết bị kết nối mạng
- `Mô hình OSI` : Physical -> Data Link -> Network -> Transport -> Session -> Presentation -> Application
  + Layer 1 : Biến dữ liệu `<logic>` -> `vật lý`
  + Layer 2 : Đóng khung, bảo vệ dữ liệu
  + Layer 3 : Routing định tuyến tìm đường tối ưu
  + Layer 4 : Quản lý cách truyền dữ liệu
  
              TCP : Giao thức dẫn truyền an toàn, chính xác nhưng chậm

              UDP : Chuyển thẳng dữ liệu, ko quan tâm có nhận được dữ liệu ko
  + Layer 5 : Tạo, duy trì, đóng kết nối với máy khác và có `checkpoint` giúp đồng bộ dữ liệu, phục hồi khi có sự cố
  + Layer 6 : Biên dịch, mã hóa, nén dữ liệu
  + Layer 7 : Giao diện, dịch vụ người dùng  
- `Packet` < tầng 3 > : Chứa dữ liệu từ tầng trên xuống và ghi IP nguồn, đích
- `Frame` < tầng 2 > : Đóng gói packet để vận chuyển ở tầng vật lý
- `Mô hình TCP/IP` : Network interface(1 + 2) -> Internet(3) -> Transport(4) -> Application(5 + 6 + 7)
  + Mở kết nối dùng "3-way handshake" : SYN -> SYN/ACK -> ACK
  + Đóng kết nối dùng "4-way handshake" : FIN -> ACK -> FIN -> ACK 
- `Port` : Địa chị cụ thể của các ứng dụng trong cùng một thiết bị , `IP` là địa chỉ nhà (thiết bị) thì `Port` là số phòng trong nhà (ứng dụng)
- `Port Forwarding` : Show số `port` (có thể khác port hiện tại) ra internet để người khác có thể kết nối vào ứng dụng đó
- `Stateful Firewall` : Kiểm tra `packet` dựa trên lịch sử và ngữ cảnh nhờ vào `state table`
- `Stateless Firewall` : Kiểm tra độc lập từng `packet`
