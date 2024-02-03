## Dataset available here: [HMC-QU](https://www.kaggle.com/datasets/aysendegerli/hmcqu-dataset?select=LV+Ground-truth+Segmentation+Masks)


**The benchmark dataset is created by the collaboration between Hamad Medical Corporation (HMC), Tampere University, and Qatar University.**

**The temporal resolution (frame rate per second) of the echocardiography recordings is 25 fps.**

**The spatial resolution varies from 422x636 to 768x1024 pixels.**

**The dataset can be utilized for both myocardial infarction (heart attack) detection and left ventricle wall segmentation purposes. The later is the case here.**

  - Apical 4-chamber

      - The dataset consists of 162 A4C view 2D echocardiography recordings.

  - Apical 2-chamber

      - The dataset consists of 160 A2C view 2D echocardiography recordings.


## Segmentation of the Left Ventricle Wall 

**A subset of 109 A4C view echocardiography recordings has their corresponding ground-truth segmentation masks for the whole left ventricle wall at each frame for one cardiac cycle. This subset includes 72 MI patients and 37 non-MI subjects.**

**The size of the ground-truth segmentation masks is 224x224 in order to have suitable input dimensions for many state-of-the-art deep network topologies.**

### References
