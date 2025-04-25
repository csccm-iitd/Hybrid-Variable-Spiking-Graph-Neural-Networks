# Hybrid-Variable-Spiking-Graph-Neural-Networks
This repository contains codes for the method described in the paper : "Hybrid variable spiking graph neural networks for energy-efficient scientific machine learning". Link to the paper is : https://arxiv.org/abs/2412.09379

## Instructions to Run Scripts
The folder ```/codes``` contains all ```.ipynb``` notebooks for which results have been shown on the paper for each example respectively. Each notebook consists of codes for training, plotting graphs, and printing error values. Before running all files, ensure all dataloader folders are downloaded from the links below and appropriate paths are changes on the notebooks accordingly.
* No extra utility files are needed in Example-1, all notebooks can be run as is 
* In Example-2, ```data.zip``` and ```hyper.zip``` need to be unzipped before run. ```norm.npz``` must stay as is
* In Example-3, notebooks for training and creating stress field plots have been provided separately. Checkpoint files obtained after training would be used as input to create the stress field maps. The code for stress field maps would also require raw data which can be downloaded from here [Data](https://drive.google.com/file/d/1eT30mFcywEpBwGm9R6MA1TOs1WoOzEjb/view?usp=sharing)
Also note that for each example, Spiking Activity is only stored as variables and printed during training, but has not been explicitly written to any external file, and will have to be done by the user. 

## Libraries Required
Please install the following libraries before running the scripts. Also note that cuda support is advised to avoid long training hours.
```
torch
torch_geometric
snntorch
seaborn
```

Below are links to zip files containing dataloaders for each respective example. Once downloaded, the scripts can be directly run.
1) Example-1 : https://drive.google.com/file/d/1AEmMN1XnRLZH8nG35Mhk_YNOf-DL02vx/view?usp=sharing
2) Example-2 : https://drive.google.com/file/d/1GELfVzBOLEnUjYwhPPUI7DPf1K1K-Vx6/view?usp=sharing
3) Example-3 : https://drive.google.com/file/d/1JpiHxgexKhUyBh9urRdr_CIqWddALRzA/view?usp=sharing

## References 
To access the actual datasets, and the data preparation methods, refer to the following papers for each example respectively. Github links for each can be found within the papers.
1. Example-1 : https://www.sciencedirect.com/science/article/abs/pii/S092702562200605X
2. Example-2 : https://www.nature.com/articles/s41524-021-00574-w
3. Example-3 : https://www.nature.com/articles/s41524-022-00879-4

## Citation
```
@article{jain2024hybrid,
  title={Hybrid variable spiking graph neural networks for energy-efficient scientific machine learning},
  author={Jain, Isha and Garg, Shailesh and Shriyam, Shaurya and Chakraborty, Souvik},
  journal={arXiv preprint arXiv:2412.09379},
  year={2024}
}
```
