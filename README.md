# FingerprintFeatureExtraction
The important fingerprint minutiae features are the ridge endpoints (a.k.a. Terminations) and Ridge Bifurcations.



The feature set for the image consists of the location of Terminations and Bifurcations and their orientations

## Installation and Running the tests

 ## method 1
 ```
  pip install fingerprint-feature-extractor
 ```
 
 **Usage:**
  ```
  import fingerprint_feature_extractor
  img = cv2.imread('image_path', 0)				# read the input image --> You can enhance the fingerprint image using the "fingerprint_enhancer" library
  FeaturesTerminations, FeaturesBifurcations = fingerprint_feature_extractor.extract_minutiae_features(img, spuriousMinutiaeThresh=10, invertImage=False, showResult=True, saveResult=True)
```
 ## method 2
- from the src folder, run the file "main.py"
- **the input image is stored in the folder "enhanced".**
***If the input image is not enhanced, the minutiae features will be very noisy***

# Libraries needed:
- opencv
- skimage
- numpy
- math
