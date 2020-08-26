# Guided Dual Networks For Single Image Super-Resolution
This repository is for GDSR, and our presentation slide can be download [here](https://pan.baidu.com/s/1xT9nc6kcLpD9J7ITnDhdGA)   (access code:ipf7)<br/>
the results of GDSR can be download [here](https://pan.baidu.com/s/1L_M2Qryd-mfr7N2z3X5PPg) (access code:l2y0)<br/>
The pretrained model can be downoad [here](https://pan.baidu.com/s/1eFON-E2sePAUGjnGDE5jTA)(access code:7noo）<br/>

The code is built on [BasicSR (PyTorch)](https://github.com/xinntao/BasicSR) and tested on Ubuntu 18.04/16.04 environment (Python3.6, PyTorch_1.0.1, CUDA9.0, cuDNN7.4) with Nividia RTX 2080Ti/GTX 1080Ti GPUs.
# Contents
[Introduction](#Introduction)
[codes](#codes)
[results](#results)

# Introduction
The PSNR-oriented super-resolution (SR) methods pursue high reconstruction accuracy, but tend to produce over-smoothed results and lose plenty of high-frequency details. The GAN-based SR methods aim to generate more photo-realistic images, but the hallucinated details are often accompanied with unsatisfying artifacts and noises. To address these problems, we propose a guided dual super-resolution network \relax(GDSR), which exploits the advantages of both the PSNR-oriented and the GAN-based methods to achieve a good trade-off between reconstruction accuracy and perceptual quality. Specifically, our network contains two branches to simultaneously generate SR images with high accuracy and satisfactory visual quality, where one branch is trained to extract global information and the other to focus on detail information. To obtain more high-frequency features, we use the global features extracted from the low-frequency branch to guide the training the high-frequency branch. Besides, our method utilizes a mask generator to adaptively recover the final super-resolved image. Extensive experiments on several standard benchmarks show that our proposed method achieves comparative performance with state-of-the-art methods.

![Network Architecture](https://github.com/wenchen4321/GDSR/tree/master/imgs/network1.png)
# codes

# results
## Quantitative Comparisons
![RMSE_PI figure](/imgs/RMSE_PI.png)

## Qualitative Results
![visual result1](/imgs/visual_result1.png)  
![visual result2](/imgs/visual_result2.png)  
![visual result3](/imgs/visual_result3.png)  

## Acknowledgement
Our work and implementations are inspired by following project:<br/>
[BasicSR] (https://github.com/xinntao/BasicSR)<br/>

If you find our work useful in your research or publication, please cite our work:


[1]W. Chen, C. Liu, Y. Yan, L. Jin, X. Sun and X. Peng, **"Guided Dual Networks for Single Image Super-Resolution," in IEEE Access, vol. 8, pp. 93608-93620, 2020, doi: 10.1109/ACCESS.2020.2995175.**</i> [[PDF](https://ieeexplore.ieee.org/document/9097227)]
'''
@article{chen2020guided,
  title={Guided Dual Networks for Single Image Super-Resolution},
  author={Chen, Wenhui and Liu, Chuangchuang and Yan, Yitong and Jin, Longcun and Sun, Xianfang and Peng, Xinyi},
  journal={IEEE Access},
  volume={8},
  pages={93608--93620},
  year={2020},
  publisher={IEEE}
}
'''
