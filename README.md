# espnet_model_1

语音增强（Speech Enhancement）相关项目代码。  
本仓库包含自定义增强相关脚本（`enh_model/`），并通过 **Git submodule** 引入 ESPnet（`espnet/`）。  
由于数据和音频文件体积较大，已通过 `.gitignore` 排除，不会上传到 GitHub。

---

## 目录结构

- `enh_model/`：自定义数据处理/训练/评估相关脚本（你的主要代码）
- `espnet/`：ESPnet（submodule，不直接把源码塞进仓库）
- `raw_data/`：本地原始数据（不上传）
- `aligned_data/`：本地对齐后的数据（不上传）
- `sliced_data/`：本地切分后的数据（不上传）
- `Hugging-Face/`：TODO（可选：与 Hugging Face 相关的脚本/导出等）

> 说明：`raw_data/ aligned_data/ sliced_data/ *.wav *.pth ...` 都已在 `.gitignore` 中忽略。

---

## 环境要求

- OS：Ubuntu 22.04（WSL2 也可）
- Python：建议 3.10+（或你当前 Conda 环境版本）
- 依赖：TODO（例如 numpy / scipy / soundfile / torch 等）

建议使用 Conda：

```bash
conda create -n espnet_enh python=3.10 -y
conda activate espnet_enh
pip install -r requirements.txt  # 如果你之后提供 requirements.txt
