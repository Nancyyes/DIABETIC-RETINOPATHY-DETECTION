# IABETIC-RETINOPATHY-DETECTION
Problem:
1. Different size of images
2. Unstandard - object images
3. Cannot standardize by traditional ways: encircle, cutting. Because dart spot on image is randomly distrbuted. If directly cut or remove, we may miss important information
4. Sample heavely imbalanced
Solution:
1. fully convolutional network
2. Elastic Deformations

On - going problems:
1. Retinopathy image is not like breast tumor which are gathered. It's randomly distributed. So, the traditional way of mass detection didn't work very well. 
