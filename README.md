## 📖 Deep Learning for Face Generation and Editing: A Survey

[//]: # "Deep Face Generation and Control: A Survey"
[//]: # "Deep Face Generation and Editing: A Survey"
[//]: # "Deep Face Synthesis and Editing: A Survey"

-   [Applications Papers](#applications-papers)
-   [Applications Applied](#applications-applied)
-   [Datasets](#datasets)
-   [Neural Network Architectures for Generation of Faces](#neural-network-architectures-for-generation-of-faces)
-   [Similarity of Faces and Loses For Training](#similarity-of-faces-and-loses-for-training)
-   [The Latent Space](#the-latent-space)
-   [Image Inversion to a Latent Space of StyleGAN](#image-inversion-to-a-latent-space-of-stylegan)
-   [Editing of Generated Images ](#editing-of-generated-images)
-   [Finding control parameters in the latent space - Editing approaches](#finding-control-parameters-in-the-latent-space)
-   [Deep Fake](#deep-fake)
-   [Deblurring](#deblurring)

---

### Application Papers

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
Project: https://mystyle-personalized-prior.github.io/ <br/>

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

### Applications Applied

<br/>

**GANfolk: Using AI to Create Portraits of Fictional People to Sell as NFTs**
| <img src='/Images/gan_folks.jpeg' style='height: 225px'>
|:--:|
| Example Generated GanFolk Faces |

App: https://towardsdatascience.com/ganfolk-using-ai-to-create-portraits-of-fictional-people-to-sell-as-nfts-6e24f5214ed1 <br/>

Examples of GANFolks from OpenSea:

https://opensea.io/assets/matic/0x2953399124f0cbb46d2cbacd8a89cf0599974963/95949048702184002022994543019454797960309252011183799747181743845102298595329 <br/>

### Virtual Makeup and Accessories Try-on

| <img src='/Images/ffhqtarget.png' style='height: 250px'>
|:--:|
| Target Image |

#### Web Applications

| <img src='/Images/loreal.png' style='height: 200px'><img src='/Images/maybelline.png' style='height: 200px'><img src='/Images/nyx.png' style='height: 200px'> <img src='/Images/eyebuydirect.png' style='height: 200px; width: 200px'>
|:--:|
| Inference results from Loreal, Maybelline, Nyx and EyebuyDirect Website in Order |

**Loreal Virtual Makeup Try-on**

App: https://www.lorealparisusa.com/virtual-try-on-makeup <br/>

**Maybelline Virtual Makeup Try-on**

App: https://www.maybelline.com/virtual-try-on-makeup-tools <br/>

**NyxCosmetics Virtual Makeup Try-on**

App: https://www.nyxcosmetics.com/try-it-on.html <br/>

**EyebuyDirect Virtual Glasses Try-on**

App: https://www.eyebuydirect.com/virtual-try-on <br/>

#### Mobile Applications

| <img src='/Images/FaceApp.JPG' style='height: 200px'><img src='/Images/facelab.JPG' style='height: 200px'><img src='/Images/Facetune2.jpg' style='height: 200px'> <img src='/Images/peachy.PNG' style='height: 200px; width: 200px'><img src='/Images/youcam.JPG' style='height: 200px; width: 200px'>
|:--:|
| Inference results from FaceApp, FaceLab, Facetune2, Peachy and 'YouCam Makeup' iOs Apps in Order |

**FaceApp**

iOS App: https://apps.apple.com/us/app/faceapp-perfect-face-editor/id1180884341
Android App: https://play.google.com/store/apps/details?id=io.faceapp&hl=tr&gl=US

**FaceLab**

iOS App: https://apps.apple.com/de/app/facelab-gesicht-bearbeiten/id1361012099
Android App: https://play.google.com/store/apps/details?id=com.lyrebirdstudio.facelab&hl=tr&gl=US

**Facetune2**

iOS App: https://apps.apple.com/us/app/facetune2-editor-by-lightricks/id1149994032
Android App: https://play.google.com/store/apps/details?id=com.lightricks.facetune.free&hl=tr&gl=US

**Peachy**

iOS App: https://apps.apple.com/us/app/peachy-gesicht-bearbeiten/id1390423469?l=de

**YouCam Makeup**
iOS App: https://apps.apple.com/de/app/youcam-makeup-selfie-editor/id863844475
Android App: https://play.google.com/store/apps/details?id=com.cyberlink.youcammakeup&hl=tr&gl=US

**Video Face Replacement Using ReFace**
| <img src='/Images/reface-gif.gif' style='height: 300px'>
|:--:|
| Inference results from Reface App |

**Misterspex Virtual Glasses Try-on**

| <img src='/Images/glasses_spex.png' style='height: 300px'><img src='/Images/glasses_spex2.png' style='height: 300px'>
|:--:|
| Inference results from Misterspex Website |

App: https://www.misterspex.co.uk/l/pg/100508 <br/>

**ZenniOptical Virtual Glasses Try-on**

(ZenniOptical is using the same application for virtual try-on and the results are near identical - 24.06.2022)

App: https://www.zennioptical.com/tryon <br/>

**RealESRGAN Application**

|<img src='/Images/realesrin.png' style='height: 200px'><img src='/Images/realesrout.jpeg' style='height: 200px'>
|:--:|
| RealESR GAN Image Enchancement|

App: https://huggingface.co/spaces/akhaliq/Real-ESRGAN <br/>
Paper: https://arxiv.org/abs/2107.10833 <br/>

**My Heritage Deep Nostalgia**

App: https://www.myheritage.com/deep-nostalgia <br/>

| <img src='/Images/einsteinanim_small_opt.gif' style='height: 250px'>
|:--:|
| MyHeritage Image Animation |

**PhotoMyne Image Restoration**

| <img src='/Images/pymne.jpg' style='height: 250px'>
|:--:|
|PhotoMyne Old Image Restoration App |

App: https://photomyne.com/ <br/>

**Old Photo Restoration**

| <img src='/Images/solvay_half.png' style='height: 250px'>
|:--:|
| Target Image |

### Super Resolution and Deblurring

##### GPEN Face Restoration

| <img src='/Images/solvay_hq_half.png' style='height: 200px'><img src='/Images/vanceai_solvay_half.png' style='height: 200px'><img src='/Images/remini_solvay_half.png' style='height: 200px'>
|:--:|
| Solvay Conference Image Restoration Using GPEN, VanceAI and ReminiAI from left to right. |

App: https://replicate.com/yangxy/gpen <br/>

**VanceAI Image Restoration**

App: https://vanceai.com/old-photo-restoration/ <br/>

**ReminiAI Image Restoration**

App: https://remini.ai/ <br/>

##### Color Enhancement

**ImageColorizer Image Colorizer**

| <img src='/Images/solvay_colored_half.png' style='height: 250px'>
|:--:|
| Solvay Conference Image Colored |

App: https://imagecolorizer.com/ <br/>

**Nvidia Image Restoration**

 <img src='/Images/einstein.gif' style='height: 250px'>

App: https://www.nvidia.com/research/inpainting/index.html <br/>

<!-- **Befunky Cartoonize Photos**

| <img src='/Images/ffhqtarget.png' style='height: 350px'><img src='/Images/befunky.png' style='height: 350px'>
|:--:|
| Image Cartoonized Using Befunky |

App: https://www.befunky.com/features/photo-to-cartoon/ <br/> -->

**BoredApp Generation and CryptoPunks Generation**

| <img src='/Images/ape_small_opt.gif' style='height: 250px'>
|:--:|
| HugginNFT Generator Result [from](https://github.com/AlekseyKorshuk/huggingnft)|

App: https://huggingface.co/huggingnft/boredapeyachtclub <br/>
App: https://huggingface.co/huggingnft/cryptopunks <br/>

<!-- **Cartoonify Photos**

App: https://www.kapwing.com/cartoonify <br/>

(Didn't work at the time: 24.06.2022) -->

**Cartoonize Photos**

App: https://www.cartoonize.net/ <br/>

(Cartoonizing was a pro feature: 24.06.2022)

**Toonify.photos**

| <img src='/Images/arnold.jpg' style='height: 200px'>
|:--:|
| Arnold photo toonified [from](https://toonify.photos/)|

App: https://toonify.photos/ <br/>

---

### Datasets

<br/>

**A Style-Based Generator Architecture for Generative Adversarial Networks**

| <img src='/Images/ffhq_dataset.jpg' style='height: 225px'>
|:--:|
|FFHQ Dataset |

Paper: https://arxiv.org/abs/1812.04948 <br/>
Dataset: https://github.com/NVlabs/ffhq-dataset <br/>

**Celeb-a Dataset**

| <img src='/Images/celeba.png' style='height: 225px'>
|:--:|
|Celeb-a Dataset |

Dataset: https://github.com/tkarras/progressive_growing_of_gans <br/>

**Celeb-a Mask-HQ Dataset**

| <img src='/Images/celebamaskhq.jpeg' style='height: 225px'>
|:--:|
|Celeb-a Mash HQ Dataset |

Dataset: https://github.com/switchablenorms/CelebAMask-HQ <br/>

**Celeb-a Multi-Modal Dataset**

| <img src='/Images/celebamulti.jpg' style='height: 200px'>
|:--:|
|Celeb-a Multi-Modal Dataset |

Dataset: https://github.com/IIGROUP/MM-CelebA-HQ-Dataset <br/>

**FaceForensics++**

| <img src='/Images/forensics.jpg' style='height: 200px'>
|:--:|
|FaceForensics Dataset|

Github: https://github.com/ondyari/FaceForensics <br/>
Data/Description: http://niessnerlab.org/projects/roessler2018faceforensics.html <br/>

**DeepFake Detection Challenge Dataset**

| <img src='/Images/deepfakeds.jpeg' style='height: 250px'>
|:--:|
|DeepFake Detection Challenge Dataset|

Data/Description: https://ai.facebook.com/datasets/dfdc/

**FaceWarehouse: a 3D Facial Expression Database for Visual Computing**

| <img src='/Images/facewh.png' style='height: 250px'><img src='/Images/facewh2.png' style='height: 250px'>
|:--:|
|FaceWarehouseDataset|

Data/Description: http://kunzhou.net/zjugaps/facewarehouse/

**MetFaces**

| <img src='/Images/metfaces.png' style='height: 200px'>
|:--:|
|MetFaces |

Data/Description : https://paperswithcode.com/dataset/metfaces

**CelebDf**

| <img src='/Images/celeb-df.jpg' style='height: 200px'>
|:--:|
|CelebDf |

Data/Description : https://paperswithcode.com/dataset/celeb-df

**LFW (Labeled Faces in the Wild)**

| <img src='/Images/lfw.jpg' style='height: 200px'>
|:--:|
|LFW (Labeled Faces in the Wild) |

Data/Description : https://paperswithcode.com/dataset/lfw

**MegaFace (Retired Data set)**

| <img src='/Images/megaface.png' style='height: 200px'>
|:--:|
|MegaFace (Retired Data set) |

Data/Description : https://paperswithcode.com/dataset/megaface

**VGGFace2 HQ**
| <img src='/Images/vggface.png' style='height: 200px'>
|:--:|
|VGG Face 2 HQ|

Data/Description : https://paperswithcode.com/dataset/vggface2-hq

**ArtBench-10**

(Not a faces data set directly but used with stylegan2 to train conditional image generation models)

| <img src='/Images/art-bench-10.jpg' style='height: 250px'>
|:--:|
|ArtBench-10 |

Data/Description : https://paperswithcode.com/dataset/artbench-10

---

### Neural Network Architectures for Generation of Faces

<br/>

**Analyzing and Improving the Image Quality of StyleGAN**

Paper: https://arxiv.org/abs/1912.04958 <br/>
Code: https://github.com/NVlabs/stylegan2 <br/>

**DeepFaceLab: Integrated, flexible and extensible face-swapping framework**

Paper: https://arxiv.org/abs/2005.05535 <br/>
Code: https://github.com/iperov/DeepFaceLab <br/>

**MyStyle: A Personalized Generative Prior**

Paper: https://arxiv.org/abs/2203.17272 <br/>

**Third Time's the Charm? Image and Video Editing with StyleGAN3**

Paper: https://arxiv.org/abs/2201.13433 <br/>
Code: https://github.com/yuval-alaluf/stylegan3-editing <br/>

---

### Similarity of Faces and Loses For Training

<br/>

**ArcFace: Additive Angular Margin Loss for Deep Face Recognition**

Paper: https://arxiv.org/abs/1801.07698 <br/>

**The Unreasonable Effectiveness of Deep Features as a Perceptual Metric**

Paper: https://arxiv.org/abs/1801.03924 <br/>

**GANs Trained by a Two Time-Scale Update Rule Converge to a Local Nash Equilibrium**

Paper: https://arxiv.org/abs/1706.08500 <br/>
Code: https://github.com/NVlabs/stylegan3 <br/>

---

### The Latent Space

<br/>

**StyleSpace Analysis: Disentangled Controls for StyleGAN Image Generation**

Paper: https://arxiv.org/abs/2011.12799 <br/>

**Image2StyleGAN: How to Embed Images Into the StyleGAN Latent Space?-Supplementary Material**

Paper: https://openaccess.thecvf.com/content_ICCV_2019/supplemental/Abdal_Image2StyleGAN_How_to_ICCV_2019_supplemental.pdf <br/>

---

### Image Inversion to a Latent Space of StyleGAN

📄 Encoding in Style: a StyleGAN Encoder for Image-to-Image Translation <br />
Elad Richardson, Yuval Alaluf, Or Patashnik, Yotam Nitzan, Yaniv Azar, Stav Shapiro, Daniel Cohen-Or
<br /> CVPR 2021 [[Paper]](https://arxiv.org/abs/2008.00951) [[Video]](https://www.youtube.com/watch?v=bfvSwhqsTgM) [[GitHub]](https://github.com/eladrich/pixel2style2pixel)

📄 Designing an Encoder for StyleGAN Image Manipulation <br />
Omer Tov, Yuval Alaluf, Yotam Nitzan, Or Patashnik, Daniel Cohen-Or
<br />
[[Paper]](https://arxiv.org/abs/2102.02766)  [[Video]](https://dl.acm.org/doi/10.1145/3450626.3459838)  [[Github]](https://github.com/omertov/encoder4editing)

📄 ReStyle: A Residual-Based StyleGAN Encoder via Iterative Refinement <br />
Yuval Alaluf, Or Patashnik, Daniel Cohen-Or
<br /> ICCV 2021
[[Paper]](https://arxiv.org/abs/2104.02699)  [[Video]](https://www.youtube.com/watch?v=6pGzLECSIWM)  [[Github]](https://github.com/yuval-alaluf/restyle-encoder)

📄 Pivotal Tuning for Latent-based editing of Real Images <br />
Daniel Roich, Ron Mokady, Amit H. Bermano, Daniel Cohen-Or
<br /> ACM TOG 2022 
[[Paper]](https://arxiv.org/abs/2106.05744) [[Github]](https://github.com/danielroich/PTI)

📄 HyperStyle: StyleGAN Inversion with HyperNetworks for Real Image Editing <br />
Yuval Alaluf, Omer Tov, Ron Mokady, Rinon Gal, Amit H. Bermano
<br /> CVPR 2022 [[Paper]](https://arxiv.org/abs/2111.15666)  [[Video]](https://www.youtube.com/watch?v=_sbXmLY2jMw)  [[Github]](https://github.com/yuval-alaluf/hyperstyle)

📄 MyStyle: A Personalized Generative Prior <br />
Yotam Nitzan, Kfir Aberman, Qiurui He, Orly Liba, Michal Yarom, Yossi Gandelsman, Inbar Mosseri, Yael Pritch, Daniel Cohen-or
<br /> [[Paper]](https://arxiv.org/abs/2203.17272)  [[Video]](https://www.youtube.com/watch?v=axWo_9Gt47o)  [[Github]](https://mystyle-personalized-prior.github.io/)

---

### Editing of Generated Images

<br/>

**StyleCLIP: Text-Driven Manipulation of StyleGAN Imagery**

Paper: https://openaccess.thecvf.com/content/ICCV2021/html/Patashnik_StyleCLIP_Text-Driven_Manipulation_of_StyleGAN_Imagery_ICCV_2021_paper.html <br/>

**Designing an Encoder for StyleGAN Image Manipulation**

Paper: https://arxiv.org/abs/2102.02766 <br/>

**Learning Transferable Visual Models From Natural Language Supervision**

Paper: https://arxiv.org/abs/2103.00020 <br/>

---

### Finding control parameters in the latent space

<br/>

**Pivotal Tuning for Latent-based Editing of Real Images**

Paper: https://arxiv.org/abs/2106.05744 <br/>

**Analyzing and Improving the Image Quality of StyleGAN**

Paper: https://arxiv.org/abs/1912.04958 <br/>
Code: https://github.com/NVlabs/stylegan2 <br/>

---

### Deep Fake

<br/>

**DeepFaceLab: Integrated, flexible and extensible face-swapping framework**

Paper: https://arxiv.org/abs/2005.05535 <br/>
Code: https://github.com/iperov/DeepFaceLab <br/>

---

### Deblurring

<br/>

**GAN Prior Embedded Network for Blind Face Restoration in the Wild**

Paper: https://arxiv.org/abs/2105.06070 <br/>
Code: https://github.com/yangxy/GPEN <br/>

**Towards Real-World Blind Face Restoration with Generative Facial Prior**

Paper: https://arxiv.org/abs/2101.04061 <br/>
Code: https://github.com/TencentARC/GFPGAN <br/>

**Deblurring by Realistic Blurring**

Paper: https://arxiv.org/abs/2004.01860v2 <br/>
Code: https://github.com/HDCVLab/Deblurring-by-Realistic-Blurring <br/>

**DeblurGAN-v2: Deblurring (Orders-of-Magnitude) Faster and Better**

Paper: https://arxiv.org/abs/1908.03826v1 <br/>
Code: https://github.com/VITA-Group/DeblurGANv2 <br/>

**ESRGAN: Enhanced Super-Resolution Generative Adversarial Networks**

Paper: https://arxiv.org/abs/1809.00219 <br/>
Code: https://github.com/xinntao/ESRGAN <br/>
