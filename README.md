# BSTE-dataset
The revised simulated dataset and the associated files required to generate simulated data has been updated in ["Simulated Data for bangali text localisation in natural image", Sourav saha, Md Easin Arafat, Md Aminul Haque Palash, Faria Afrin, Md Dewan Farid, M Shamim Kaiser](https://data.mendeley.com/datasets/h9kry9y46s/3)



** simulated text-localization Image Samples **
![simulated text-localization Image Samples](images/srnet_github.drawio.png "Simulated image")

## INSTALLATION

At first create a conda environment. We choose ```bste_dataset``` as the name of the environment. 

```
conda create -n bste_dataset python==3.9.0
conda activate bste_dataset
pip install -r requirements.txt
```
## Data Generation 
To generate data need to maintain few files. In the table below illustrating the file formatting.
first download the ```Source Dataset.zip``` file from this [Link](https://data.mendeley.com/datasets/h9kry9y46s/3). Then create a file in the root of this repo named ```utils```. 

| path                 | Source Dataset                            | 
| :------------------  |    :---------------------------------------:       
| ```utils/text```     | unzip ```text.zip``` and copy only text folder         | 
| ```utils/fonts```    | unzip ```fonts.zip``` and copy only fonts folder       |       
|```utils/background```| Unzip ```background.zip``` and copy only backgraound folder    |
|```utils/colors.cp``` | Unzip ```color.zip``` and copy only colors folder     |

Now just run ```python datagen.py```
