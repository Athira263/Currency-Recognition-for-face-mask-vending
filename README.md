# Currency-Recognition-for-face-mask-vending

Prerequisites/Downloads needed: 

  

1. Visual Studio C++ Installer: https://visualstudio.microsoft.com/vs/   

2. Visual Studio C++  Build Tools:https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=16  

3. Anaconda and Tensorflow: https://www.anaconda.com/ 

4. DataSet: https://www.kaggle.com/datasets 

5. Tensorflow Model: https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md 

  

Steps To Follow: 

  

1. Open CMD , Change Directory to "D" (D:). 

2. Git clone https://github.com/nicknochnack/RealTimeObjectDetection to clone this repository and use the code. 

3. Labelling Img Library: git clone https://github.com/tzutalin/labelImg     (Do this inside Tensorflow folder)   (cd RealTimeObjectDetection\Tensorflow) 

4. Get Inside the Tensorflow folder,Workspace folder, Images folder and copy-paste the data set in train and test folders ( Donot paste the same images in test and train folders)  

5. Install Anaconda, Visual Studio C++, Optional(CUDA and cudNN If you have gpu) 

6. Install Anaconda and Tensorflow packages as specified inside  https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html  

7.  conda install pyqt=5  

    conda install -c anaconda lxml 

8.  pyrcc5 -o resources.py resources.qrc. Cut and paste resources.py and resources.qrc files into libs.  

9. Get Inside "D: RealTimeObjectDetection" and activate tensorflow virtual environment using (conda activate xyz). 

10. Run the code inside Jupyter Notebooks (jupyter notebook) 

11. After 6th Step an error will be encountered as we need to train the model before further execution. After successfull Execution till 6th step, Run (python Tensorflow/models/research/object_detection/model_main_tf2.py --model_dir=Tensorflow/workspace/models/my_ssd_mobnet --pipeline_config_path=Tensorflow/workspace/models/my_ssd_mobnet/pipeline.config --num_train_steps=5000) this command in the cmd. It will take take to completely train the model. Once completed, we can continue the execution and detect denominations in currency through Live webcam feed. 
