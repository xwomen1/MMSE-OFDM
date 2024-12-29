# Mô Phỏng Kỹ Thuật Ước Lượng Kênh MMSE

Repository này chứa mã MATLAB để mô phỏng kỹ thuật ước lượng kênh **MMSE (Minimum Mean Squared Error)** trong hệ thống OFDM (Ghép Kênh Phân Chia Tần Số Trực Giao).

Mã được thực hiện bởi **Hiren Gami** và tham khảo từ tài liệu:

> J.J. Van de Beek, *"Synchronization and Channel Estimation in OFDM Systems"*, Luận án Tiến sĩ, Tháng 9 năm 1998.

---

## Tính Năng

Mô phỏng tập trung vào kỹ thuật ước lượng kênh:
- **Ước lượng MMSE**: Phương pháp tối ưu giảm thiểu sai số bình phương trung bình trong môi trường có nhiễu.

### Thành Phần Chính
- **Tham số đầu vào**:
  - Tiền tố vòng (`nCP`)
  - Kích thước FFT (`nFFT`)
  - Sơ đồ điều chế (ví dụ: QAM)
  - Dải tỷ lệ tín hiệu trên nhiễu (SNR)
- **Mô hình kênh**:
  - Kênh đa đường với các thành phần ngẫu nhiên
- **Chỉ số đầu ra**:
  - Sai số bình phương trung bình (MSE) của phương pháp MMSE

---

## Tham Số Mô Phỏng

Các tham số mặc định được sử dụng:
- Kích thước FFT: 64
- Tiền tố vòng: 8
- Điều chế: 16-QAM
- Dải SNR: từ 0 dB đến 40 dB (tăng từng bước 5 dB)
- Số vòng lặp Monte Carlo: 1500
- Độ dài kênh: 5

---

## Hướng Dẫn Sử Dụng

1. **Clone repository**:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
