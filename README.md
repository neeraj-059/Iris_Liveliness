### DESCRIPTION:
Iris is one of the most important biometric approaches that can perform high confidence recognition.
This eye-liveness detection depend on the reaction of pupil diameter size during the existence of the
ambient light while iris recognition is based on matching the iris—with the one previously stored in 
a database—two times.

### NORMALIZATION:
![image](/images/7.jpg)
![image](/images/8.jpg)
![image](/images/normalisetoiris.jpg)

-This was done with matlab 
![image](/images/test.png)

### MATCHING:
The assumpion is made as the first image is the user's iris at first and the second image is his expanded iris which he showed after closing and opening his eyes 
again according to the procedure. Now both the images are matched with the previously stored images.

### Results:
1. Iris code generation process:
![image](/images/iriscode01.png)

Done using ModelSim
![image](/images/codegen.png)

## Matched
![image](/images/id2.png)
![image](/images/id3.png)

How to run the program
1. Download the CASIA Iris Image Database(version 1.0) from (http://biometrics.idealtest.org/dbDetailForUser.do?id=1) 
2. Read all images and extract features using the read_all_images.m and createiristemplate.m. 
3. The templates of each subject will be saved into template.mat and mask.m after you creating the templates. Using matching.m to calculate the Hamming distance (HD) for the same subject(intra-class) and different subjects (innner-class) and saving the results into HD_diff.mat and HD_same.m.
