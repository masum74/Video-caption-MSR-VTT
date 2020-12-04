## VIDEO CAPTIONING WITH MSR-VTT DATASET

* Dataset is available here:  https://www.mediafire.com/folder/h14iarbs62e7p/shared

* A trained version of the model can be found here: https://drive.google.com/file/d/1-GfiBd_CfW0IcUNOMpGDwUIReXA_z0sn/view?usp=sharing. This was trained using 5 frames per video, with batch size 128.

* We have modified a code originally written for image captioning. Thanks to Ziyan Yang  (zy3cx@virginia.edu)!


### Description

*  This is a vision + language based model for video captioning. It is trained using 20,000 video clips as training data and 5,000 video clips as validation data from the MSR-VTT (MSRVideo to Text) dataset. From each video clips 5 scattered frames were extracted and fed into a video encoder (ResNet152) to generate an encoded output. This output is then passeda to a text decoder (sequence of LSTM models) to generate meaningful caption for the video.
