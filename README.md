# Stock Valuation Website

Ứng dụng web phân tích và định giá cổ phiếu Việt Nam sử dụng Python Flask và JavaScript.

## Tính năng

- Phân tích dữ liệu tài chính của các công ty niêm yết trên VN-Index
- Tính toán các chỉ số định giá (P/E, P/B, EV/EBITDA, etc.)
- Hiển thị biểu đồ lịch sử giá cổ phiếu
- So sánh các công ty trong cùng ngành
- Giao diện web thân thiện và dễ sử dụng

## Cài đặt

1. Clone repository:
```bash
git clone https://github.com/quanganhtapcode/val.git
cd val
```

2. Cài đặt dependencies:
```bash
pip install -r requirements.txt
```

3. Chạy ứng dụng:
```bash
python backend_server.py
```

4. Mở trình duyệt và truy cập: `http://localhost:5000`

## Cấu trúc dự án

- `backend_server.py` - Server Flask chính
- `app.js` - Logic JavaScript cho frontend
- `index.html` - Giao diện người dùng
- `style.css` - Styling CSS
- `valuation_models.py` - Các mô hình định giá
- `industry_data/` - Dữ liệu cổ phiếu theo ngành
- `requirements.txt` - Dependencies Python

## API Endpoints

- `GET /api/stock/<symbol>` - Lấy dữ liệu cổ phiếu
- `GET /api/current-price/<symbol>` - Lấy giá hiện tại
- `POST /api/valuation/<symbol>` - Tính toán định giá
- `GET /api/historical-chart-data/<symbol>` - Dữ liệu biểu đồ lịch sử

## Công nghệ sử dụng

- **Backend**: Python Flask
- **Frontend**: HTML5, CSS3, JavaScript
- **Data**: Vnstock API, VCI data
- **Charts**: Chart.js
- **Deployment**: GitHub Pages (static files)

## License

MIT License