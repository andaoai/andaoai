<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/andaoai/andaoai/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/andaoai/andaoai/output/github-contribution-grid-snake.svg">
  <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/andaoai/andaoai/output/github-contribution-grid-snake.svg">
</picture>

# 📚 学习过的模型记录

## 👁️ 视觉模型
| 模型名称                 | 实现跑通地址            | 描述                          | Git地址                                      | 实践验证记录              |
|-------------------------|-----------------------|-----------------------------|--------------------------------------------|-------------------------|
| 🎯 SAM (Segment Anything Model) | [SAM转ONNX脚本](https://www.kaggle.com/code/andaoai/sam2onnx) | 🔍 Meta AI开发的通用图像分割模型<br>✨ 支持零样本分割 | [GitHub](https://github.com/facebookresearch/segment-anything) | ✅ 2023.05完成本地部署和测试<br>💡 成功实现自动分割<br>🚀 [TS部署脚本](https://github.com/andaoai/yolo-label-vs/blob/ai/src/test/sam-inference.test.ts) |
| ⚡ FastSAM               | [Kaggle实现](https://www.kaggle.com/code/andaoai/fastsam)<br>[模型下载](https://www.kaggle.com/models/andaoai/fastsam) | 🚀 SAM的快速实现版本<br>⚡ 使用CNN架构提升速度 | [GitHub](https://github.com/CASIA-IVA-Lab/FastSAM) | ✅ 基础功能跑通<br>⚠️ 未集成CLIP文本输入 |
| 🎯 YOLOv2                | [YOLOv2 Kaggle实现](https://www.kaggle.com/code/andaoai/yolo2) | 🖼️ 目标检测模型第二版<br>⚡ Darknet框架 | [GitHub](https://github.com/pjreddie/darknet) | ✅ 亲手实现基础版本 |
| 🎯 YOLOv5                | [DeepSORT+YOLOv5 Demo](https://github.com/andaoai/DeepSORT_YOLOv5_Pytorch) | 🖼️ 实时目标检测模型<br>⚡ 单阶段检测器 | [GitHub](https://github.com/ultralytics/yolov5) | ✅ 熟练掌握各种训练<br>🚀 实现DeepSORT目标跟踪<br>🛠️ [自主开发标签工具](https://github.com/andaoai/yolo-label-vs)<br>📊 最高准确率85% |
| 🎯 ResUNet               | [ResUNet实现脚本](https://www.kaggle.com/code/andaoai/resunet-cocmap-learning) | 🏗️ 使用TensorFlow 2搭建<br>🧠 图像分割模型 | [GitHub](https://github.com/facebookarchive/fb.resnet.torch) | ✅ 亲手搭建并训练<br>📈 在自定义数据集上验证 |
| 🎯 ResNet18              | [ResNet18分类实现](https://www.kaggle.com/code/andaoai/two-classifications-of-star-map) | 🏗️ 经典图像分类模型<br>🧠 18层深度 | [GitHub](https://github.com/pytorch/vision/blob/main/torchvision/models/resnet.py) | ✅ 熟练训练各类数据集<br>📊 在星图分类任务中验证 |
| 🔜 CLIP                  | [待实现] | 🖼️ 多模态视觉语言模型 | [GitHub](https://github.com/openai/CLIP) | ⏳ 计划学习模型调用方法 |
| 🔜 SAM2                  | [待实现] | 🔍 SAM升级版本 | [GitHub](https://github.com/facebookresearch/segment-anything) | ⏳ 跟踪最新版本特性 |
| 🎯 VAE                   | [VAE实现](https://www.kaggle.com/code/andaoai/variantional-autoencoders-vae) | 🌀 变分自编码器<br>🧠 生成模型研究 | [GitHub](https://github.com/keras-team/keras/blob/master/keras/layers/__init__.py) | ✅ 完成基础研究学习 |

## 🎮 深度强化学习
| 模型名称                 | 实现跑通地址            | 描述                          | Git地址                                      | 实践验证记录              |
|-------------------------|-----------------------|-----------------------------|--------------------------------------------|-------------------------|
| 🚀 Streaming-DRL        | [Demo实现](https://www.kaggle.com/code/andaoai/stream-q-atari) | 🔥 创新优化函数的强化学习算法<br>✨ 重点关注优化函数创新 | [GitHub](https://github.com/mohmdelsayed/streaming-drl) | ✅ 已跑通Demo实现<br>📊 研究优化函数创新 |

## 💬 NLP领域
| 模型名称                 | 实现跑通地址            | 描述                          | Git地址                                      | 实践验证记录              |
|-------------------------|-----------------------|-----------------------------|--------------------------------------------|-------------------------|
| 🔜 [待添加]             | [待实现] | [待描述] | [待补充] | ⏳ 计划学习领域 |

---

### 📝 表格说明：
1. **实现跑通地址**：填写本地路径或云端地址
2. **Git地址**：点击可直接访问仓库
3. **跑通记录**：使用emoji标记关键信息
4. 表格支持Markdown语法，可根据需要调整格式

### 🎨 美化特点：
- 使用emoji增强可读性
- 重要信息分行显示
- 添加超链接方便访问
- 统一的对齐方式
