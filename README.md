# Cats-And-Dogs (Tóm tắt phần code)

### Bước 1: Nhập các thư viện cần thiết
![image](https://github.com/ChiTrug/Cats-And-Dogs-Classification/assets/125122891/63a7bbda-e066-4aa9-88e1-8ae0f18f2da8)

 ### Bước 2: Tải bộ dữ liệu 
 Lấy dữ liệu từ trang:  https://storage.googleapis.com/kaggle-data-sets/630856/1122723/bundle/archive.zip?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=gcp-kaggle-com%40kaggle-161607.iam.gserviceaccount.com%2F20230713%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20230713T075634Z&X-Goog-Expires=259200&X-Goog-SignedHeaders=host&X-Goog-Signature=ba3c2011ea6eba9a846e9a68ded6f35070b23662a4e078e2612cb2471c8e98340c2313afe1aca14ae57ffc3519a692ed70326b8890815387cd81463d6f8eb97d96d3bf028f502ef7d872897d28fcb0931e7e5a57a1ba2c4f4cc82e15daae8dd15aa028765858f9af43f61c06ceda230a4d6e4394ecc80e709303cf7bca5c3cb2786c4b45ee7689082adbab040b17ec1c2e8e454e5730631294f7182f4f2cb648d21c54982127b9d56fb785871a16a3ab9b7105d1fbd34dd76e004aab0db4013e6647f81ede354b8c80fb68887af01840c30886cc37f6dd09b0b4c349f51a442a1d514c4903417f7725928f16b58e1d2dd7b284f3d9a15ec11f91aba257df5810 sau đó xuất file.
Bộ dữ liệu gồm 2 file Cat và Dog

### Bước 3: Chuẩn bị data
![image](https://github.com/ChiTrug/Cats-And-Dogs-Classification/assets/125122891/1003b88b-a743-48b2-b89f-8ac8d3794413)

### Bước 4:   Xây dựng mô hình
- Trong chương trình, em sử dụng một mô hình CNN đơn giản với các lớp Conv2D và MaxPooling2D để trích xuất đặc trưng của hình ảnh. Sau đó, em sử dụng các lớp Dense để thực hiện phân loại nhị phân (chó hoặc mèo).
- Với độ chính xác là 0.9830 thì model chạy khá chính xác. Loss cao và accuracy thấp trên tập kiểm tra (0.7730 và 0.8227) cho thấy mô hình có xu hướng không hoạt động tốt trên dữ liệu mới, khả năng bị overfitting.

### Bước 5: Vẽ biểu đồ độ lỗi tập test và train
![image](https://github.com/ChiTrug/Cats-And-Dogs-Classification/assets/125122891/925dae6b-2fed-405a-88a0-38a9e16e4477)

### Bước 6: Kiểm tra
Trong phần này để tránh gặp lỗi thì nên xài phiên bản tensorflow 2.12.0 mới nhất hiện tại nếu cũ hơn 2. trở về trước thì sẽ gặp lỗi. Phần này chỉ chạy code và đứa hình vào để xem model dự đoán.
