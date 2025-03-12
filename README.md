<td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/Owelia.png"></td>

# OWELIA - Ovarian Wellness & Early Learning AI
Prediction of Polycystic Ovary Syndrome (PCOS) Using Optimized Machine Learning Classifiers
# Introduction

**Problem Statement**: Polycystic Ovary Syndrome (PCOS) is a common hormonal disorder affecting individuals of reproductive age, often leading to complications like irregular periods, infertility, metabolic issues and the most common cause of anovulatory infertility; ∼90–95% of anovulatory women seeking treatment for infertility have PCOS. So, an early detection of PCOS can help in timely medical intervention and lifestyle management.

**Solution**: OWELIA, an especially trained AI model leverages machine learning techniques to develop an early stage detection of PCOS using medical and lifestyle data. By analyzing key health indicators, the model aims to provide an efficient and data-driven approach to assist healthcare professionals in diagnosing PCOS accurately.

## Global trends in PCOS, National Institutes of Health (NIH) article, January 9, 2023 
<td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/fendo-13-1027945-g002.jpg"></td>
A world map displaying the contribution of each country to PCOS research based on publication counts: the darker the color, the more publications, as shown at the bottom left.

To learn more, follow this <a href="https://www.ncbi.nlm.nih.gov/core/lw/2.0/html/tileshop_pmc/tileshop_pmc_inline.html?title=Click%20on%20image%20to%20zoom&p=PMC3&id=9868474_fendo-13-1027945-g002.jpg">Link</a>
## How PCOS changes one's life!!!
### My Life with PCOS: A Real-Life Story, The National Infertility Association article, September 16, 2019
### Meet SHASHA
<td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/Sasha-Night-of-Hope-Award-landscape.jpg"></td>
Left side lady in the image.

**Sasha Ottey is the founder and executive director of PCOS Challenge: The National Polycystic Ovary Syndrome Association, the leading patient support and advocacy organisation for women and girls with PCOS**,  sharing how once she got diagnosed with PCOS after two decades of having it,

I was diagnosed with PCOS in my late 20s after missing a period and visiting my ObGYN. Despite clear symptoms since adolescence, my diagnosis was delayed due to lack of awareness and missed opportunities by healthcare providers. My doctors offered little guidance—one dismissing my irregular periods and another advising weight loss without support. Frustrated and left to manage on my own.

After doing research, I found out that I had been experiencing PCOS symptoms such as hair loss and weight gain since adolescence. Looking back at my history, I found that there were many missed opportunities for an earlier diagnosis, but due to my own lack of awareness about PCOS, and various specialists not asking the right questions, I was diagnosed almost two decades after the onset of symptoms.

This story clearly shows that early awareness and detection of PCOS are the biggest needs for the women having it, without knowing, so that with the clear diagnosis and advised medication, they can help them to reverse PCOS. Indeed, people like Shasha are there to help those who are in need.

Read about her more from [here](https://resolve.org/my-life-with-pcos-a-personal-story/).
Shasha Ottey [LinkedIn](https://www.linkedin.com/in/pcoschallenge/).

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
7. A .json file will appear on the file section Copy path of the kaggle.json file, and replace it in the code below after the word (download).
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
<table>
    <p>➡ These image guide will help you for better understanding of codes. </p>
  <tr>
    <td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/IMG_20250305_221801.jpg" width="300"></td>
    <td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/IMG_20250305_221815.jpg" width="300"></td>
    <td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/IMG_20250305_221831.jpg" width="300"></td>
  </tr>
   <tr>
    <td><b>Step 1</b><br> Drag and upload json.</td>
    <td><b>Step 2</b><br> Copy paths.</td>
    <td><b>Step 3</b><br> End of steps.</td>
  </tr>
</table>


> [!NOTE]  
> The dataset provided on Kaggle is an Excel file to avoid any bugs, use the CSV file provided inside this repo.

Click [here](https://github.com/shivax-21/OWELIA/tree/main/dataset) to download the raw csv files. 
# Data & Model
<table>
    <p>➡ Data Visuals for understanding. </p>
  <tr>
    <td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/SAVE_20250306_164720.jpg" width="500"></td>
  </tr>
   <tr>
    <td><b>Data Counts</b></td>
  </tr>
</table>

# Classifiers & Results
<table>
    <p>➡ These images will show accuracy accquired by each classifiers. </p>
  <tr>
    <td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/IMG_20250306_172102.jpg" width="300"></td>
    <td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/IMG_20250306_172038.jpg" width="300"></td>
    <td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/IMG_20250306_172151.jpg" width="300"></td>
  </tr>
   <tr>
    <td><b>1. Multi-Layer Perceptron</b><br>~82.41% accuracy</td>
    <td><b>2. Random Forest</b><br>~90.44% accuracy</td>
    <td><b>3. XGBOOST</b><br>~88.9% accuracy</td>
  </tr>
</table>
<table>
    <p>➡ To increase the accuracy futher we will apply SMOTE (Synthetic Minority Over-sampling Technique), synthetically generating new minority class samples and increase our models' accuracy upto 100% .</p>
  <tr>
    <td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/IMG_20250306_172203.jpg" width="300"></td>
    <td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/IMG_20250306_172022.jpg" width="300"></td>
    <td><img src="https://github.com/shivax-21/OWELIA/blob/main/images/IMG_20250306_173637.jpg" width="300"></td>
  </tr>
   <tr>
    <td><b>1. K-Neighbors</b><br>~94.69% accuracy</td>
    <td><b>2. SVC</b><br>~97.35% accuracy</td>
    <td><b>3. Random Forest</b><br>100.00% accuracy</td>
  </tr>
</table>

For a deeper understanding, explore the complete notebook provided [here](https://github.com/shivax-21/OWELIA/blob/main/Notebooks/OWELIA.ipynb). You can also access it on Google Colab by clicking [here](https://colab.research.google.com/drive/1SaSU85mp6_fTOl526uBv2M47gnyJ_oS7?usp=sharing). 

# Conclusion
We explored the prediction of Polycystic Ovary Syndrome (PCOS) using machine learning techniques. By leveraging data preprocessing, feature engineering, and model evaluation, we built a predictive model to assist in early diagnosis and awareness of PCOS.

While our model shows promising results, further improvements can be made by incorporating larger datasets, advanced feature selection, and deep learning approaches. This work serves as a step toward utilizing AI in healthcare and early detection, potentially aiding in better management and timely interventions.

Thank you for exploring this notebook! I hope it contributes to raising awareness and encourages further research in this critical domain. 

# About the Author
I am Shivani Patwa, 2nd year undergraduate from JK Institute of Applied Physics and Technology, University of Allahabad, Prayagaraj, Uttar Pradesh, passionate about leveraging technology to address real-world health challenges, and this PCOS detection project is a step toward making early diagnosis more accessible and efficient. While this model provides valuable insights, I believe there’s always room for improvement.

I warmly welcome researchers, developers, and healthcare professionals to collaborate and enhance this project further. Let’s refine, innovate, and push the boundaries of perfection together! 

Feel free to connect and contribute, every idea counts!





 
