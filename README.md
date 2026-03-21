# zero-shot-denoising



# Real-world video
Before denoising
## Before Denoising
https://github.com/user-attachments/assets/bbfe7f2e-0c6a-473f-a4dc-f85483e42ccf

# After denoising


# Real-world Image


![Alt text](https://github.com/asd567/zero-shot-denoising/blob/main/results/image.png)


![Alt text](https://github.com/asd567/zero-shot-denoising/blob/main/results/image2.jpg)


# Training

## Single Image Training

```python
python train.py --image_path ./image.png --noise FIM_mixed --save_dir ./checkpoints
```

## Directory Image

```python
python train.py --data_dir ./data_input --noise FIM_mixed --save_dir ./checkpoints
```

# Inference

```python
python inference.py --input_path ./image.png --model_path ./checkpoints/noist2patern_epochx.pth --output_dir ./results
```

# requirments

torch>=1.10.0

torchvision>=0.11.0

numpy>=1.20.0

opencv-python>=4.5.0

matplotlib>=3.4.0

tqdm>=4.60.0

scikit-image>=0.18.0

pytorch-msssim>=0.2.1

adabelief-pytorch>=0.2.0

