# Neural Network Finger Printer

### Project Overview
This is a final project for CS-GY 9223: DEEP LEARNING at New York University Tandon School of Engineering. The goal of the project is to use a neural network for the purpose of fingerprinting audio data. The neural network used is based off work by Google in their paper [Now Playing: Continuous low-power music
recognition](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46522.pdf). This project is for education purposes ONLY and uses code found on other Github repositories. Two projects that I modified code from are [Triplet Loss](https://github.com/CrimyTheBold/tripletloss) and [Music Genre Classification](https://github.com/celestinhermez/music-genre-classification).

This project is using my own account with NYU's HPC resources. When creating directory structure, make sure to replace anything with my username jw6254 with your own. To see some system requirements, please look at the [sbatch script](https://github.com/jawooson/deep-learning-final/blob/master/sbatch_files/run-jupyter.sbatch) provided. 

### Data Download

1. Clone the directory

```bash
git clone https://github.com/jawooson/deep-learning-final.git
cd deep-learning-final
```

2. Install dependencies

```bash
conda env create --name music --file=/yml_files/requirements.yml
conda env create --name keras --file=/yml_files/keras_env.yml
```

4. Create a data directory, and download the data

```bash
mkdir /scratch/jw6254/unziptest
cd /scratch/jw6254/unziptest
wget https://os.unil.cloud.switch.ch/fma/fma_small.zip
unzip fma_small.zip
```
May need to use p7zip to unzip fma_small.zip

### Cleaning Data and Running Network 
Two different yml files are provided. If you follow the instructions to download the conda environements, the environement music is meant to run [convert_mp3_wav.ipynb](https://github.com/jawooson/deep-learning-final/blob/master/convert_mp3_wav.ipynb) and the environment keras is meant to run [batching _and_network.ipynb](https://github.com/jawooson/deep-learning-final/blob/master/batching_and_network.ipynb)

