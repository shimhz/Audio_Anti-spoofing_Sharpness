# Multi-Dataset Co-Training with Sharpness-Aware Optimization for Audio Anti-spoofing

Official Repository for the paper "Multi-Dataset Co-Training with Sharpness-Aware Optimization for Audio Anti-spoofing", published in Interspeech 2023 ([Paper](https://www.isca-speech.org/archive/pdfs/interspeech_2023/shim23c_interspeech.pdf)).

### Dependencies
```
pip install -r requirements.txt
```

### Training

1. Download ASVspoof2019 dataset 
2. Change the "database_path" in `AASIST-L_ASAM.conf` file
    (or Move data to data folder)

```
python main.py --config ./config/AASIST-L_ASAM.conf
```

### Evaluation using pre-trained model
```
python main.py --eval --config ./config/AASIST-L_ASAM.conf
```

- Performance
    - ASVspoof2019 evaluation(SAM w/o additional training datasets): EER 1.06% 


### Citation
```
@article{shim2023multidataset,
      title={Multi-Dataset Co-Training with Sharpness-Aware Optimization for Audio Anti-spoofing}, 
      author={Hye-jin Shim and Jee-weon Jung and Tomi Kinnunen},
      journal={Proc. Interspeech},
      year={2023}
}
```

### Reference
This code refers to the the following repositories:
1. https://github.com/clovaai/aasist
2. https://github.com/davda54/sam

### License
This code is licensed under MIT license