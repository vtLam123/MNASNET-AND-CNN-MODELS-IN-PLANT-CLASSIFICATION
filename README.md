![image](https://github.com/user-attachments/assets/7269bd53-50e6-49e2-8123-7840143ca1db)# MNASNET-AND-CNN-MODELS-IN-PLANT-CLASSIFICATION

**Sơ đồ:**
Sơ đồ quá trình xây dựng bộ dữ liệu lá cây chứa đầy đủ thông tin
<img src="image/Tiền xử lý Gray.png">

Sơ đồ quá trình xây dựng bộ dữ liệu lá cây được mô tả lại
<img src="image/Tiền xử lý RGB.png">

**Thuật toán:**

**Dữ liệu sưu tầm:**

**Dữ liệu xây dựng:**

**Kết quả thực nghiệm:**

Kết quả về độ chính xác và thời gian kiểm tra trung bình trên từng mẫu cho dữ liệu đầy đủ thông tin lá cây
(với “-” sử dụng cấu trúc của mô hình gốc)

| STT | Model       | Kernel lớp đầu | Padding lớp đầu | Accuracy (%) | Latency (ms) | Epoch có độ chính xác lớn nhất khi học |
|----|-------------|-----------------|-----------------|--------------|--------------|---------------------------------------|
| 1  | VGG19       | -               | -               | 87.55        | 0.03         | 54                                    |
| 2  | ResNet152   | -               | -               | 89.03        | 0.109        | 53                                    |
| 3  | SqueezeNet  | -               | -               | 89.29        | 0.04         | 26                                    |
| 4  | MobileNetV3 | -               | -               | 93.32        | 0.047        | 13                                    |
| 5  | ShuffleNetV2| -               | -               | 93.30        | 0.044        | 19                                    |
| 6  | MNASNet_1   | 1x1             | 0x0             | 86.01        | 0.045        | 61                                    |
| 7  | MNASNet_3   | 3x3             | 1x1             | 94.88        | 0.037        | 21                                    |
| 8  | MNASNet_7   | 7x7             | 3x3             | 91.17        | 0.037        | 30                                    |


Kết quả về độ chính xác và thời gian kiểm tra trung bình trên từng mẫu cho dữ liệu mô tả hình dáng lá cây.
| STT | Model       | Kernel lớp đầu | Padding lớp đầu | Accuracy (%) | Latency (ms) | Epoch có độ chính xác lớn nhất khi học |
|----|-------------|-----------------|-----------------|--------------|--------------|---------------------------------------|
| 1  | MNASNet_1   | 1x1             | 0x0             | 78.24        | 0.032        | 30                                    |
| 2  | MNASNet_3   | 3x3             | 1x1             | 77.02        | 0.039        | 24                                    |
| 3  | MNASNet_5   | 5x5             | 2x2             | 77.16        | 0.027        | 24                                    |
| 4  | MNASNet_7   | 7x7             | 3x3             | 79.37        | 0.036        | 26                                    |
| 5  | MNASNet_9   | 9x9             | 4x4             | 77.94        | 0.034        | 27                                    |
| 6  | MNASNet_11  | 11x11           | 5x5             | 77.05        | 0.035        | 25                                    |
