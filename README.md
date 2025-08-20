# Knee Osteoarthritis (KL & Ahlbäck Grading + JSW Regression)

Short project summary in 2–3 lines:
- Dual-output ResNet50 for KL & Ahlbäck grades from X-ray images.
- ESN-based (and/or CNN) approach for joint space width (JSW) regression.

## ✨ Highlights
- Clean training & evaluation pipeline
- Confusion matrices, classification report, accuracy, MSE out-of-the-box
- Reproducible configs (`configs/default.yaml`)
- No datasets committed; easy download script + instructions

## 🗂 Repo Layout
`notebooks/` (experiments), `src/` (library code), `scripts/` (CLI), `models/` (weights via Git LFS), `assets/` (figures), `data/` (ignored).

## ⏳ Quickstart
```bash
git clone https://github.com/<your-username>/knee-osteoarthritis.git
cd knee-osteoarthritis
python -m venv .venv && source .venv/bin/activate # (Windows: .venv\Scripts\activate)
pip install -r requirements.txt
python scripts/download_data.py   # explains where to get data
python src/train_resnet18.py --config configs/default.yaml
python src/eval.py --config configs/default.yaml
