# 📓 Quant Journal

Nhật ký học tập và thực hành các chiến lược giao dịch định lượng.

---

## 🗓️ 2025-04-14 — Bollinger Bands Backtest

**🎯 Mục tiêu:**  
Tạo một chiến lược mean-reversion đơn giản sử dụng Bollinger Bands và backtest hiệu suất trên SPY từ 2020 đến 2024.

**📌 Học được hôm nay:**
- Cách sử dụng `yfinance` để tải dữ liệu lịch sử
- Tính toán Bollinger Bands: MA20 ± 2 * STD20
- Logic vào lệnh:  
  - Mua khi `Close < Lower Band`  
  - Giữ đến khi `Close > Upper Band`
- Dùng Pandas để tạo tín hiệu (`position`) và tính toán lợi nhuận
- Plot biểu đồ so sánh hiệu suất chiến lược với chiến lược mua & giữ

**📈 Kết quả:**
- Sharpe Ratio: **0.80**
- Số lệnh mua: **32**
- Cumulative Return (Strategy): **XX.XX%**
- Cumulative Return (Buy & Hold): **YY.YY%**

**🤔 Cần hiểu thêm:**
- Khi nào Sharpe Ratio > 1 là "tốt"?  
- Tại sao đôi khi chiến lược hoạt động kém hơn thị trường?  
- Nếu thêm điều kiện RSI hoặc Volume thì có cải thiện không?

---

## ⏭️ Ngày mai định làm gì:
- Viết chiến lược mean-reversion với chỉ báo RSI
- So sánh hiệu suất với Bollinger Strategy

---
