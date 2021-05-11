# Create a new conda environment
conda create --name i3cl python=3.7.3  
conda activate i3cl  

# Intsall pytorch 1.3.1
conda install pytorch=1.3.1 torchvision cudatoolkit=10.1 -c pytorch  

# Install other libraries for building I3CL-detectron2
pip install opencv-python  
pip install tensorboard  
pip install yacs  
pip install tqdm  
pip install termcolor  
pip install tabulate  
pip install matplotlib  
pip install cloudpickle  
pip install wheel  
pip install pycocotools  

# Rebuild fvcore, we rebuild it for training more conveniently
pip install fvcore-master.zip  

# Build I3CL-detectron2, which needs cuda-10.1 and gcc-4.9
python setup.py build develop  



