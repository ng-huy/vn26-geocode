# vn26-geocode
Các bạn đều biết với hệ thống GPS hiện tại sử dụng cho toàn cầu.
Việc đánh dấu một vị trí nào đó khá dễ dàng, tuy nhiên khuyết điểm lớn nhất đó là dữ liệu tọa độ quá dài. Bỗng dưng mình không thể ghi nhớ một vị trí nào đó, hay phải chia sẻ có số quá dài đó rất cực hình.

Bỗng mình nãy ra một ý định là, VN là quốc gia không quá lớn. Sao chúng ta không vẽ một hình chữ nhật và cắt ra trên tọa độ GPS, để định vị trên đất liền
1. Lấy 4 điểm cực Đông, Tây , Nam , Bắc  để tạo hình chữ nhật sau đó chia lưới 10x10

2. Tạo ra 1 hệ tọa độ mới bên trong lưới đó và chỉ dùng ở VN
+ Lấy tọa độ 8.6069298 làm cực Nam, 23.3845395 làm cực Bắc ta có ratio 0.6766994259

+ Lấy tọa độ 109.461669 làm cực Đông và 102.1491246 làm cực Tây ta có ratio 1.367513064

3. Chọn trục cực Đông 109.461669 và đánh dấu về phía Tây lúc này ta có công thức: Điểm cực Đông - (Longitude/Hệ số: 1.367513064) kết quả làm tròn

​Chọn trục Nam 8.6069298 ta có công thức: Điểm cực Nam- (Latitude/Hệ số: 0.6766994259) kết quả làm tròn

4. Loại dấu thập phân và ghép với dấu .

Ví dụ: tọa độ GPS 10.8256985,106.6782971 cho ra VN26: 1501.3806   một con số cực kì dễ nhớ với hệ số làm tròn 3 độ sai lệch dưới 1km

​hoặc từ VN26: 1216.6583 > tọa độ gần đúng 10.40388714,104.647821 (gốc 10.40420673,104.6479163)

5. Lợi ích quá rõ ràng ở việc định vị và xác định tọa độ trong nước.


Đây là ý tưởng chưa từng có và mình mất khá nhiều công để lập nên tài liệu, hoàn thiện và chia sẻ.

Với con số 10.40420673,104.6479163 quá đáng sợ đúng không. Nhưng 1216.6583 rõ ràng rất dễ nhớ và chia sẻ

https://docs.google.com/spreadsheets/d/1nficfQglkXTz01KG5Z_Jst5nJpt_YHUn7Gd_c3OArsU/edit?usp=sharing
______________

Github: GitHub - ng-huy/vn26-geocode (https://github.com/ng-huy/vn26-geocode)

Liên hệ: Liên hệ (https://vnappscom.blogspot.com/p/lien-he.html)

HCM 11/02/2026
​




