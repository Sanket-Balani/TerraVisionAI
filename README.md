**TerraVisionAI: A Comprehensive Geospatial AI Solution**

**Overview**

TerraVisionAI is a powerful geospatial AI solution designed to address critical challenges in terrain analysis and object detection. This project leverages cutting-edge technologies like Google Earth Engine, Deep Learning, and YOLOv8 to provide accurate and efficient insights from satellite imagery.
![image](https://github.com/user-attachments/assets/0c3f73a1-c963-45f6-a8d9-d605e7f6aaa9)


**Key Components**

1. **Terrain Segmentation with Google Earth Engine:**
   * **Purpose:** Segments terrain into distinct regions based on specific criteria like land cover, elevation, or vegetation.
   * **Methodology:** 
     - Utilizes Google Earth Engine's vast satellite imagery and powerful cloud computing capabilities.
     - Implements clustering-based segmentation techniques to categorize terrain into meaningful segments.
     - Visualizes the segmented terrain using interactive maps.
   * **Notebook:** TerrainSegmentation_GoogleEarthEngine.ipynb
     ![image](https://github.com/user-attachments/assets/8c5fe7f7-f4b7-4f57-8345-4649a7365b3a)


2. **Terrain Mapping and Recognition with Deep Learning:**
   * **Purpose:** Classifies different land cover types within a given terrain using deep learning models.
   * **Methodology:**
     - Employs a pre-trained Wide ResNet model for feature extraction.
     - Trains the model on the EuroSAT dataset to classify land cover types like forests, urban areas, and agricultural land.
     - Evaluates the model's performance using metrics like accuracy and F1-score.
   * **Notebook:** Terrain_Mapping_Deep_Learning_Model.ipynb

     Highway: ![image](https://github.com/user-attachments/assets/8639b17a-c377-4dca-9a1c-33a18ccc7680)
     Industrial: ![image](https://github.com/user-attachments/assets/4dcb35b4-1431-4287-9a01-f89d19beea7f)


3. **Object Detection with YOLOv8:**
   * **Purpose:** Detects and classifies objects within satellite images, such as buildings, roads, and vehicles.
   * **Methodology:**
     - Leverages the YOLOv8 model, a state-of-the-art object detection architecture.
     - Trains the model on the DIOR dataset, which contains a diverse range of objects in satellite imagery.
     - Evaluates the model's performance using metrics like mAP (mean Average Precision).
   * **Notebook:** dior_object_detection_satellite_imagery_yolov8.ipynb
     ![image](https://github.com/user-attachments/assets/8ed6fd82-55b2-421e-96b6-71202be1977c)


**Installation and Setup**

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Sanket-Balani/TerraVisionAI.git
   ```
2. **Install Dependencies:**
   Ensure you have the following libraries installed:
   ```bash
   pip install earthengine-api rasterio numpy matplotlib seaborn tqdm torch torchvision ultralytics
   ```
3. **Set up Google Earth Engine:**
   Follow the instructions to authenticate and initialize the Earth Engine API.

**Usage**

1. **Run Notebooks:**
   Execute each notebook sequentially to perform the respective tasks.
   * **Terrain Segmentation:** Follow the steps in `TerrainSegmentation_GoogleEarthEngine.ipynb` to load satellite imagery, perform segmentation, and visualize results.
   * **Terrain Mapping:** Run `Terrain_Mapping_Deep_Learning_Model.ipynb` to train the deep learning model, evaluate its performance, and make predictions on new images.
   * **Object Detection:** Execute `dior_object_detection_satellite_imagery_yolov8.ipynb` to train the YOLOv8 model, evaluate its performance, and make predictions on new images or videos.

**Potential Applications**

* **Urban Planning:** Identify urban growth patterns, monitor infrastructure development, and assess urban heat islands.
* **Disaster Management:** Detect and monitor natural disasters like floods, fires, and landslides.
* **Agriculture:** Monitor crop health, estimate crop yields, and optimize irrigation practices.
* **Environmental Monitoring:** Track deforestation, monitor pollution levels, and assess biodiversity.

**Future Directions**

* **Integration:** Combine the three components into a unified platform for comprehensive geospatial analysis.
* **Real-time Processing:** Explore real-time processing of satellite imagery using cloud-based solutions.
* **Advanced Deep Learning Techniques:** Experiment with more advanced deep learning architectures like transformers for improved performance.
* **Explainable AI:** Develop techniques to interpret the decisions made by the models, enhancing transparency and trust.

By leveraging the power of AI and satellite imagery, TerraVisionAI aims to contribute to sustainable development, environmental conservation, and disaster response efforts.
