# HisDoc1B Dataset
The HisDoc1B dataset comprises 40,281 books, over 3 million document images, and over 1 billion characters across 30,615 character categories. To the best of our knowledge, HisDoc1B is the largest dataset in the field, surpassing existing datasets by more than 200 times in terms of scale (as shown in the below table). Additionally, it is the only dataset with complete book-level annotations and punctuation annotations. 



| Dataset | #Books | #Document images | #Characters | #Character categories | Text punctuation |
|---------|--------|-------------------|--------------|-----------------------|------------------|
| MTHv1[[1]] | -      | 1,500             | 521,370      | 4,058                | ×                |
| MTHv2[[2]] | -      | 3,199             | 1,081,678    | 6,733                | ×                |
| IC19 HDRC[[3]] | -    | <u>11,715</u>       | 2,482,994    | 8,353                | ×                |
| M5HisDoc[[4]] | -    | 8,000             | <u>4,367,360<u> | <u>16,151</u>           | ×                |
| CASIA-AHCDB[[5]] | -  | -                 | 2,276,740    | 10,350               | ×                |
| HisDoc1B (Ours) | **40,281** | **3,163,330** (270×) | **1,082,544,808** (248×) | **30,615** (1.9×) | ✓                |
<p align="center">Table 1: Comparison of HisDoc1B with existing Chinese historical document datasets. The highest and second highest values within each column are denoted by bold and underline, respectively.</p>


[1]: https://ieeexplore.ieee.org/document/8364534
[2]: https://ieeexplore.ieee.org/abstract/document/9257624
[3]: https://ieeexplore.ieee.org/document/8977999
[4]: https://proceedings.neurips.cc/paper_files/paper/2023/hash/f7b424d242cc6bb7708cff241367334d-Abstract-Datasets_and_Benchmarks.html
[5]: https://ieeexplore.ieee.org/document/8978010





# Usage & Download
OneDrive: https://1drv.ms/u/s!ApQfSeOP7LDTdPghMv281sKYsq0?e=fIuK65   
BaiduYun: https://pan.baidu.com/s/1CQnfmHwh6hGigyvHNlmPCQ?pwd=aziq  

The HisDoc1B dataset can only be used for non-commercial research purposes. Scholars or organizations wishing to use the HisDoc1B dataset should first complete this [Application Form](application-form/Application-Form-for-Using-HisDoc1B.docx) and send it via email to us ([lianwen.jin@gmail.com](mailto:lianwen.jin@gmail.com) or [eelwjin@scut.edu.cn](mailto:eelwjin@scut.edu.cn)). When submitting the application form to us, please list or attach 1-2 of your publications from the past 6 years to demonstrate that you (or your team) conduct research in the related research fields of Historical Document Analysis, Optical Character Recognition, Document Image Processing, and so on. Currently, this dataset is only freely available to scholars in the above-mentioned fields. **We will send you the decompression password for the dataset after your letter has been received and approved**.


# License
The HisDoc1B dataset should be used and distributed under the [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0) License](https://creativecommons.org/licenses/by-nc-nd/4.0/) for non-commercial research purposes.


# Directory Format
The dataset is organized in the following directory format:
```
├── HisDoc1B
    ├── books
    │   ├── xxx.pdf/.djvu
    │   └── ...
    ├── annos
    │   ├── xxx.json
    │   └── ...
    ├── readme.md
    ├── book2im.py
    ├── read_anno.py
```



# Citation
Please cite our paper when using the dataset:
```
@article{shi2025large,
  title={A large-scale dataset for Chinese historical document recognition and analysis},
  author={Shi, Yongxin and Peng, Dezhi and Zhang, Yuyi and Cao, Jiahuan and Jin, Lianwen},
  journal={Scientific Data},
  volume={12},
  number={1},
  pages={169},
  year={2025},
  publisher={Nature Publishing Group UK London}
}
```

# Contact
For any questions about the dataset, please contact the authors by sending an email to Prof. Jin([eelwjin@scut.edu.cn](mailto:eelwjin@scut.edu.cn), or [lianwen.jin@gmail.com](mailto:lianwen.jin@gmail.com)). 
