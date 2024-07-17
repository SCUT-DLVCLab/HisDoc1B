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


# Download
OneDrive: https://1drv.ms/u/s!ApQfSeOP7LDTdPghMv281sKYsq0?e=fIuK65   
BaiduYun: https://pan.baidu.com/s/1CQnfmHwh6hGigyvHNlmPCQ?pwd=aziq  

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


# Inference codes to generate the dataset
* Download the docker image:  
OneDrive: https://1drv.ms/u/s!ApQfSeOP7LDTc0VErUM9NBjQLls?e=gVTcqw  
BaiduYun: https://pan.baidu.com/s/1OV_RjZ8pf9QJlCrMDFvztA?pwd=wdlm   

* Initialize the docker container:
    ```bash
    docker load -i hisdoc1b-docker.tar
    docker run -it --gpus all --shm-size="2g" hisdoc1b-image:20240716
    ```

* The code are in the /root/HisDoc1B_codes/.


# Contact
For any questions about the dataset, please contact the authors by sending an email to [yongxin_shi@foxmail.com](mailto:yongxin_shi@foxmail.com). 
