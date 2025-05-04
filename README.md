<style>
  .art-name-container {
    perspective: 500px;
    margin-bottom: 30px;
  }
  .art-name {
    font-family: 'Brush Script MT', cursive;
    font-size: 4rem;
    background: linear-gradient(45deg, #ff3366, #33ccff, #ffcc33, #33ff66);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    text-shadow: 0 0 10px rgba(255,255,255,0.8);
    animation: float 3s ease-in-out infinite, colorChange 8s linear infinite;
    transform-style: preserve-3d;
    display: inline-block;
    padding: 15px 30px;
    border-radius: 20px;
    box-shadow: 0 10px 20px rgba(0,0,0,0.2);
    position: relative;
    overflow: hidden;
  }
  .art-name::before {
    content: "";
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: linear-gradient(
      to bottom right,
      rgba(255,255,255,0.2),
      rgba(255,255,255,0)
    );
    transform: rotate(30deg);
    animation: shine 3s ease-in-out infinite;
  }
  @keyframes float {
    0%, 100% {
      transform: translateY(0) rotateY(0);
    }
    50% {
      transform: translateY(-10px) rotateY(10deg);
    }
  }
  @keyframes colorChange {
    0% { filter: hue-rotate(0deg); }
    100% { filter: hue-rotate(360deg); }
  }
  @keyframes shine {
    0% { left: -50%; }
    100% { left: 150%; }
  }
  .decoration {
    position: absolute;
    width: 20px;
    height: 20px;
    background: #ff3366;
    border-radius: 50%;
    animation: float 2s ease-in-out infinite;
    opacity: 0.7;
  }
  .decoration:nth-child(1) {
    top: 10px;
    left: 20px;
    animation-delay: 0s;
  }
  .decoration:nth-child(2) {
    bottom: 10px;
    right: 20px;
    animation-delay: 0.5s;
  }
</style>

<div align="center">
  <div class="art-name-container">
    <div class="art-name">AnDaoAi</div>
    <div class="decoration"></div>
    <div class="decoration"></div>
  </div>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/andaoai/andaoai/output/github-contribution-grid-snake-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/andaoai/andaoai/output/github-contribution-grid-snake.svg">
    <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/andaoai/andaoai/output/github-contribution-grid-snake.svg">
  </picture>
</div>

## 🛠️ 技术栈

### 主要编程语言
- 🐍 **Python**: NumPy, PyTorch, TensorFlow
- 📜 **TypeScript/JavaScript**: Node.js, React
- 🦫 **Golang**: Gin, GORM
- ➕ **C++**: STL, OpenCV

### 开发工具
- 🛠️ VS Code, PyCharm
- 🐳 Docker, Kubernetes
- 🔄 Git, GitHub Actions

---

## 📋 模型学习记录


| 模型名称 | 描述 | 实践验证记录 |
|---------|-----|------------|
| [🎯 SAM (Segment Anything Model)](https://github.com/facebookresearch/segment-anything) | <br>🔍 Meta AI开发的通用图像分割模型<br>✨ 支持零样本分割<br><br> | <br>🔗 [SAM转ONNX脚本](https://www.kaggle.com/code/andaoai/sam2onnx)<br>✅ 2023.05完成本地部署和测试<br>💡 成功实现自动分割<br>🚀 [TS部署脚本](https://github.com/andaoai/yolo-label-vs/blob/ai/src/test/sam-inference.test.ts)<br><br> |
| [⚡ FastSAM](https://github.com/CASIA-IVA-Lab/FastSAM) | 🚀 SAM的快速实现版本<br>⚡ 使用CNN架构提升速度 | 🔗 [Kaggle实现](https://www.kaggle.com/code/andaoai/fastsam)<br>🔗 [模型下载](https://www.kaggle.com/models/andaoai/fastsam)<br>✅ 基础功能跑通<br>⚠️ 未集成CLIP文本输入 |
| [🎯 YOLOv2](https://github.com/pjreddie/darknet) | 🖼️ 目标检测模型第二版<br>⚡ Darknet框架 | 🔗 [YOLOv2 Kaggle实现](https://www.kaggle.com/code/andaoai/yolo2)<br>✅ 亲手实现基础版本 |
| [🎯 YOLOv5](https://github.com/ultralytics/yolov5) | 🖼️ 实时目标检测模型<br>⚡ 单阶段检测器 | 🔗 [DeepSORT+YOLOv5 Demo](https://github.com/andaoai/DeepSORT_YOLOv5_Pytorch)<br>✅ 熟练掌握各种训练<br>🚀 实现DeepSORT目标跟踪<br>🛠️ [自主开发标签工具](https://github.com/andaoai/yolo-label-vs)<br>📊 最高准确率85% |
| [🎯 ResUNet](https://github.com/facebookarchive/fb.resnet.torch) | 🏗️ 使用TensorFlow 2搭建<br>🧠 图像分割模型 | 🔗 [ResUNet实现脚本](https://www.kaggle.com/code/andaoai/resunet-cocmap-learning)<br>✅ 亲手搭建并训练<br>📈 在自定义数据集上验证 |
| [🎯 ResNet18](https://github.com/pytorch/vision/blob/main/torchvision/models/resnet.py) | 🏗️ 经典图像分类模型<br>🧠 18层深度 | 🔗 [ResNet18分类实现](https://www.kaggle.com/code/andaoai/two-classifications-of-star-map)<br>✅ 熟练训练各类数据集<br>📊 在星图分类任务中验证 |
| [🎯 VAE](https://github.com/keras-team/keras/blob/master/keras/layers/__init__.py) | 🌀 变分自编码器<br>🧠 生成模型研究 | 🔗 [VAE实现](https://www.kaggle.com/code/andaoai/variantional-autoencoders-vae)<br>✅ 完成基础研究学习 |
| [🚀 Streaming-DRL](https://github.com/mohmdelsayed/streaming-drl) | <br>🔥 创新优化函数的强化学习算法<br>✨ 重点关注优化函数创新<br><br> | <br>🔗 [Demo实现](https://www.kaggle.com/code/andaoai/stream-q-atari)<br>✅ 已跑通Demo实现<br>📊 研究优化函数创新<br><br> |
| [🎯 SimCLR](https://github.com/google-research/simclr) | <br>🌀 对比学习框架<br>✨ 自监督视觉表示学习<br><br> | <br>🔗 [亲手搭建实现](https://www.kaggle.com/code/andaoai/simclr)<br>🔗 [TorchLight快速搭建](https://www.kaggle.com/code/andaoai/simclr-test)<br>✅ 两种方式均已跑通<br>💡 支持自定义数据训练<br><br> |
| [🔜 CLIP](https://github.com/openai/CLIP) | 🖼️ 多模态视觉语言模型 | 🔗 [待实现]<br>⏳ 计划学习模型调用方法 |
| [🔜 SAM2](https://github.com/facebookresearch/segment-anything) | 🔍 SAM升级版本 | 🔗 [待实现]<br>⏳ 跟踪最新版本特性 |
| <br>🔜 [待添加]<br><br> | <br>[待描述]<br><br> | <br>🔗 [待实现]<br>⏳ 计划学习领域<br><br> |

