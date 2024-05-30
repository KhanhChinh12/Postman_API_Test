# Postman_API_Test

## Ngày thực hiện: 24/05/2024

## Tóm tắt

- Tổng số test: 4
- Test thành công: 2
- Test thất bại: 2
- Test bỏ qua: 0
- Chi tiết test

## Test 1: GET New Request

## URL: https://jsonplaceholder.typicode.com/users
- Phương thức: GET
- Trạng thái: Thành công
- Thời gian phản hồi: 461 ms
- Kích thước phản hồi: 6,779 KB

## Kết quả:
Thành công:
- Mã trạng thái là 200
- Tiêu đề Content-Type có mặt

## Thất bại:
Thân phản hồi không khớp với chuỗi mong muốn
Yêu cầu POST thành công không trả về mã trạng thái 200, 201 hoặc 202
Test 2

## Chi tiết hình ảnh các bước thực hiện kiểm tra API:
![1](https://github.com/KhanhChinh12/Postman_API_Test/assets/145414389/5a99eb24-1de4-463a-b48a-3e11adff0b49)
Sử dụng URL: https://jsonplaceholder.typicode.com/users để kiểm tra API

![image](https://github.com/KhanhChinh12/Postman_API_Test/assets/145414389/16492839-9d46-44b4-beb7-007dc2b50b01)
Các trường hợp kiểm tra (test) đang được cấu hình trong Postman để kiểm tra phản hồi từ API bao gồm:
1. Kiểm tra xem mã trạng thái HTTP của phản hồi có phải là 200 hay không.
2. Kiểm tra xem tiêu đề (header) "Content-Type" có tồn tại trong phản hồi hay không.
3. Kiểm tra xem nội dung (body) của phản hồi có chứa chuỗi "string_you_want_to_search" hay không.
4. Kiểm tra xem mã trạng thái HTTP của phản hồi có phải là 201 (Created) hoặc 202 (Accepted) hay không.

![image](https://github.com/KhanhChinh12/Postman_API_Test/assets/145414389/0eb75fcd-1966-46ef-8920-d47a8d701e52)
Thực hiện Run Collection với các thông số: 
1. Run manually: để chạy tập hợp một cách thủ công trong Collection Runner.
2. Iterations: Số lần lặp lại của tập hợp yêu cầu, hiện tại được đặt là 1.
3. Delay: Thời gian chờ giữa các lần chạy, đơn vị là mili giây, hiện tại được đặt là 0 ms.

![Screenshot 2024-05-24 152741](https://github.com/KhanhChinh12/Postman_API_Test/assets/145414389/147eaa0c-2b92-457c-abc7-9b5a2950b544)
Kết quả nhận được khi thực hiện kiểm tra API

## Kết luận

Hai trong số bốn test đã được thực hiện thành công. Hai test còn lại đã thất bại do thân phản hồi không khớp với chuỗi mong muốn và yêu cầu POST thành công không trả về mã trạng thái mong muốn.
