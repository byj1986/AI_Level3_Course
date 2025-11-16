# AI_Level3_Course

## 项目简介
本仓库为《计算所_人工智能训练师（3级）》课程的配套素材与练习集合，包含数据集、Jupyter Notebook 示例、模型文件（如 ONNX）以及部分实验报告。适合配合课程章节进行动手实践与复现。

## 目录结构
- `计算所_人工智能训练师_3级_sucai/`：按章节归档的素材目录，包含：
  - `1.x.x-素材`、`2.x.x-素材`、`3.x.x-素材`、`4.x.x-素材`
  - 常见内容：`*.ipynb` 笔记本、`*.csv`/`*.xlsx` 数据、`*.onnx` 模型、`*.docx`/`*.txt` 报告等
- 顶层文件：
  - `README.md`：项目说明
  - 其他说明或资料文件（例如：`浦东AI考试.txt`）

部分典型示例：
- `3.2.1-素材/resnet.onnx`（图像分类示例模型）
- `3.2.2-素材/mnist.onnx`（手写数字识别示例模型）

## 环境要求
- Python 3.8 及以上
- Jupyter Notebook 或 JupyterLab
- 常用依赖（按需安装）：`numpy`、`pandas`、`scikit-learn`、`matplotlib`、`onnxruntime`

安装示例（可按需调整）：
```bash
pip install jupyter numpy pandas scikit-learn matplotlib onnxruntime
```

## 快速开始
1. 克隆仓库：
   ```bash
   git clone https://github.com/byj1986/AI_Level3_Course.git
   cd AI_Level3_Course
   ```
2. 启动 Jupyter：
   ```bash
   jupyter notebook
   ```
3. 进入 `计算所_人工智能训练师_3级_sucai/` 相应章节目录，打开对应的 `*.ipynb` 笔记本，按单元依次运行。

## 模型与大文件说明
- 仓库中包含较大的模型文件（例如 `resnet.onnx` 约 97.83MB），超过 GitHub 推荐的 50MB 上限，建议启用 Git LFS 管理：
  ```bash
  git lfs install
  git lfs track "*.onnx"
  git add .gitattributes
  git commit -m "Track ONNX models with Git LFS"
  git push
  ```

## 注意事项
- 不同操作系统可能会生成临时文件（如 `__MACOSX/`、以 `._` 开头的文件），不影响学习使用；如需精简版本，可在 `.gitignore` 中忽略这类文件。
- 课程数据与模型仅用于教学和学习目的，请勿用于未经授权的商业用途。

## 反馈与贡献
- 欢迎提出问题或建议（Issues），也可按章节补充示例与说明。

## 许可
- 若无特别声明，素材与示例仅用于教学用途。若需进一步使用，请联系仓库维护者确认。