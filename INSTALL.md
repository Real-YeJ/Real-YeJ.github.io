## Installation

### Requirements:
- PyTorch 1.3.1
- torchvision
- matplotlib
- GCC >= 4.9
- OpenCV
- CUDA >= 10.1


### Step-by-step installation

```bash
# create a new conda environment

conda create --name i3cl python=3.7.3
conda activate i3cl

# install pytorch 1.3.1
conda install pytorch=1.3.1 torchvision cudatoolkit=10.1 -c pytorch

# install other libraries for building I3CL-detectron2
pip install opencv-python tensorboard yacs tqdm termcolor tabulate matplotlib cloudpickle wheel pycocotools

# rebuild the fvcore, we rebuild it for training more conveniently
cd I3CL
pip install fvcore-master.zip

# Build I3CL-detectron2, which needs CUDA >= 10.1 and GCC >= 4.9
python setup.py build develop

