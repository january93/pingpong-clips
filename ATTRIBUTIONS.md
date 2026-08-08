# 归属说明

本项目（pingpong-clips）参考并移植了以下开源项目的代码与数据。请在使用与分发时遵守各自的许可证。

## 代码

### TTcut — MIT License
- 仓库：https://github.com/WeiyePlayer/TTcut
- 许可证：MIT（仅限 TTcut 自有源码）
- 移植内容：
  - `src/types.py` ← TTcut `worker/ttcut_worker/types.py`
  - `src/calibration.py` ← TTcut `worker/ttcut_worker/calibration.py`
  - `src/bounce.py` ← TTcut `worker/ttcut_worker/bounce.py`（弹跳检测）
  - `src/rallies.py` ← TTcut `worker/ttcut_worker/rallies.py`（回合分组）
  - `src/clips.py` ← TTcut 导出层的剪辑组规则（合并 / margin / 尾部延长 / 重叠合并）
  - `src/tracknet.py` ← TTcut `worker/ttcut_worker/model.py`（TrackNet 模型）+ `predictor.py`（推理/预处理）
  - `src/postprocess.py` ← TTcut `worker/ttcut_worker/postprocess.py`（热力图后处理 / 运动历史选球）
- TrackNet 派生代码、模型权重等保留各自版权与许可证，详见 TTcut 的
  [THIRD_PARTY_NOTICES.md](https://github.com/WeiyePlayer/TTcut/blob/main/THIRD_PARTY_NOTICES.md)

## 数据 / 权重

### OpenTTGames 数据集 / TrackNet 预训练权重 — CC BY-NC-SA 4.0（非商用）
- 来源：https://lab.osai.ai/datasets/openttgames/ ；TrackNet：https://github.com/yastrebksv/TrackNet
- 限制：**禁止商用**。本项目为个人 / 开源用途，使用前请确认你符合许可条款。
- 本项目 README 已声明禁止商用。

## 第三方运行库

Python、PyTorch、NumPy、OpenCV、FFmpeg、imageio-ffmpeg 等保留各自许可证，详见各项目声明。
