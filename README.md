# depth-CNN
The goal of this project is to use a mix between Simultaneous Localisation And Mapping (SLAM) and Depth Prediction with different Deep Learning models to get better depth prediction from short videos. Indeed, feature-based visual SLAM gives sparse information of depth with high accuracy but no scale while learned models give dense information with scale and medium accuracy.
That's what Mukasa and al. [1] stated and therefore proposed a method to improve CNN-depth predictions with mesh deformation based on key points localisation.
We believe that this idea could be further explored in using the localisations as secondary entry to the DP model. 

The plan is to modify state-of-the-art models from Ranftl [2] by adding extra layers and including a secondary input of known depth points.
The reference SLAM network will be ORB-SLAM.
The training can be done on synthetized data without the implication of SLAM.
