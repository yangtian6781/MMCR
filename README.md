<div align="center">

# MMCR: Benchmarking Cross-Source Reasoning in Scientific Papers
<a href="https://huggingface.co/datasets/bbbeer/MMCR">🤗 HF data</a>
</div>

## News 🚀🚀🚀

- `03/25/2025`: 🔥 We have released evaluation code. The PR to [VLMEvalKit](https://github.com/open-compass/VLMEvalKit) is coming soon.
- `03/24/2025`: 🔥 We have released the MMCR [Paper](https://arxiv.org/abs/2503.16856) and [Data](https://huggingface.co/datasets/bbbeer/MMCR). We will submit a PR to [VLMEvalKit](https://github.com/open-compass/VLMEvalKit) as soon as possible, but prior to that, we will release our evaluation code.

# Quickstart
## Step 1. Installation
```bash
git clone https://github.com/yangtian6781/MMCR.git
cd MMCR
cd VLMEvalKit
pip install -e .
```
## Step 2. Evaluation
```bash
# such as InternVL2_5-1B
python run.py --data MMCR --model InternVL2_5-1B --verbose
# or
torchrun --nproc-per-node=8 run.py --data MMCR --model InternVL2_5-1B --verbose
```
# Trouble Shooting
1. If you encounter errors when testing different models, try changing to a different transformers version.
2. If you encounter network issues when downloading data from huggingface, please try using [VLMEvalKit](https://github.com/open-compass/VLMEvalKit) and we will upload the data to their servers.


## Citation

If you find this project useful in your research, please consider cite:
