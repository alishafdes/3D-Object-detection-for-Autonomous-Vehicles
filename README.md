# 3D-Object-detection-for-Autonomous-Vehicles

![alt text](https://www.chp.ca.gov/CommercialVehicleSectionSite/PublishingImages/Pages/Autonomous-Vehicles/Autonomuos%20Vehicles.PNG)

Our project focuses on 3D Object Detection of Lyft’s autonomous vehicles. We used the Lyft dataset which was part of a [kaggle competition](https://www.kaggle.com/c/3d-object-detection-for-autonomous-vehicles/overview). We used 3D point cloud data as well as camera data to perform both segmentation and localization. 

For preprocessing of the data, the lidar point clouds were transformed using matrix transformations. This transformed data was then fed into a UNET model.
We implemented changes in the architecture of the UNET model in terms of optimizers, batch size, sampling, etc. to obtain the best possible solution.

Due to the high volume of data, the analysis and training of the model was performed in Google Cloud Platform. Additionally, we used the [lyft_dataset_sdk](https://github.com/lyft/nuscenes-devkit) for data manipulation and transformation.

A detailed explanation of our approach and results can be found in our blog - [3D-Object Detection for Autonomous Vehicles](https://towardsdatascience.com/3d-object-detection-for-autonomous-vehicles-b5f480e40856).