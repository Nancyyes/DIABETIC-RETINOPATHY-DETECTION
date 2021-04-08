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


#### What we do is not to directly input various-size image. By adding 0 to small size image, which make them as the same as max-size image. 0 (zero) will be ignored as backgroup in the model. 
Why still use FCN? Becuase images we use is not equal width and height (they are same size,but ratio of width and height is not 1), and CNN doesn't work well on such images. Also, by resizeing images to have equal width and height, it will have to sacrifice a lots of imformation.
This way we have a batch with equal image dimensions but every batch has a different shape (due to difference in max height and width of images across batches)
 
