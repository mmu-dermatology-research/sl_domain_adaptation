# Domain Adaptation for Skin Lesion: Evaluating Real-World Generalisation
#### Accepted at WiCV @ CVPR 2025 (Oral Presentation)

📄 Full paper Link:
https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Domain+Adaptation+for+Skin+Lesion%3A+Evaluating+Real-World+Generalisation&btnG=


### Authors: Nurjahan Sultana, Wenqi Lu, Xinqi Fan, Moi Hoon Yap

This work addresses a critical issue in medical AI: models trained on dermoscopic images often fail when tested on real-world clinical images due to domain shift.

💡 What We Did

We introduced IMPS, a diverse clinical dataset built from SD198, ISIC-Clinical, MED-NODE, and PAD-UFES-20.

We benchmarked supervised (ATDOC, LIC) and unsupervised (DANN, ADDA) domain adaptation methods.

We showed that DANN, an unsupervised method, generalises better than others—even without using target labels.

Our findings emphasise that evaluation on narrow datasets can mislead model performance claims.

📊 Evaluation

We designed a two-fold evaluation to test real-world generalisation:

Single-target evaluation: Each clinical dataset (SD198, ISIC-Clinical, MED-NODE, PAD-UFES) was tested independently.

Diverse-target evaluation: We combined them into the IMPS dataset to simulate real-world variability (e.g. device, lighting, skin tone).

📂 Dataset 

IMPS is a diverse clinical dataset created by combining:

- SD198: [DermQuest](https://github.com/xpwu95/SPBL_Pytorch?tab=readme-ov-file)
- ISIC Archive (Clinical): [https://www.isic-archive.com/](https://www.isic-archive.com/)
- MED-NODE: [https://www.kaggle.com/datasets/andrewmvd/mednode](https://www.kaggle.com/datasets/andrewmvd/mednode)
- PAD-UFES-20: [https://data.mendeley.com/datasets/wtwzydcc8y/1](https://data.mendeley.com/datasets/wtwzydcc8y/1)

It reflects real-world variability in demographics, lighting, devices, and image quality—making it suitable for robust domain adaptation evaluation.

🗂 IMPS image IDs will be published soon.

### 📚 Citation

If you use any of the concepts or code from this repository, please consider citing our paper:

```bibtex
@InProceedings{Sultana_2025_CVPR,
    author    = {Sultana, Nurjahan and Lu, Wenqi and Fan, Xinqi and Yap, Moi Hoon},
    title     = {Domain Adaptation for Skin Lesion: Evaluating Real-World Generalisation},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
    month     = {June},
    year      = {2025},
    pages     = {3433-3443}
}
```

Contact me for more detail about the IMPS dataset (nurjahan.sultana@stu.mmu.ac.uk).
