# PELMI
PELMI is a DNA storage codec algorithm for images. In short, it can convert images into binary data, and binary data into DNA sequences. In decoding, the bases can be converted into images. The algorithm helps to achieve high reconstruction of thought and high quality DNA sequences. Before using this repository, we implore you to have a basic understanding of DNA-based data storage. Here you can see a case of improper communication for your reference.
## Installation and use
Environment Configuration
The kit is developed by Python3.7.3.
In addition, the packages we are calling now is as follows:
```
sys
os
random
numpy
cv2
PIL
math
struct
datetime
pickle
```
Another simply way is
```
conda install --yes --file requirements.txt
```
Or
```
pip install -r requirements.txt
```
### Introduction of PELMI
PELMI is an algorithm based on parity coding and local mean iteration reported by Wang et al.
Users can run PELMI 
```
/examples/new_work.py
```
 directly, by entering the image, setting the error scale, obtaining the encoding sequence, and rebuilding the image.
 
Users can install 
```"pip install chamaeleo"``` to test other schemes for encoding encoded sequences and reconstructing images.
In the encoding process
```
read_image_path = "SOURCE.xx"
dna_path = "XXXXXX.dna"
error_rate = “***”
pipeline(read_image_path, error_rate, dna_path)
```
In the decoding process
```
Python
write_file_path = "TARGET.xx"
dna_path = "XXXXXX.dna"
decode(write_file_path, dna_path)
```
### Citing

If you think this repo helps or being used in your research, please consider refer this paper.

@article{10.1093/bib/bbae463,
    author = {Cao, Ben and Wang, Kun and Xie, Lei and Zhang, Jianxia and Zhao, Yunzhu and Wang, Bin and Zheng, Pan},
    title = "{PELMI: Realize robust DNA image storage under general errors via parity encoding and local mean iteration}",
    journal = {Briefings in Bioinformatics},
    volume = {25},
    number = {5},
    pages = {bbae463},
    year = {2024},
    month = {09},
    issn = {1477-4054},
    doi = {10.1093/bib/bbae463},
    url = {https://doi.org/10.1093/bib/bbae463},
    eprint = {https://academic.oup.com/bib/article-pdf/25/5/bbae463/59148283/bbae463.pdf},
}

Thank you!
