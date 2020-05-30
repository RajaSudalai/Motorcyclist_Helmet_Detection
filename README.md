# Automatic traffic violation detection of Motorcyclist not wearing Helmet - Instance Segmentation using Mask R-CNN


### Authors: 
####		Sudalaiandi Raja Sudalaimuthu
####		Jayaraman Revathi

# Objective 

#### To develop a reliable and efficient Artificial intelligent system for detecting helmet use by motorcycle riders that does not rely on a human observer. The purpose of this project is to reliably detect and segment the motorcyclist wearing helmet and not wearing helmet.

# Installation guideline

#### Below are the steps to complete conda environment and folder structure setup

- Download and Setup Ananconda if you base conda does not exist


- open `Ananconda Prompt`


- 
` conda config --append channels conda-forge`


- Create a virtual conda environment 'helmet'
` conda create -n helmet python=3.6 numpy=1.15.1 opencv=3.4.2 matplotlib=2.2.3 tensorflow-gpu=1.12.0 scipy=1.1.0 scikit-learn=0.19.1 spyder=3.3.2 yaml=0.1.7 keras-gpu=2.1.6 pillow=5.4.1 notebook=5.7.4 pandas=0.24.2 h5py=2.8.0 cython  Pillow scikit-image  imgaug IPython[all] tqdm`


- Activate helmet conda environment
` conda activate helmet`


- Install pycocotools for cocoapi for datasets preparation
` pip install git+https://github.com/philferriere/cocoapi.git#egg=pycocotools^&subdirectory=PythonAPI`


- Clone from Helmet_Mask_RCNN project from the git repository
` git clone https://github.com/aivoyagers/Helmet_Mask_RCNN.git`


- Change current working directory to project base folder
` cd Helmet_Mask_RCNN`


- Setup Helmet_Mask_RCNN environment
` python setup.py install`


- Download datasets and offline trained model files from the google drive and copy to 'Helmt_Mask_RCNN' base folder 
` https://drive.google.com/drive/folders/1VHDlu76J1bScRBSy-4WsWI_mldf_Pf-b?usp=sharing`


- Open Jupyter Notebook for executing helmet_detect API
` jupyter notebook`


- Update 'COMMAND' to 'train' if fresh training on downloaded helmet 'train' & 'val' datasets. For test or inference, 'val' datasets required

- Execute helmet_detect.ipynb

# Demo Samples

![Motorcyclist without Helmet detection using Mask R-CNN](demo/helmet_detection_mask.png)

![Motorcyclist without Helmet detection using Mask R-CNN](https://github.com/RajaSudalai/Motorcyclist_Helmet_Detection/blob/master/demo/motorcyclist_helmet_use.mp4)

<div align="center">
    <img src="demo/motorcyclist_helmet_use.gif", width="800">
</div>


- 

## Citation
```
@misc{matterport_maskrcnn_2017,
  title={Mask R-CNN for object detection and instance segmentation on Keras and TensorFlow},
  author={Waleed Abdulla},
  year={2017},
  publisher={Github},
  journal={GitHub repository},
  howpublished={\url{https://github.com/matterport/Mask_RCNN}},
}
```