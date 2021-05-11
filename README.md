# I3CL: Intra- and Inter-Instance Collaborative Learning for Arbitrary-shaped Scene Text Detection.
This software implements I3CL: Intra- and Inter-Instance Collaborative Learning for Arbitrary-shaped Scene Text Detection in PyTorch.   

# Installation
This implementation is based on [Detectron2](https://github.com/facebookresearch/detectron2), the installation can refer to step-by-step installation.  

# Run demo
A demo program can be found in demo, which can save the detected text contours in txt file and visualize the detection results. Set the path of files (include model, testing images, configs, output etc.) in demo/***_detection.py.  Then launch demo by:
    
    python demo/art_detection.py

# Evaluation
The detection demo will save text contours to an txt file for each images. For calculating the Recall, Precision, and F-measure, please refer to evaluation.  

# Train a new model
Before training，please register your datasets in detectron2/data/datasets/builtin.py. Set training implementation details in configs/ocr/***.yaml.  To train a model with 4 gpus，please run:

    python tools/train_net.py --num-gpus 4 --config-file configs/ocr/art_50_FPN.yaml



