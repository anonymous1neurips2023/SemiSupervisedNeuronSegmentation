# Semi-Supervised Deep Learning for Neuron Segmentation with Fewer Ground Truth Labels

Requirements: 
CUDA compatible GPU, Anaconda

## Demo:

### Install Pipeline

1) Download repository and save to easily identifiable directory - e.g. *C:/Users/{username}/Documents/segmentation* 

2) Open Anaconda prompt and type:  

        cd segmentation_directory
        cd installation
        conda env create -f environment_suns.yml -n suns 
        
  this uses Tensorflow V1, for Tensorflow V2, use environment_suns_tf2.yml
  
3) Go to the Anaconda environment folder, (e.g., C:/ProgramData/Anaconda3/envs or C:/Users/{username}/.conda/envs), and then go to folder suns/Lib/site-packages/fissa, overwrite core.py with the files provided in the installation folder. The modified files increase speed by eliminating redundant separate or separation_prep during initializating an Experiment object, and enable videos whose size are larger than 4 GB after converting to float32. If neither of them is important to you, then you can skip replacing the files. If you see a lot of text output when activating suns environment and do not want to see them, you can go to the Anaconda environment foler, go to folder suns/etc/conda/activate.d, and delete the two files under this folder. 

### Download Data





