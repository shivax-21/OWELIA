![Image](https://github.com/user-attachments/assets/1c4c86dc-0eb3-4998-9960-feb32a5535b3)
# OWELIA - Ovarian Wellness & Early Learning AI
Prediction of Polycystic Ovary Syndrome (PCOS) Using Optimized Machine Learning Classifiers
# Introduction

**Problem Statement**: Polycystic Ovary Syndrome (PCOS) is a common hormonal disorder affecting individuals of reproductive age, often leading to complications like irregular periods, infertility, metabolic issues and the most common cause of anovulatory infertility; ∼90–95% of anovulatory women seeking treatment for infertility have PCOS. So, an early detection of PCOS can help in timely medical intervention and lifestyle management.

**Solution**: OWELIA, an especially trained AI model leverages machine learning techniques to develop an early stage detection of PCOS using medical and lifestyle data. By analyzing key health indicators, the model aims to provide an efficient and data-driven approach to assist healthcare professionals in diagnosing PCOS accurately.

## Global trends in PCOS, National Institutes of Health (NIH) article, Januaury 9, 2023 
![Image](https://github.com/user-attachments/assets/a728d616-e449-4ec6-8f50-0f0485a8d725)

A world map displaying the contribution of each country to PCOS research based on publication counts: the darker the color, the more publications, as shown at the bottom left.

To learn more, follow this <a href="https://www.ncbi.nlm.nih.gov/core/lw/2.0/html/tileshop_pmc/tileshop_pmc_inline.html?title=Click%20on%20image%20to%20zoom&p=PMC3&id=9868474_fendo-13-1027945-g002.jpg">Link</a>
## How PCOS changes one's life!!!
### My Life with PCOS: A Real-Life Story, The National Infertility Association article, September 16, 2019
**Sasha Ottey is the founder and executive director of PCOS Challenge: The National Polycystic Ovary Syndrome Association, the leading patient support and advocacy organisation for women and girls with PCOS**,  sharing how once she got diagnosed with PCOS after two decades of having it,

I was diagnosed with PCOS in my late 20s after missing a period and visiting my ObGYN. Despite clear symptoms since adolescence, my diagnosis was delayed due to lack of awareness and missed opportunities by healthcare providers. My doctors offered little guidance—one dismissing my irregular periods and another advising weight loss without support. Frustrated and left to manage on my own.

After doing research, I found out that I had been experiencing PCOS symptoms such as hair loss and weight gain since adolescence. Looking back at my history, I found that there were many missed opportunities for an earlier diagnosis, but due to my own lack of awareness about PCOS, and various specialists not asking the right questions, I was diagnosed almost two decades after the onset of symptoms.

This story clearly shows that early awareness and detection of PCOS are the biggest needs for the women having it, without knowing, so that with the clear diagnosis and advised medication, they can help them to reverse PCOS. Indeed, people like Shasha are there to help those who are in need.

# Getting Started 
> [!IMPORTANT]  
> The model requires Internet connection and internal memory to run properly on jupyter notebook or else you can use google collab.
## Dataset 
To download your dataset from Kaggle, click [here](https://www.kaggle.com/datasets/prasoonkottarathil/polycystic-ovary-syndrome-pcos).
## Run SetUp
- To run the model on google collab without dowloading it, follow these steps:
1. Go to Kaggle: https://www.kaggle.com/datasets/prasoonkottarathil/polycystic-ovary-syndrome-pcos
2. Click on your profile picture (top right) > Account.
3. Scroll down to the API section and click **Create New API Token**.
4. This will download a file named **kaggle.json**.
- Create a google collab notebook and Run these steps:
5. Upload your kaggle.json file.
6. Run the following codes in the code cell.
```bash
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
 ```
7. A ,json file will appear on the file section Copy path of the kaggle.json file, and replace it in the code below after the word (download).
```bash
!kaggle datasets download prasoonkottarathil/polycystic-ovary-syndrome-pcos
 ```
8. A .zip file will appear on the file section, copy the path and paste it in the code below to get the csv file. 
```bash
import zipfile
zip_ref = zipfile.ZipFile('/content/polycystic-ovary-syndrome-pcos.zip', 'r')
zip_ref.extractall('/content')
zip_ref.close()
 ```

<table style="width: 100%;">
  <tr>
    <p>➡ These are the step to step guide for better understanding. </p>
    <td>
      <img src="![Image](https://github.com/user-attachments/assets/ff2e7272-40af-47ea-a85b-7618ee1379c0)" alt="Image 1" style="width: 100%;">
    </td>
    <td>
      <img src="https://i.postimg.cc/vHxGjKN7/image.png" alt="Image 8" style="width: 100%;">
    </td>
  </tr>
  <tr> 
    <td style="text-align: center;">
      <img src="https://i.postimg.cc/jjx0s3ZF/image.png" alt="Image 2" style="width: 100%;">  
    </td>
    <td style="text-align: center;">
      <img src="https://i.postimg.cc/xd1fsdD8/image.png" alt="Image 3" style="width: 100%;">
    </td>
  </tr>
  <tr>




 
