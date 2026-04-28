# 📊 Telecom Customer Churn Analysis: Power BI & Machine Learning

## 📌 Tổng quan dự án
Dự án này tập trung vào việc phân tích và dự báo tỷ lệ khách hàng rời bỏ dịch vụ (Churn) tại một công ty viễn thông. Bằng cách kết hợp **Power BI** để trực quan hóa dữ liệu và **Machine Learning (Python)** để dự báo, dự án giúp xác định các yếu tố rủi ro và đưa ra các chiến lược giữ chân khách hàng hiệu quả.

---

## 🛠 Công cụ và Công nghệ
* **Business Intelligence:** Power BI (DAX, Power Query).
* **Ngôn ngữ lập trình:** Python (Google Colab).
* **Thư viện Python:** Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn.
* **Machine Learning:** Logistic Regression, Random Forest hoặc XGBoost.

---

## 📂 Cấu trúc dự án

### 1. Phân tích dữ liệu khám phá (EDA) trên Google Colab
Tôi đã sử dụng Python để thực hiện phân tích chuyên sâu nhằm hiểu rõ cấu trúc dữ liệu:
* **Xử lý dữ liệu:** Xử lý giá trị thiếu (missing values) ở cột `TotalCharges` và loại bỏ các bản ghi trùng lặp.
* **Trực quan hóa phân phối:** Sử dụng Boxplot và Histogram để phân tích sự phân bổ của `MonthlyCharges` và `Tenure`.
* **Phân tích tương quan:** Sử dụng **Heatmap** để tìm ra các biến có ảnh hưởng lớn nhất đến biến mục tiêu (Churn).
* **Feature Engineering:** Chuyển đổi các biến định tính sang định lượng (Label Encoding) và tạo nhóm `Tenure Group`.

### 2. Huấn luyện mô hình Machine Learning
Xây dựng mô hình dự báo khách hàng có khả năng rời bỏ:
* **Tiền xử lý:** Chuẩn hóa dữ liệu (Scaling) để mô hình đạt độ chính xác cao hơn.
* **Huấn luyện:** Thử nghiệm nhiều thuật toán để tìm ra mô hình tối ưu.
* **Đánh giá mô hình:** Sử dụng **Confusion Matrix**, **Accuracy**, và **F1-Score** để đo lường hiệu suất.
* **Trực quan hóa mô hình:** * **Feature Importance:** Biểu đồ hiển thị các yếu tố quan trọng nhất (như Loại hợp đồng, Internet Service) ảnh hưởng đến quyết định của khách hàng.
    * **ROC Curve:** Đánh giá khả năng phân loại của mô hình.

### 3. Dashboard trực quan trên Power BI
Dashboard được thiết kế để cung cấp cái nhìn toàn diện cho nhà quản lý:
* **Trang 1 - Overview:** Tổng quan số lượng khách hàng, tỷ lệ Churn tổng thể và theo loại hợp đồng.
* **Trang 2 - Customer Behavior:** Phân tích sâu hành vi khách hàng dựa trên các dịch vụ gia tăng như `Online Security`, `Tech Support`.
* **Slicers:** Cho phép lọc dữ liệu theo `Senior Citizen`, `Gender`, `Dependents` để xem chi tiết từng phân khúc.

<img width="1559" height="753" alt="image" src="https://github.com/user-attachments/assets/6ea79076-1c47-467b-bc9f-a75ccb9a2d12" />

<img width="1559" height="787" alt="image" src="https://github.com/user-attachments/assets/b2ca545c-28a1-4e24-b662-596ff8a6f0f0" />


---

## 🔍 Kết quả và Insight chính
* **Hợp đồng:** Khách hàng sử dụng hợp đồng ngắn hạn (Month-to-month) có tỷ lệ rời bỏ cao nhất.
* **Dịch vụ Internet:** Người dùng dịch vụ **Fiber optic** có xu hướng rời bỏ nhiều hơn so với DSL.
* **Dịch vụ gia tăng:** Những khách hàng **không** đăng ký `Online Security` hoặc `Tech Support` có nguy cơ rời bỏ cao gấp nhiều lần.
* **Mô hình dự báo:** Mô hình đạt độ chính xác (Accuracy) trên **80%**, giúp bộ phận CSKH chủ động tiếp cận nhóm khách hàng rủi ro cao.

---

## 💡 Đề xuất hành động
1.  **Chuyển đổi hợp đồng:** Cung cấp ưu đãi để khuyến khích khách hàng chuyển từ gói tháng sang gói năm.
2.  **Gói dịch vụ kèm theo:** Tặng kèm hoặc giảm giá dịch vụ `Online Security` để tăng tính gắn kết.
3.  **Cải thiện Fiber Optic:** Kiểm tra lại chất lượng dịch vụ hoặc điều chỉnh mức giá cho nhóm khách hàng sử dụng cáp quang.

---

## 📎 Tác giả
**Võ Khánh Linh**
* GitHub: [caarotnee](https://github.com/caarotnee)
