# MAAI901_Manufacturing_Defects_Project
Unsupervised manufacturing defect detection on MVTec AD (bottle &amp; cable). Compares a frozen vs. synthetic-defect-adapted Vision Transformer (ViT-S/16) under the same patch nearest-neighbour detector, with zero-shot CLIP as a baseline. Adaptation raised cable AUROC from 0.890 to 0.938.

This project tests whether fine-tuning a pretrained Vision Transformer on synthetic CutPaste-style defects improves detection of real manufacturing defects. Using the bottle and cable categories of MVTec AD, a ViT-S/16 is evaluated frozen and partially fine-tuned, with an identical patch-level nearest-neighbour detector and thresholds set from normal images only. Zero-shot CLIP is included as a multimodal reference. Adaptation improved cable AUROC from 0.890 to 0.938 and recall from 0.61 to 0.74 without extra false alarms. Logical defects (swapped wires) remained largely undetected.

Contents: an EDA notebook, an experiment notebook (Google Colab, T4 GPU), and the saved results and figures. The dataset is not included; download MVTec AD from MVTec under its CC BY-NC-SA 4.0 licence.
