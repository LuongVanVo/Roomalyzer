# Phân tích dữ liệu và các yếu tố tác động đến giá nhà trọ

## 1. Giới thiệu
Tiểu dự án tập trung vào bài toán phân tích giá thuê phòng trọ tại các thành phố lớn như Hà Nội, TP.HCM và Đà Nẵng.

Dữ liệu được thu thập bằng phương pháp web scraping, sau đó làm sạch và phân tích để trả lời các câu hỏi:
- Giá thuê chịu ảnh hưởng như thế nào bởi diện tích và vị trí?
- Chênh lệch giá giữa các khu vực ra sao?
- Những đặc trưng nào liên quan mạnh nhất tới giá thuê?

## 2. Mục tiêu
- Xây dựng bộ dữ liệu phòng trọ có thể tái sử dụng cho phân tích.
- Làm sạch dữ liệu và chuẩn hóa các biến quan trọng.
- Trực quan hóa và đánh giá các yếu tố tác động đến giá nhà trọ.
- Tạo pipeline cơ bản: crawl -> clean -> analyze.

## 3. Yêu cầu môi trường
- Python: 3.9+
- Khuyến nghị dùng môi trường ảo (`venv` hoặc `conda`).

Thư viện chính:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- beautifulsoup4
- cloudscraper

## 4. Cấu trúc chính trong thư mục này
- `data_crawl.ipynb`: Notebook thu thập dữ liệu phòng trọ thô.
- `data_analysis.ipynb`: Notebook phân tích, trực quan hóa, rút ra insight.
- `data/raw/raw_data.csv`: Dữ liệu thô sau crawl.
- `data/clean/clean_data.csv`: Dữ liệu đã xử lý phục vụ phân tích.

## 5. Cách chạy
1. Mở thư mục dự án bằng VS Code hoặc Jupyter Notebook.
2. Cài thư viện cần thiết.
3. Chạy notebook theo thứ tự:
     1. `data_crawl.ipynb` (nếu cần thu thập mới)
     2. `data_analysis.ipynb`
4. Chọn đúng kernel Python và dùng `Run All Cells`.

## 6. Nội dung phân tích
- Thu thập dữ liệu (Web Crawling): lấy dữ liệu phòng trọ từ các trang đăng tin.
- Data Cleaning:
    - Xử lý giá trị thiếu.
    - Chuẩn hóa định dạng giá và diện tích.
    - Loại bỏ trùng lặp và dữ liệu bất thường.
- Data Encoding: mã hóa các biến danh mục như thành phố, quận/huyện.
- Feature Engineering:
    - `Log_Gia`
    - `Log_Dien_Tich`
    - `Gia_tren_m2`
- Data Visualization:
    - Histogram
    - Boxplot
    - Correlation Heatmap
    - Scatter Plot
    - t-SNE
