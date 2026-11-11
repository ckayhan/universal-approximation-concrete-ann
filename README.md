# Universal Approximation: Concrete ANN Depth and Width Analysis

This repository accompanies the Turkish academic study **“Evrensel Yaklaşım Teoreminin Deneysel Sınırları: Derinlik ve Genişlik Ekseninde Bir Analiz”**.

**Authors:** M. Bahattin Akgül and Celalettin Kayhan.

## Dataset
UCI Concrete Compressive Strength dataset: 1,030 samples, eight input variables and one compressive-strength target. The original `Concrete_Data.xls` is retained because the notebook reads that filename. An `.xlsx` copy is also included.

Dataset source: https://archive.ics.uci.edu/dataset/165/concrete+compressive+strength

## Run
1. Install Python 3 and Jupyter.
2. Run `pip install -r requirements.txt`.
3. Open `YSA_Concrete_Analysis.ipynb` with Jupyter.
4. Run notebook cells in order from the repository's root directory.

## Contents
- `YSA_Concrete_Analysis.ipynb`: original analysis notebook.
- `Concrete_Data.xls`, `Concrete_Data.xlsx`: data.
- `YSA_Deney_Sonuclari.xlsx`: experimental result tables.
- `YSA_Hata_Analizi.xlsx`: prediction error analysis.
- `Sekiller_300_DPI/`: figures used in the study.
- `Kaynakca.bib`: bibliographic records (check metadata against original publications before reuse).

## Reproducibility notes
The original notebook explicitly uses `random_state` seeds **42, 52, 62** in both the repeated width and repeated depth experiments. Results can still vary across software versions and environments. Figures `10_Egitim_Dogrulama_Kayip.png` and `11_Egitim_Dogrulama_RMSE.png` come from a **separate 250-epoch control experiment**, not the original early-stopping run. These should not be presented as loss curves from that original run.

This repository provides the underlying research materials; it does not independently establish that every literature reference has been verified.
