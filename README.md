# Semantic Correspondence Methods Paper List


## Contents
- [Handcrafted Descriptors](#handcrafted-descriptors)
- [Architectural Improvement](#architectural-improvement)
  - [Feature Enhancement](#feature-enhancement)
     - [Feature Assembly](#Feature-assembly)
     - [Feature Adaptation](#Feature-adaptation)
  - [Matching Refinement](#matching-refinement)
     - [Cost Volume-Based Methods](#cost-volume-based-methods)
     - [Flow Field-Based Methods](#flow-field-based-methods)
     - [Parameterized Transformation-Based Methods](#parameterized-transformation-based-methods)
  - [Other Improvements](#other-improvements)
- [Training Strategy Improvement](#training-strategy-improvement)
  - [Non-Keypoint Label-Based Methods](#non-keypoint-label-based-methods)
  - [Cycle/Warp Consistency-Based Methods](#cyclewarp-consistency-based-methods)
  - [Pseudo-Label Generation-Based Methods](#pseudo-label-generation-based-methods)
  - [Other Improvements](#other-improvements)

---

## Handcrafted Descriptors
- A maximum entropy framework for part-based texture and object recognition, ICCV 2005. [Paper](https://ieeexplore.ieee.org/document/1541339)
  
    S. Lazebnik, C. Schmid, J. Ponce

- Flexible Object Models for Category-Level 3D Object Recognition, CVPR 2007. [Paper](https://ieeexplore.ieee.org/document/4270174/)

    Akash Kushal, Cordelia Schmid, Jean Ponce

- Sift flow: Dense correspondence across scenes and its applications, TPAMI 2011. [Paper](https://ieeexplore.ieee.org/document/5551153)

    Ce Liu, Jenny Yuen, Antonio Torralba

- Deformable spatial pyramid matching for fast dense correspondences, CVPR 2013. [Paper](https://openaccess.thecvf.com/content_cvpr_2013/papers/Kim_Deformable_Spatial_Pyramid_2013_CVPR_paper.pdf)

    Jaechul Kim, Ce Liu, Fei Sha, Kristen Grauman

- DAISY Filter Flow: A Generalized Discrete Approach to Dense Correspondences, CVPR 2014. [Paper](https://openaccess.thecvf.com/content_cvpr_2014/papers/Yang_DAISY_Filter_Flow_2014_CVPR_paper.pdf)

    Hongsheng Yang, Wen-Yan Lin, Jiangbo Lu

- Unsupervised object discovery and localization in the wild: Part-based matching with bottom-up region proposals, CVPR 2015. [Paper](https://ieeexplore.ieee.org/document/7298724/)

    Minsu Cho, Suha Kwak, Cordelia Schmid, Jean Ponce

- Proposal flow, CVPR 2016. [Paper](https://openaccess.thecvf.com/content_cvpr_2016/papers/Ham_Proposal_Flow_CVPR_2016_paper.pdf)

    Bumsub Ham, Minsu Cho, Cordelia Schmid, Jean Ponce

- Proposal flow: Semantic correspondences from object proposals, TPAMI 2018. [Paper](https://arxiv.org/abs/1703.07144)

    Bumsub Ham, Minsu Cho, Cordelia Schmid, Jean Ponce


### Other Improvements
- Deep ViT Features as Dense Visual Descriptors, ECCVW 2022. [paper](https://arxiv.org/abs/2112.05814)

    Shir Amir, Yossi Gandelsman, Shai Bagon, Tali Dekel

- GAN-Supervised Dense Visual Alignment, CVPR 2022. [paper](https://arxiv.org/abs/2112.05143)

    William Peebles, Jun-Yan Zhu, Richard Zhang, Antonio Torralba, Alexei A. Efros, Eli Shechtman

- CoordGAN: Self-Supervised Dense Correspondences Emerge from GANs. CVPR 2022. [paper](https://arxiv.org/abs/2203.16521)

    Jiteng Mu, Shalini De Mello, Zhiding Yu, Nuno Vasconcelos, Xiaolong Wang, Jan Kautz, Sifei Liu

- Space-Time Correspondence as a Contrastive Random Walk, NeurIPS 2021. [paper](https://arxiv.org/abs/2006.14613)

    Allan Jabri, Andrew Owens, Alexei A. Efros

- Deep Matching Prior: Test-Time Optimization for Dense Correspondence, ICCV 2021. [paper](https://arxiv.org/abs/2106.03090)

    Sunghwan Hong, Seungryong Kim


## Architectural Improvement
Early CNN methods

- Universal correspondence network, NeurIPS 2016. [Paper](https://arxiv.org/abs/1606.03558)

    Christopher B. Choy, JunYoung Gwak, Silvio Savarese, Manmohan Chandraker

- SCNet: Learning semantic correspondence, ICCV 2017. [Paper](https://arxiv.org/abs/1705.04043)
  
    Kai Han, Rafael S. Rezende, Bumsub Ham, Kwan-Yee K. Wong, Minsu Cho, Cordelia Schmid, Jean Ponce

- FCSS: Fully Convolutional Self-Similarity for Dense Semantic Correspondence, CVPR 2017, [Paper](https://openaccess.thecvf.com/content_cvpr_2017/papers/Kim_FCSS_Fully_Convolutional_CVPR_2017_paper.pdf). TPAMI 2019, [Paper](https://ieeexplore.ieee.org/document/8283767)

    Seungryong Kim, Dongbo Min, Bumsub Ham, Stephen Lin, Kwanghoon Sohn

### Feature Enhancement

#### Feature Assembly

- Hypercolumns for object segmentation and fine-grained localization, CVPR 2015. [Paper](https://openaccess.thecvf.com/content_cvpr_2015/papers/Hariharan_Hypercolumns_for_Object_2015_CVPR_paper.pdf)

    Bharath Hariharan, Pablo Arbeláez, Ross Girshick, Jitendra Malik

- Hyperpixel Flow: Semantic Correspondence with Multi-layer Neural Features, ICCV 2019. [Paper](https://openaccess.thecvf.com/content_ICCV_2019/papers/Min_Hyperpixel_Flow_Semantic_Correspondence_With_Multi-Layer_Neural_Features_ICCV_2019_paper.pdf)

    Juhong Min, Jongmin Lee, Jean Ponce, Minsu Cho

- Learning to Compose Hypercolumns for Visual Correspondence, ECCV 2020. [Paper](https://arxiv.org/abs/2007.10587)

    Juhong Min, Jongmin Lee, Jean Ponce, Minsu Cho

- Multi-scale matching networks for semantic correspondence, ICCV 2021. [Paper](https://arxiv.org/abs/2108.00211)

    Dongyang Zhao, Ziyang Song, Zhenghao Ji, Gangming Zhao, Weifeng Ge, Yizhou Yu

- Efficient Semantic Matching with Hypercolumn Correlation, WACV 2024. [Paper](https://arxiv.org/abs/2311.04336)

    Seungwook Kim, Juhong Min, Minsu Cho

- Independently Keypoint Learning for Small Object Semantic Correspondence, arXiv preprint 2024. [Paper](https://arxiv.org/abs/2404.02678)

    Hailong Jin, Huiying Li

- Pixel-level Semantic Correspondence through Layout-aware Representation Learning and Multi-scale Matching Integration, CVPR 2024. [Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Sun_Pixel-level_Semantic_Correspondence_through_Layout-aware_Representation_Learning_and_Multi-scale_Matching_CVPR_2024_paper.pdf)

    Yixuan Sun, Zhangyue Yin, Haibo Wang, Yan Wang, Xipeng Qiu, Weifeng Ge

- Diffusion hyperfeatures: Searching through time and space for semantic correspondence, NeurIPS 2023. [Paper](https://arxiv.org/abs/2305.14334)

    Grace Luo, Lisa Dunlap, Dong Huk Park, Aleksander Holynski, Trevor Darrell

- A tale of two features: Stable diffusion complements dino for zero-shot semantic correspondence, NeurIPS 2023. [Paper](https://arxiv.org/abs/2305.15347)

    Junyi Zhang, Charles Herrmann, Junhwa Hur, Luisa Polania Cabrera, Varun Jampani, Deqing Sun, Ming-Hsuan Yang

#### Feature Adaptation

- SimSC: A Simple Framework for Semantic Correspondence with Temperature Learning, arXiv preprint 2023. [Paper](https://arxiv.org/abs/2305.02385)

    Xinghui Li, Kai Han, Xingchen Wan, Victor Adrian Prisacariu

- SD4Match: Learning to Prompt Stable Diffusion Model for Semantic Matching, CVPR 2024. [Paper](https://arxiv.org/abs/2310.17569)

    Xinghui Li, Jingyi Lu, Kai Han, Victor Adrian Prisacariu

- Unsupervised semantic correspondence using stable diffusion, NeurIPS 2023. [Paper](https://arxiv.org/abs/2305.15581)

    Eric Hedlin, Gopal Sharma, Shweta Mahajan, Hossam Isack, Abhishek Kar, Andrea Tagliasacchi, Kwang Moo Yi

- Telling left from right: Identifying geometry-aware semantic correspondence, CVPR 2024. [Paper](https://arxiv.org/abs/2311.17034)

    Junyi Zhang, Charles Herrmann, Junhwa Hur, Eric Chen, Varun Jampani, Deqing Sun, Ming-Hsuan Yang

- LiFT: A Surprisingly Simple Lightweight Feature Transform for Dense ViT Descriptors, ECCV 2024. [Paper](https://arxiv.org/abs/2403.14625)

    Saksham Suri, Matthew Walmer, Kamal Gupta, Abhinav Shrivastava


### Matching Refinement

#### Cost Volume-Based Methods

- Neighbourhood consensus networks, NeurIPS 2018. [Paper](https://arxiv.org/abs/1810.10510)

    Ignacio Rocco, Mircea Cimpoi, Relja Arandjelović, Akihiko Torii, Tomas Pajdla, Josef Sivic

- Correspondence networks with adaptive neighbourhood consensus, CVPR 2020. [Paper](https://arxiv.org/abs/2003.12059)

    Shuda Li, Kai Han, Theo W. Costain, Henry Howard-Jenkins, Victor Adrian Prisacariu

- Dual-resolution correspondence networks, NeurIPS 2020. [Paper](https://arxiv.org/abs/2006.08844)

    Xinghui Li, Kai Han, Shuda Li, Victor Adrian Prisacariu

- DualRC: A Dual-Resolution Learning Framework With Neighbourhood Consensus for Visual Correspondences, TPAMI 2024. [Paper](https://ieeexplore.ieee.org/document/10255317)

    Xinghui Li, Kai Han, Shuda Li, Victor Adrian Prisacariu

- Convolutional Hough Matching Networks, CVPR 2021. [Paper](https://arxiv.org/abs/2103.16831)

    Juhong Min, Minsu Cho

- Convolutional hough matching networks for robust and efficient visual correspondence, TPAMI 2023. [Paper](https://ieeexplore.ieee.org/document/10008958?denied=)

    Juhong Min, Seungwook Kim, Minsu Cho


- Patchmatch-based neighborhood consensus for semantic correspondence, CVPR 2021. [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Lee_PatchMatch-Based_Neighborhood_Consensus_for_Semantic_Correspondence_CVPR_2021_paper.pdf)

    Jae Yong Lee, Joseph DeGol, Victor Fragoso, Sudipta N. Sinha

- Cats: Cost aggregation transformers for visual correspondence, NeurIPS 2021. [Paper](https://arxiv.org/abs/2106.02520)

    Seokju Cho, Sunghwan Hong, Sangryul Jeon, Yunsung Lee, Kwanghoon Sohn, Seungryong Kim

- Cats++: Boosting cost aggregation with convolutions and transformers, TPAMI 2023. [Paper](https://arxiv.org/abs/2202.06817)

    Seokju Cho, Sunghwan Hong, Seungryong Kim

- Cost aggregation with 4D convolutional swin transformer for few-shot segmentation, ECCV 2022. [Paper](https://arxiv.org/abs/2207.10866)

    Sunghwan Hong, Seokju Cho, Jisu Nam, Stephen Lin, Seungryong Kim

- Neural matching fields: Implicit representation of matching fields for visual correspondence, NeurIPS 2022. [Paper](https://arxiv.org/abs/2210.02689)

    Sunghwan Hong, Jisu Nam, Seokju Cho, Susung Hong, Sangryul Jeon, Dongbo Min, Seungryong Kim

- Integrative feature and cost aggregation with transformers for dense correspondence, arXiv preprint 2022. [Paper](https://arxiv.org/abs/2209.08742)

    Sunghwan Hong, Seokju Cho, Seungryong Kim, Stephen Lin

- Unifying Feature and Cost Aggregation with Transformers for Semantic and Visual Correspondence, ICLR 2024. [Paper](https://arxiv.org/abs/2403.11120)

    Sunghwan Hong, Seokju Cho, Seungryong Kim, Stephen Lin

- Transformatcher: Match-to-match attention for semantic correspondence, CVPR 2022. [Paper](https://arxiv.org/abs/2205.11634)

    Seungwook Kim, Juhong Min, Minsu Cho

#### Flow Field-Based Methods
- SFNet: Learning object-aware semantic correspondence, CVPR 2019. [Paper](https://arxiv.org/abs/1904.01810)

    Junghyup Lee, Dohyung Kim, Jean Ponce, Bumsub Ham

- Learning Semantic Correspondence Exploiting an Object-Level Prior, TPAMI 2022. [Paper](https://arxiv.org/abs/1911.12914)

    Junghyup Lee, Dohyung Kim, Wonkyung Lee, Jean Ponce, Bumsub Ham

- GLU-Net: Global-Local Universal Network for Dense Flow and Correspondences, CVPR 2020. [Paper](https://arxiv.org/abs/1912.05524)

    Prune Truong, Martin Danelljan, Radu Timofte

- Correspondence transformers with asymmetric feature learning and matching flow super-resolution, CVPR 2023. [Paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Sun_Correspondence_Transformers_With_Asymmetric_Feature_Learning_and_Matching_Flow_Super-Resolution_CVPR_2023_paper.pdf)

    Yixuan Sun, Dongyang Zhao, Zhangyue Yin, Yiwen Huang, Tao Gui, Wenqiang Zhang

- Pixel-level Semantic Correspondence through Layout-aware Representation Learning and Multi-scale Matching Integration, CVPR 2024. [Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Sun_Pixel-level_Semantic_Correspondence_through_Layout-aware_Representation_Learning_and_Multi-scale_Matching_CVPR_2024_paper.pdf)

    Yixuan Sun, Zhangyue Yin, Haibo Wang, Yan Wang, Xipeng Qiu, Weifeng Ge


#### Parameterized Transformation-Based Methods

- Attentive Semantic Alignment with Offset-Aware Correlation Kernels, ECCV 2018. [Paper](https://arxiv.org/abs/1808.02128)

    Paul Hongsuck Seo, Jongmin Lee, Deunsol Jung, Bohyung Han, Minsu Cho

- End-to-end weakly-supervised semantic alignment, CVPR 2018. [Paper](https://arxiv.org/abs/1712.06861)

    Ignacio Rocco, Relja Arandjelović, Josef Sivic

- Recurrent transformer networks for semantic correspondence,  NeurIPS 2018. [Paper](https://arxiv.org/abs/1810.12155)

    Seungryong Kim, Stephen Lin, Sangryul Jeon, Dongbo Min, Kwanghoon Sohn

- PARN: Pyramidal Affine Regression Networks for Dense Semantic Correspondence, ECCV 2018. [Paper](https://arxiv.org/abs/1807.02939)

    Sangryul Jeon, Seungryong Kim, Dongbo Min, Kwanghoon Sohn


## Training Strategy Improvement

### Non-Keypoint Label-Based Methods

- Proposal flow, CVPR 2016. [Paper](https://openaccess.thecvf.com/content_cvpr_2016/papers/Ham_Proposal_Flow_CVPR_2016_paper.pdf)

    Bumsub Ham, Minsu Cho, Cordelia Schmid, Jean Ponce

- Proposal flow: Semantic correspondences from object proposals, TPAMI 2018. [Paper](https://arxiv.org/abs/1703.07144)

    Bumsub Ham, Minsu Cho, Cordelia Schmid, Jean Ponce

- FCSS: Fully Convolutional Self-Similarity for Dense Semantic Correspondence, CVPR 2017, [Paper](https://openaccess.thecvf.com/content_cvpr_2017/papers/Kim_FCSS_Fully_Convolutional_CVPR_2017_paper.pdf). TPAMI 2019, [Paper](https://ieeexplore.ieee.org/document/8283767)

    Seungryong Kim, Dongbo Min, Bumsub Ham, Stephen Lin, Kwanghoon Sohn

- Recurrent transformer networks for semantic correspondence,  NeurIPS 2018. [Paper](https://arxiv.org/abs/1810.12155)

    Seungryong Kim, Stephen Lin, Sangryul Jeon, Dongbo Min, Kwanghoon Sohn

- Neighbourhood consensus networks, NeurIPS 2018. [Paper](https://arxiv.org/abs/1810.10510)

    Ignacio Rocco, Mircea Cimpoi, Relja Arandjelović, Akihiko Torii, Tomas Pajdla, Josef Sivic

- SFNet: Learning object-aware semantic correspondence, CVPR 2019. [Paper](https://arxiv.org/abs/1904.01810)

    Junghyup Lee, Dohyung Kim, Jean Ponce, Bumsub Ham

- Learning Semantic Correspondence Exploiting an Object-Level Prior, TPAMI 2022. [Paper](https://arxiv.org/abs/1911.12914)

    Junghyup Lee, Dohyung Kim, Wonkyung Lee, Jean Ponce, Bumsub Ham

- Learning to Compose Hypercolumns for Visual Correspondence, ECCV 2020. [Paper](https://arxiv.org/abs/2007.10587)

    Juhong Min, Jongmin Lee, Jean Ponce, Minsu Cho

- Weakly Supervised Learning of Semantic Correspondence through Cascaded Online Correspondence Refinement, ICCV 2023. [Paper](https://ieeexplore.ieee.org/document/10377845)

    Yiwen Huang, Yixuan Sun, Chenghang Lai, Qing Xu, Xiaomei Wang, Xuli Shen


### Cycle/Warp Consistency-Based Methods

- FlowWeb: Joint image set alignment by weaving consistent, pixel-wise correspondences, CVPR 2015. [Paper](https://ieeexplore.ieee.org/document/7298723)

    Tinghui Zhou, Yong Jae Lee, Stella X. Yu, Alexei A. Efros

- Learning dense correspondence via 3d-guided cycle consistency, CVPR 2016. [Paper](https://arxiv.org/abs/1604.05383)

    Tinghui Zhou, Philipp Krähenbühl, Mathieu Aubry, Qixing Huang, Alexei A. Efros
    
- Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks, ICCV 2017. [Paper](https://arxiv.org/abs/1703.10593)

    Jun-Yan Zhu, Taesung Park, Phillip Isola, Alexei A. Efros

- FCSS: Fully Convolutional Self-Similarity for Dense Semantic Correspondence, CVPR 2017, [Paper](https://openaccess.thecvf.com/content_cvpr_2017/papers/Kim_FCSS_Fully_Convolutional_CVPR_2017_paper.pdf). TPAMI 2019, [Paper](https://ieeexplore.ieee.org/document/8283767)

    Seungryong Kim, Dongbo Min, Bumsub Ham, Stephen Lin, Kwanghoon Sohn

- Deep Semantic Matching with Foreground Detection and Cycle-Consistency, ACCV 2018. [Paper](https://arxiv.org/abs/2004.00144)

    Yun-Chun Chen, Po-Hsiang Huang, Li-Yu Yu, Jia-Bin Huang, Ming-Hsuan Yang, Yen-Yu Lin

- Semantic Matching by Weakly Supervised 2D Point Set Registration, WACV 2019. [Paper](https://arxiv.org/abs/1901.08341)

    Zakaria Laskar, Hamed R. Tavakoli, Juho Kannala

- Show, Match and Segment: Joint Weakly Supervised Learning of Semantic Matching and Object Co-segmentation, TPAMI 2020. [Paper](https://arxiv.org/abs/1906.05857)

    Yun-Chun Chen, Yen-Yu Lin, Ming-Hsuan Yang, Jia-Bin Huang

- Semantic Correspondence via 2D-3D-2D Cycle, arXiv preprint 2020. [Paper](Semantic Correspondence via 2D-3D-2D Cycle)

    Yang You, Chengkun Li, Yujing Lou, Zhoujun Cheng, Lizhuang Ma, Cewu Lu, Weiming Wang

- GLU-Net: Global-Local Universal Network for Dense Flow and Correspondences, CVPR 2020. [Paper](https://arxiv.org/abs/1912.05524)

    Prune Truong, Martin Danelljan, Radu Timofte

- Warp consistency for unsupervised learning of dense correspondences, ICCV 2021. [Paper](https://arxiv.org/abs/2104.03308)

    Prune Truong, Martin Danelljan, Fisher Yu, Luc Van Gool

- Probabilistic warp consistency for weakly-supervised semantic correspondences, CVPR 2022. [Paper](https://arxiv.org/abs/2203.04279)

    Prune Truong, Martin Danelljan, Fisher Yu, Luc Van Gool

### Pseudo-Label Generation-Based Methods

- Probabilistic model distillation for semantic correspondence, CVPR 2021. [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Li_Probabilistic_Model_Distillation_for_Semantic_Correspondence_CVPR_2021_paper.pdf)

    Xin Li, Deng-Ping Fan, Fan Yang, Ao Luo, Hong Cheng, Zicheng Liu

- Learning semantic correspondence with sparse annotations, ECCV 2022. [Paper](https://arxiv.org/abs/2208.06974)

    Shuaiyi Huang, Luyu Yang, Bo He, Songyang Zhang, Xuming He, Abhinav Shrivastava

- Match me if you can: Semantic Correspondence Learning with Unpaired Images, ACCV 2024. [Paper](https://arxiv.org/abs/2311.18540)

    Jiwon Kim, Byeongho Heo, Sangdoo Yun, Seungryong Kim, Dongyoon Han

- Semi-supervised learning of semantic correspondence with pseudo-labels, CVPR 2022. [Paper](https://arxiv.org/abs/2203.16038)

    Jiwon Kim, Kwangrok Ryoo, Junyoung Seo, Gyuseong Lee, Daehwan Kim, Hansang Cho, Seungryong Kim

- Weakly Supervised Learning of Semantic Correspondence through Cascaded Online Correspondence Refinement, ICCV 2023. [Paper](https://ieeexplore.ieee.org/document/10377845)

    Yiwen Huang, Yixuan Sun, Chenghang Lai, Qing Xu, Xiaomei Wang, Xuli Shen

### Other Improvements

- DCTM: Discrete-Continuous Transformation Matching for Semantic Flow, ICCV 2017. [Paper](https://ieeexplore.ieee.org/document/8237747)

    Seungryong Kim, Dongbo Min, Stephen Lin, Kwanghoon Sohn

- Discrete-Continuous Transformation Matching for Dense Semantic Correspondence, TPAMI 2020. [Paper](https://ieeexplore.ieee.org/document/8510898)

    Seungryong Kim, Dongbo Min, Stephen Lin, Kwanghoon Sohn


- Semantic Correspondence as an Optimal Transport Problem, cvpr 2020. [Paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Liu_Semantic_Correspondence_as_an_Optimal_Transport_Problem_CVPR_2020_paper.pdf)

    Yanbin Liu, Linchao Zhu, Makoto Yamada, Yi Yang


- Dense Contrastive Learning for Self-Supervised Visual Pre-Training, CVPR 2021. [paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Wang_Dense_Contrastive_Learning_for_Self-Supervised_Visual_Pre-Training_CVPR_2021_paper.pdf)

   Xinlong Wang, Rufeng Zhang, Chunhua Shen, Tao Kong, Lei Li

- Unsupervised Learning of Dense Visual Representations, NeurIPS 2020. [paper](https://arxiv.org/abs/2011.05499)

    Pedro O. O. Pinheiro, Amjad Almahairi, Ryan Benmalek, Florian Golemo, Aaron C. Courville

 - ASIC: Aligning Sparse in-the-wild Image Collections, ICCV 2023. [Paper](https://arxiv.org/abs/2303.16201)

    Kamal Gupta, Varun Jampani, Carlos Esteves, Abhinav Shrivastava, Ameesh Makadia, Noah Snavely, Abhishek Kar

- Demystifying unsupervised semantic correspondence estimation, ECCV 2022. [Paper](https://arxiv.org/abs/2207.05054) 

    Mehmet Aygün, Oisin Mac Aodha

- Improving Semantic Correspondence with Viewpoint-Guided Spherical Maps, CVPR 2024. [Paper](https://arxiv.org/abs/2312.13216)

    Octave Mariotti, Oisin Mac Aodha, Hakan Bilen

- Distillation of Diffusion Features for Semantic Correspondence, WACV 2025. [Paper](https://arxiv.org/abs/2412.03512)

    Frank Fundel, Johannes Schusterbauer, Vincent Tao Hu, Björn Ommer
    