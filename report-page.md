# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Tóm tắt ngắn gọn mục tiêu của bài lab.
Mục tiêu của bài lab là hiểu và cài đặt cách tính entropy để đo mức độ ngẫu nhiên của dữ liệu, từ đó tính redundancy để đánh giá phần dư thừa thông tin. Ngoài ra, bài lab giúp áp dụng thuật toán Euclid mở rộng để tìm nghịch đảo modulo và kiểm thử chương trình với nhiều trường hợp khác nhau.

---
## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy dựa trên công thức log2(N) - H.
- Hoàn thiện hàm mod_inverse() bằng thuật toán Euclid mở rộng.
- Chạy thử trên nhiều test case khác nhau (bao gồm cả trường hợp lỗi).

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0 |  | 8 | Chuỗi lặp hoàn toàn → entropy thấp, dư thừa cao |
| abcd | 2 |  | 6 | Chuỗi đa dạng → entropy cao hơn |
| hello world | 2.85 |  | 5.15 | Chuỗi có lặp và không lặp → entropy trung bình |


### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | Không tồn tại |

## 4. Kết luận
Nêu ngắn gọn em học được gì từ bài lab, khó khăn lớn nhất là gì, và điều gì giúp em hiểu rõ hơn về entropy hoặc modulo inverse.
Qua bài lab, em hiểu rõ hơn về cách tính entropy và ý nghĩa của nó trong việc đo độ ngẫu nhiên của dữ liệu. Em cũng nắm được cách tính redundancy để đánh giá lượng thông tin dư thừa. Ngoài ra, em học được cách sử dụng thuật toán Euclid mở rộng để tìm nghịch đảo modulo. Khó khăn lớn nhất là hiểu công thức và xử lý trường hợp không tồn tại nghịch đảo, nhưng việc thực hành và test nhiều trường hợp đã giúp em hiểu rõ hơn.
