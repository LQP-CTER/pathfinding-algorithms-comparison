# So sánh thuật toán A* và Dijkstra trên bản đồ thành phố

## Giới thiệu
Dự án này so sánh hiệu suất của hai thuật toán tìm đường phổ biến: **Dijkstra** và **A*** trên bản đồ thành phố Hồ Chí Minh, Việt Nam. Cả hai thuật toán được sử dụng để tìm đường đi ngắn nhất giữa hai điểm ngẫu nhiên trên bản đồ, với các thông số như khoảng cách, tốc độ tối đa và thời gian di chuyển.

## Tính năng chính
- **Trực quan hóa bản đồ**: Sử dụng thư viện `osmnx` để tải và hiển thị bản đồ thành phố Hồ Chí Minh.
- **Làm sạch dữ liệu**: Chuẩn hóa dữ liệu tốc độ tối đa và tính toán trọng số (thời gian di chuyển) cho các cạnh trên bản đồ.
- **Thuật toán Dijkstra**: Triển khai thuật toán Dijkstra để tìm đường đi ngắn nhất dựa trên trọng số.
- **Thuật toán A***: Triển khai thuật toán A* với hàm heuristic là khoảng cách Euclid giữa hai điểm.
- **Trực quan hóa quá trình tìm đường**: Hiển thị các cạnh đã thăm, đang xét và đường đi cuối cùng.
- **So sánh hiệu suất**: Chạy nhiều lần để so sánh số lần lặp và đường đi tìm được của hai thuật toán.
- **Heatmap**: Hiển thị heatmap các cạnh được sử dụng nhiều nhất bởi mỗi thuật toán.

## Yêu cầu hệ thống
- Python 3.x
- Các thư viện cần thiết:
  - `osmnx`
  - `heapq`
  - `random`

## Cài đặt
1. **Clone repository**:
   ```bash
   git clone https://github.com/your-repo/pathfinding-algorithms.git
   cd pathfinding-algorithms
   ```
2. **Cài đặt các thư viện cần thiết**:
   ```bash
   pip install osmnx heapq random
   ```

## Cách chạy
1. **Mở Jupyter Notebook**:
   ```bash
   jupyter notebook pathfinding_algorithm.ipynb
   ```
2. **Chạy từng ô lệnh**:
   - Chạy các ô lệnh trong notebook để tải bản đồ, triển khai thuật toán và trực quan hóa kết quả.

## Kết quả
- **Số lần lặp**: Thuật toán A* thường có số lần lặp ít hơn so với Dijkstra.
- **Khoảng cách và thời gian**: Cả hai thuật toán đều tìm được đường đi tối ưu, nhưng A* thường nhanh hơn nhờ sử dụng hàm heuristic.
- **Heatmap**: Heatmap cho thấy các cạnh được sử dụng nhiều nhất bởi mỗi thuật toán, giúp phân tích sự khác biệt trong cách tiếp cận của hai thuật toán.

## Lưu ý
- Đảm bảo rằng bạn có kết nối Internet để tải bản đồ từ OpenStreetMap.
- Quá trình chạy có thể mất thời gian tùy thuộc vào số lần lặp và kích thước bản đồ.

## Hỗ trợ
Nếu bạn gặp bất kỳ vấn đề nào, vui lòng liên hệ qua email hoặc tạo issue trên GitHub.

## Giấy phép
Dự án này được phân phối dưới giấy phép MIT. Xem file `LICENSE` để biết thêm chi tiết.
