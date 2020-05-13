## Video Object Segmentation using Space-Time Memory Networks
### Seoung Wug Oh, Joon-Young Lee, Ning Xu, Seon Joo Kim
### ICCV 2019
[[paper]](http://openaccess.thecvf.com/content_ICCV_2019/html/Oh_Video_Object_Segmentation_Using_Space-Time_Memory_Networks_ICCV_2019_paper.html)

[![Video Object Segmentation using Space-Time Memory Networks (ICCV 2019)](https://img.youtube.com/vi/vVZiBEDmgIU/0.jpg)](https://www.youtube.com/watch?v=vVZiBEDmgIU "Video Object Segmentation using Space-Time Memory Networks (ICCV 2019)")



### - Requirements
- python 3.6
- pytorch 1.0.1.post2
- numpy, opencv, pillow

### - How to Use
#### Download weights
##### Place it the same folder with demo scripts
```
wget -O STM_weights.pth "https://www.dropbox.com/s/mtfxdr93xc3q55i/STM_weights.pth?dl=1"
```

#### Run
##### DAVIS-2016 validation set (Single-object)
``` 
python eval_DAVIS.py -g '1' -s val -y 16 -D [path/to/DAVIS]
```
##### DAVIS-2017 validation set (Multi-object)
``` 
python eval_DAVIS.py -g '1' -s val -y 17 -D [path/to/DAVIS]
```



### - Reference 
If you find our paper and repo useful, please cite our paper. Thanks!
``` 
Video Object Segmentation using Space-Time Memory Networks
Seoung Wug Oh, Joon-Young Lee, Ning Xu, Seon Joo Kim
ICCV 2019
```

### - Related Project
``` 
Fast Video Object Segmentation by Reference-Guided Mask Propagation
Seoung Wug Oh, Joon-Young Lee, Kalyan Sunkavalli, Seon Joo Kim
CVPR 2018
```
[[paper]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Oh_Fast_Video_Object_CVPR_2018_paper.pdf)
[[github]](https://github.com/seoungwugoh/RGMP)


### - Interactive VOS (Quantitative Evaluation)
A modified STM model is used for DAVIS Interactive VOS Challenge 2019 (https://davischallenge.org/challenge2019/interactive.html). 
If you are intersted in comparison with our interactive STM model, please use evaluation summary obtained from the [DAVIS framework](https://interactive.davischallenge.org/). The timing is measured using a single 2080Ti GPU.
[[Download link (DAVIS-17-val)]](https://www.dropbox.com/s/owoms3rtalg52wn/STM_Interactive_summary_DAVIS17_val.json?dl=1).
We will make a demo software available soon. 
For the further questions, please contact me by E-mail.


### - Terms of Use
This software is for non-commercial use only.
The source code is released under the Attribution-NonCommercial-ShareAlike (CC BY-NC-SA) Licence
(see [this](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode) for details)
