# 🍓 基于YOLO模型的轻量化深度学习草莓成熟度检测 (YOLOv8 Strawberry Ripeness Detection)

本项目基于 **YOLOv8n (Nano)** 轻量化目标检测模型，对草莓的成熟度进行 6 个阶段的分类与检测。代码在 VS Code 中编写，针对 CPU 训练环境进行了专门的防崩溃优化。

## 📁 数据集分类
模型将草莓的成熟度划分为以下 6 个阶段：
- `Early-Turning` (转色初期)
- `Green` (未成熟/青草莓)
- `Late-Turning` (转色后期)
- `Red` (完全成熟/红草莓)
- `Turning` (转色期)
- `White` (白果期)

## 🛠️ 环境配置
- 编辑器：VS Code
- 核心库：PyTorch, Ultralytics (YOLOv8), OpenCV, Matplotlib
- 安装命令：
  ```bash
  micromamba install pytorch torchvision -c pytorch -c conda-forge -y
  pip install ultralytics opencv-python matplotlib pyyaml
