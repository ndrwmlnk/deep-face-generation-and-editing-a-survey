# 📖 Deep Learning for Face Generation and Editing: A Survey

[//]: # "Deep Face Generation and Control: A Survey"
[//]: # "Deep Face Generation and Editing: A Survey"
[//]: # "Deep Face Synthesis and Editing: A Survey"

### Introduction

<br />

-   [1. Introduction](#introduction)
-   [2. Applications](#applications)
-   [2b. Datasets](#datasets)
-   [3. Neural Network Architectures for Generation of Faces](#neural-network-architectures-for-generation-of-faces)
-   [4. Similarity of Faces and Loses For Training](#similarity-of-faces-and-loses-for-training)
-   [5. The Latent Space](#the-latent-space)
-   [6. GAN Inversion to the Latent Space](#gan-inversion-to-the-latent-space)
-   [7. Editing of Generated Images ](#editing-of-generated-images)
-   [8. Finding control parameters in the latent space - Editing approaches](#finding-control-parameters-in-the-latent-space)
-   [9. Deep Fake](#deep-fake)
-   [10. Deblurring](#deblurring)

---

### Applications

<br/>

**GANfolk: Using AI to Create Portraits of Fictional People to Sell as NFTs**
| <img src='/Images/gan_folks.jpeg' style='height: 225px'>
|:--:|
| Example Generated GanFolk Faces |

App: https://towardsdatascience.com/ganfolk-using-ai-to-create-portraits-of-fictional-people-to-sell-as-nfts-6e24f5214ed1 <br/>

Examples of GANFolks from OpenSea:

https://opensea.io/assets/matic/0x2953399124f0cbb46d2cbacd8a89cf0599974963/95949048702184002022994543019454797960309252011183799747181743845102298595329 <br/>

**Ca-GAN: Weakly supervised color aware gan for controllable makeup transfer**

| <img src='/Images/cagan.png' style='height: 225px'>
|:--:|
| Ca-GAN Approach to Transfer Makeup styles |

Paper: https://arxiv.org/abs/2008.10298 <br/>

**Towards real-world blind face restoration with generative facial prior**

| <img src='/Images/gfpgan.png' style='height: 225px'>
|:--:|
| GFP-GAN Compared to Other Approaches and GT |

Paper: https://arxiv.org/abs/2101.04061 <br/>
Code: https://github.com/TencentARC/GFPGAN <br/>

**MyStyle: A Personalized Generative Prior**

| <img src='/Images/mystyle.png' style='height: 200px'> | <img src='/Images/mystyle2.png' style='height: 200px'> |
| :---------------------------------------------------: | :----------------------------------------------------: |
|                    Solarized dark                     |                    Solarized Ocean                     |

Paper: https://arxiv.org/abs/2203.17272 <br/>
Project Page: https://mystyle-personalized-prior.github.io/ <br/>

**Normalized Avatar Synthesis Using StyleGAN and Perceptual Refinement**

| <img src='/Images/normalizedavatar.png' style='height: 225px'>
|:--:|
| Normalized Avatar Synthesis Using StyleGAN and Perceptual Refinement Examples |

Paper: https://arxiv.org/abs/2106.11423 <br/>

**DeepFaceLab: Integrated, flexible and extensible faceswapping framework**

|<img src='/Images/deepfake.png' style='height: 225px'>
|:--:|
| Deepface Labs results from original [paper](https://arxiv.org/pdf/2005.05535.pdf) |

Paper: https://arxiv.org/pdf/2005.05535.pdf <br/>
Code: https://github.com/iperov/DeepFaceLab <br/>

**Loreal Virtual Makeup Try-on**

App: https://www.lorealparisusa.com/virtual-try-on-makeup <br/>

**Maybelline Virtual Makeup Try-on**
| <img src='/Images/ffhqtarget.png' style='height: 350px'><img src='/Images/maybelline.png' style='height: 350px'>
|:--:|
| Inference results from Maybelline Website |

App: https://www.maybelline.com/virtual-try-on-makeup-tools <br/>

**NyxCosmetics Virtual Makeup Try-on**

| <img src='/Images/ffhqtarget.png' style='height: 350px'><img src='/Images/nyx.png' style='height: 350px'>
|:--:|
| Inference results from Nyx Website |

App: https://www.nyxcosmetics.com/try-it-on.html <br/>

**EyebuyDirect Virtual Glasses Try-on**

| <img src='/Images/ffhqtarget.png' style='height: 350px'><img src='/Images/eyebuydirect.png' style='height: 350px'>
|:--:|
| Inference results from EyebuyDirect Website |

App: https://www.eyebuydirect.com/virtual-try-on <br/>

**Misterspex Virtual Glasses Try-on**

| <img src='/Images/glasses_spex.png' style='height: 400px'><img src='/Images/glasses_spex2.png' style='height: 400px'>
|:--:|
| Inference results from Misterspex Website |

App: https://www.misterspex.co.uk/l/pg/100508 <br/>

**ZenniOptical Virtual Glasses Try-on**

(ZenniOptical is using the same application for virtual try-on and the results are near identical - 24.06.2022)

App: https://www.zennioptical.com/tryon <br/>

**GPEN Face Restoration**

| <img src='/Images/solvay_half.png' style='height: 350px'><img src='/Images/solvay_hq_half.png' style='height: 350px'>
|:--:|
| Solvay Conference Images With GPEN Inference |

App: https://replicate.com/yangxy/gpen <br/>

**RealESRGAN Application**

|<img src='/Images/realesrin.png' style='height: 350px'><img src='/Images/realesrout.jpeg' style='height: 350px'>
|:--:|
| Solvay Conference Images With GPEN Inference |

App: https://huggingface.co/spaces/akhaliq/Real-ESRGAN <br/>

**My Heritage Deep Nostalgia**

App: https://www.myheritage.com/deep-nostalgia <br/>

| ![](/Images/einsteinanim.gif)
|:--:|
| Solvay Conference Images With GPEN Inference |

**PhotoMyne Image Restoration**

App: https://photomyne.com/ <br/>

**ImageColorizer Image Colorizer**

| <img src='/Images/solvay_half.png' style='height: 350px'><img src='/Images/solvay_colored_half.png' style='height: 350px'>
|:--:|
| Solvay Conference Image Colored|

App: https://imagecolorizer.com/ <br/>

**VanceAI Image Restoration**

| <img src='/Images/solvay_half.png' style='height: 350px'><img src='/Images/vanceai_solvay_half.png' style='height: 350px'>
|:--:|
| Solvay Conference Image Enhanced Using VanceAI |

App: https://vanceai.com/old-photo-restoration/ <br/>

**Nvidia Image Restoration**

(Didn't work at the moment)

App: https://www.nvidia.com/research/inpainting/index.html <br/>

**ReminiAI Image Restoration**

| <img src='/Images/solvay_half.png' style='height: 350px'><img src='/Images/remini_solvay_half.png' style='height: 350px'>
|:--:|
| Solvay Conference Image Enhanced Using ReminiAI |

App: https://remini.ai/ <br/>

**Befunky Cartoonize Photos**

| <img src='/Images/ffhqtarget.png' style='height: 350px'><img src='/Images/befunky.png' style='height: 350px'>
|:--:|
| Image Cartoonized Using Befunky |

App: https://www.befunky.com/features/photo-to-cartoon/ <br/>

**BoredApp Generation and CryptoPunks Generation**

| ![](/Images/bored_compressed.gif)
|:--:|
| HugginNFT Generator Result [from](https://github.com/AlekseyKorshuk/huggingnft)|

App: https://huggingface.co/huggingnft/boredapeyachtclub <br/>
App: https://huggingface.co/huggingnft/cryptopunks <br/>

**Cartoonify Photos**

App: https://www.kapwing.com/cartoonify <br/>

(Didn't work at the time: 24.06.2022)

**Cartoonize Photos**

App: https://www.cartoonize.net/ <br/>

(Cartoonizing was a pro feature: : 24.06.2022)

**Toonify.photos**

App: https://toonify.photos/ <br/>

(Asking for a license key at the moment: : 24.06.2022)

---

### Datasets

**A Style-Based Generator Architecture for Generative Adversarial Networks**

| <img src='/Images/ffhq_dataset.jpg' style='height: 300px'>
|:--:|
|FFHQ Dataset |

Paper: https://arxiv.org/abs/1812.04948 <br/>
Dataset repo: https://github.com/NVlabs/ffhq-dataset <br/>

**Celeb-a Dataset**

| <img src='/Images/celeba.png' style='height: 300px'>
|:--:|
|Celeb-a Dataset |

Dataset Repo: https://github.com/tkarras/progressive_growing_of_gans <br/>

**Celeb-a Mask-HQ Dataset**

| <img src='/Images/celebamaskhq.jpeg' style='height: 300px'>
|:--:|
|Celeb-a Mash HQ Dataset |

Dataset Repo: https://github.com/switchablenorms/CelebAMask-HQ <br/>

**Celeb-a Multi-Modal Dataset**

| <img src='/Images/celebamulti.jpg' style='height: 300px'>
|:--:|
|Celeb-a Multi-Modal Dataset |

Dataset Repo: https://github.com/IIGROUP/MM-CelebA-HQ-Dataset <br/>

---

### Neural Network Architectures for Generation of Faces

<br/>

**Analyzing and Improving the Image Quality of StyleGAN**

https://github.com/NVlabs/stylegan2
https://arxiv.org/abs/1912.04958 <br />

**DeepFaceLab: Integrated, flexible and extensible face-swapping framework**

https://arxiv.org/abs/2005.05535
https://github.com/iperov/DeepFaceLab <br/>

**MyStyle: A Personalized Generative Prior**

https://arxiv.org/abs/2203.17272 <br/>

**Third Time's the Charm? Image and Video Editing with StyleGAN3**

https://arxiv.org/abs/2201.13433
https://github.com/yuval-alaluf/stylegan3-editing <br/>

---

### Similarity of Faces and Loses For Training

<br/>

**ArcFace: Additive Angular Margin Loss for Deep Face Recognition**

https://arxiv.org/abs/1801.07698 <br />

**The Unreasonable Effectiveness of Deep Features as a Perceptual Metric**

https://arxiv.org/abs/1801.03924 <br />

**GANs Trained by a Two Time-Scale Update Rule Converge to a Local Nash Equilibrium**

https://arxiv.org/abs/1706.08500
https://github.com/NVlabs/stylegan3 <br />

---

### The Latent Space

<br/>

**StyleSpace Analysis: Disentangled Controls for StyleGAN Image Generation**

https://arxiv.org/abs/2011.12799 <br />

**Image2StyleGAN: How to Embed Images Into the StyleGAN Latent Space?-Supplementary Material**

https://openaccess.thecvf.com/content_ICCV_2019/supplemental/Abdal_Image2StyleGAN_How_to_ICCV_2019_supplemental.pdf <br />

---

### GAN Inversion (to the Latent Space)

<br/>

**Encoding in Style: a StyleGAN Encoder for Image-to-Image Translation**

https://arxiv.org/abs/2008.00951 <br />

**Analyzing and Improving the Image Quality of StyleGAN**

https://arxiv.org/abs/1912.04958 <br />

---

### Editing of Generated Images

<br/>

**StyleCLIP: Text-Driven Manipulation of StyleGAN Imagery**

https://openaccess.thecvf.com/content/ICCV2021/html/Patashnik_StyleCLIP_Text-Driven_Manipulation_of_StyleGAN_Imagery_ICCV_2021_paper.html <br />

**Designing an Encoder for StyleGAN Image Manipulation**

https://arxiv.org/abs/2102.02766 <br />

**Learning Transferable Visual Models From Natural Language Supervision**

https://arxiv.org/abs/2103.00020 <br />

---

### Finding control parameters in the latent space

<br/>

**Pivotal Tuning for Latent-based Editing of Real Images**

https://arxiv.org/abs/2106.05744 <br />

**Analyzing and Improving the Image Quality of StyleGAN**

https://github.com/NVlabs/stylegan2
https://arxiv.org/abs/1912.04958 <br />

---

### Deep Fake

<br />

**DeepFaceLab: Integrated, flexible and extensible face-swapping framework**

https://arxiv.org/abs/2005.05535
https://github.com/iperov/DeepFaceLab <br/>

---

### Deblurring

<br />

**GAN Prior Embedded Network for Blind Face Restoration in the Wild**
https://arxiv.org/abs/2105.06070
https://github.com/yangxy/GPEN <br />

**Towards Real-World Blind Face Restoration with Generative Facial Prior**
https://arxiv.org/abs/2101.04061
https://github.com/TencentARC/GFPGAN <br/>

**Deblurring by Realistic Blurring**
https://arxiv.org/abs/2004.01860v2
https://github.com/HDCVLab/Deblurring-by-Realistic-Blurring <br/>

**DeblurGAN-v2: Deblurring (Orders-of-Magnitude) Faster and Better**
https://arxiv.org/abs/1908.03826v1
https://github.com/VITA-Group/DeblurGANv2 <br/>

**ESRGAN: Enhanced Super-Resolution Generative Adversarial Networks**
https://arxiv.org/abs/1809.00219
https://github.com/xinntao/ESRGAN <br/>
