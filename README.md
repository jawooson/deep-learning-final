# Neural Network Finger Printer
This project is using my own account with NYU's HPC resources. When creating directory structure, make sure to replace anything with my username jw6254 with your own. 

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
