# Phân tích dữ liệu phòng trọ tại Việt Nam

## Giới thiệu
Dự án này thực hiện phân tích dữ liệu phòng trọ tại một số thành phố lớn ở Việt Nam như Hà Nội, Hồ Chí Minh và Đà Nẵng.  
Dữ liệu được **tự thu thập bằng phương pháp web scraping (crawl dữ liệu)** từ các website cho thuê phòng trọ.

Mục tiêu của dự án:
- Khám phá đặc điểm của thị trường cho thuê phòng trọ
- Phân tích mối quan hệ giữa các biến như diện tích, giá thuê, vị trí và tiện ích
- Trực quan hóa cấu trúc dữ liệu đa chiều bằng các kỹ thuật như correlation heatmap và t-SNE

---

## Yêu cầu môi trường

Python version: **Python 3.9+**

Các thư viện cần thiết:

```
    + pandas
    + numpy
    + matplotlib
    + seaborn
    + scikit-learn

## Cách chạy notebook: 
- B1: Mở Jupyter Notebook/ VS Code
- B2: Mở file phongtro_data_analysis.ipynb
- B3: Mở Kernel -> Run All Cells

## Nội dung phân tích trong notebook

- Thu thập dữ liệu (Web Crawling): Tự thu thập dữ liệu phòng trọ từ các website cho thuê nhà.
- Data Cleaning: 
    + Xử lý dữ liệu thiếu
    + Chuẩn hóa dữ liệu
    + Loại bỏ dữ liệu bất thường
- Data Encoding: Mã hóa các biến danh mục như thành phố và quận/huyện.
- Feature Engineering: Tạo các biến mới như
    + Log_Giá
    + Log_Diện_Tích
    + Giá_trên_m2
- Data Visualization: 
    + Histogram
    + Boxplot
    + Correlation Heatmap
    + Scatter Plot
    + t-SNE visualization



