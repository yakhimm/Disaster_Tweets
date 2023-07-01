# **Natural Language Processing with Disaster Tweets**

Predict which Tweets are about real disaters and which ones are not 

Thông tin cuộc thi: https://www.kaggle.com/competitions/nlp-getting-started/overview 			

## I. THÔNG TIN THÀNH VIÊN 
### 1. Giới thiệu thành viên

|**STT**|**MSSV**|**Họ và tên**|**Email**|
|---|-----------------------|--------|---------------------|
|01|20120328|Hoàng Đức Nhật Minh|20120328@student.hcmus.edu.vn|
|02|20120224|Trần Thị Mỹ Trinh|20120224@student.hcmus.edu.vn|
|03|20120210|Trần Thị Kim Tiến|20120210@student.hcmus.edu.vn|
|04|20120307|Phạm Gia Khiêm|20120307@student.hcmus.edu.vn|
|05|20120231|Phan Huy Trường|20120231@student.hcmus.edu.vn|
|06|20120578|Phạm Quốc Thái|20120578@student.hcmus.edu.vn|

Github: https://github.com/yakhimm/Disaster_Tweets		

### 2. Phân chia công việc

|**Nội dung công việc**|**Thành viên thực hiện**| 
|:----:|:----:|
| Khám phá dữ liệu (EDA) | Trinh | 
| Tiền xử lý dữ liệu | Thái, Trường |
| Xây dựng mô hình | Minh, Khiêm, Tiến |
| Phân tích và đánh giá kết quả | Minh, Khiêm, Tiến |
| Cải thiện độ chính xác | Minh, Khiêm |
| Tìm hiểu lý thuyết của mô hình | Tiến, Trường |
| Quay video | Cả nhóm |

### 3. Video thuyết trình 
https://drive.google.com/file/d/1P-iorRwk_3gTU3eBUQAGBCdA1SJfQzDQ/view?usp=sharing

## II. GIỚI THIỆU CHUNG VỀ ĐỒ ÁN
Với yêu cầu của [cuộc thi Kaggle](https://www.kaggle.com/competitions/nlp-getting-started/overview) là phân loại Tweet, dựa trên dữ liệu đầu vào là 1 bài Tweet có nội dung là một đoạn văn bản thuần, cần tiến hành phân loại thành hai nhóm 0 - Không có thảm họa và 1 - Có thảm họa. Dựa theo yêu cầu và bộ dữ liệu được cung cấp, nhóm đã tiến hành khám phá, tiền xử lý dữ liệu, xây dựng, huấn luyện mô hình thích hợp để hoàn thành yêu cầu phân loại Tweet của đề bài.

## III. MÔ HÌNH SỬ DỤNG VÀ KẾT QUẢ CỦA NHÓM
### 1. Mô hình sử dụng:
Nhóm sử dụng mô hình BERT.
- BERT là viết tắt của từ Bidirectional Encoder Representation from Transformer nghĩa là mô hình biểu diễn từ theo 2 chiều ứng dụng kỹ thuật Transformer.
- Được train trên Wikipedia (~2.5B words) và Google’s BooksCorpus (~800M words)
- Mô hình BERT nhóm sử dụng: bert-base-uncased với 110 triệu tham số. Với base tương ứng với 12 encoder transformer layer, và uncased phù hợp sử dụng cho các ngôn ngữ không dấu, như tiếng anh. 
### 2. Kết quả:
Nhóm đạt được rank 112, sau khi trừ các 34 hack account có độ chính xác là 100%, thì nhóm đạt rank 78, thuộc top 7.8%
![image](https://github.com/yakhimm/Disaster_Tweets/assets/76483242/efcf4da7-c0e5-4bbe-889c-7a78ec4693d6)