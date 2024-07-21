# MNASNET-AND-CNN-MODELS-IN-PLANT-CLASSIFICATION

**Sơ đồ:**
Sơ đồ quá trình xây dựng bộ dữ liệu lá cây chứa đầy đủ thông tin
<img src="image/Tiền xử lý Gray.png">

Sơ đồ quá trình xây dựng bộ dữ liệu lá cây được mô tả lại
<img src="image/Tiền xử lý RGB.png">

**Thuật toán:**

**Dữ liệu sưu tầm:**

**Dữ liệu xây dựng:**

**Kết quả thực nghiệm:**

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


