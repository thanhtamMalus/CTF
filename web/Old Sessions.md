# Old Sessions - Pico CTF 
Web Exploitation - Easy 
![Giao diện bài thi]({6E9B1957-F032-4F42-8881-2399D3B29F10}.png)
Khi vào trang web được cung cấp, mình thực hiện thử thao tác đăng kí và đăng nhập vào trang web
![alt text](image-1.png)
Sau khi vào ta có thể thấy dòng 
`Hey I found a strange page at /sessions`
-> có thể là gợi ý key
Ta chỉnh sửa đường link http://xebec.cylabacademy.net:41692/ thành http://xebec.cylabacademy.net:41692/sessions để vào
![alt text]({F87E11B9-895A-4C49-96EA-D42CC08E5E51}.png)
Ở đây ta có thể thấy các session, đây là phiên làm việc và mã dùng để phân biệt user và admin
có thể thấy dòng thứ 2 chính là cookie của user (chúng ta) 
![alt text]({F52A7753-6794-4B36-98E6-DCD7EF8C0671}.png)
Do giao thức HTTP vốn mang tính chất stateless (không lưu trạng thái — server không tự nhớ được người gửi request hiện tại là ai), Session ra đời để giúp website "nhận diện" và duy trì trạng thái của từng người dùng.
Chỉnh sửa cookie lại thành của admin
![alt text]({F1A09363-7B3E-4679-9A3E-1B3E5BC2787C}.png)
F5 để refesh trang
![alt text]({CE42CCEB-2E09-4FFA-A53A-FB1E99770CE5}.png)
Đây chính là key 
academy{s3t_s3ss10n_3xp1rat10n5_3b59378b}