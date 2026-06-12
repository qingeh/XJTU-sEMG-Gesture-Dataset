# XJTU sEMG Gesture Dataset

This repository provides the self-constructed surface electromyography (sEMG) dataset used in our published paper:

**Yike Zhang, Xuyang Zhang, Jiashun Zhao, Yang Zheng, and Jun Peng,
"Fourier-Wavelet convolutional network improving the accuracy of sEMG-based gesture recognition,"
Sensors and Actuators A: Physical, vol. 409, 2026, Article 118077.**

DOI: https://doi.org/10.1016/j.sna.2026.118077

## Dataset Download

The dataset is available in this GitHub repository and is managed using Git LFS:

https://github.com/qingeh/XJTU-sEMG-Gesture-Dataset.git

Users can download the dataset files directly from the repository page or clone the repository after installing Git LFS:

```bash
git lfs install
git clone https://github.com/qingeh/XJTU-sEMG-Gesture-Dataset.git
```

## Dataset Description

The dataset contains sEMG recordings collected from 10 healthy participants during hand and wrist movement tasks. The signals were recorded using a self-developed high-density sEMG acquisition system with a sampling rate of 2 kHz.

In the experiment, participants performed 7 gesture categories, including selective finger extension, full hand opening and closing, and wrist flexion and extension. Each gesture was performed in 5 repetitive trial sets, with each trial lasting 100 s. The prescribed gesture was repeated every 5 s, and a 5-minute rest period was introduced between gestures to reduce muscle fatigue.

Although the acquisition system supports 64-channel sEMG recording, the published study mainly used a reduced 4-channel configuration selected from the central region of the electrode array to balance recognition performance and computational cost.

## File Structure

The dataset is organized by subject and gesture category. Each `.txt` file stores one sEMG recording sample.

A typical organization is as follows:

```text
XJTU-sEMG-Gesture-Dataset/
├── S1/
│   ├── Gesture_A/
│   ├── Gesture_B/
│   ├── ...
│   └── Gesture_G/
├── S2/
│   ├── Gesture_A/
│   ├── Gesture_B/
│   ├── ...
│   └── Gesture_G/
└── ...
```

## Reference Paper

The dataset was used in the following paper:

> Y. Zhang, X. Zhang, J. Zhao, Y. Zheng, and J. Peng,
> "Fourier-Wavelet convolutional network improving the accuracy of sEMG-based gesture recognition,"
> *Sensors and Actuators A: Physical*, vol. 409, Article 118077, 2026.

## Citation

If you use this dataset or find it helpful for your research, please cite our paper:

```bibtex
@article{zhang2026fourier,
  title={Fourier-Wavelet convolutional network improving the accuracy of sEMG-based gesture recognition},
  author={Zhang, Yike and Zhang, Xuyang and Zhao, Jiashun and Zheng, Yang and Peng, Jun},
  journal={Sensors and Actuators A: Physical},
  volume={409},
  pages={118077},
  year={2026},
  issn={0924-4247},
  doi={10.1016/j.sna.2026.118077}
}
```

## License

This dataset is released for academic research purposes. Please cite the corresponding paper when using the dataset.
