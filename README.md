# MVD : Moving Vehicle Detection Dataset

This is the main branch for the code, data an application associated with the paper titled "MVD: A Novel Benchmark Dataset and Methodology for Robust Acoustic Vehicle Sub-type Classification".

Abstract- Traffic monitoring has emerged as an essential research area for improved traffic management on account of the surging population of urban cities. Acoustic traffic monitoring (ATM) has emerged to be a cost-effective and efficient alternative to more computationally expensive methods of monitoring traffic such as those involving computer vision technologies. In this paper we present MVD and MVDA: two open datasets for the development of acoustic traffic monitoring and  moving vehicle sub-type classification algorithms, which contains audio recordings of moving vehicles. The dataset contain four classes— Trucks, Cars, Motorbikes and a No-vehicle class. Additionally, we propose a novel and efficient way to classify these acoustic signals with great accuracy using cepstrum and spectrum based local and global audio features, and a multi-input neural network. Experimental results show that our methodology improves upon the established baselines on the IDMT-Traffic and IDMT-Augmented datasets and achieves an accuracy of 91.98% and 96.66% on our MVD and MVDA Datasets respectively. Finally, we deploy the proposed model through an Android application to make it accessible for testing and demonstrate its efficacy.   

<br>

To replicate the results published in the paper, steps are as follows:
<br>
Step 1 -> Download MVD dataset (or the MVDA dataset) and run code in "MVD feature Extraction.ipynb" to obtain features (in the form of a numpy array) and .csv file.

Step 2 -> Run the "MVD Classifier.ipynb" and insert the path of the features and .csv file obtained from step 1 to replicate results.

<br>
Note- The same code can be used to test the model on other datasets by simply changing the path of the dataset in "MVD feature Extraction.ipynb" and changing the code for extraction of labels depending on the naming structure of the audio samples wherever necessary.

<br>
<br>

Link to download the MVD Dataset: https://drive.google.com/drive/folders/1VhPQAoAWs4TFDOEXauBQIZrCCM4_0qt9?usp=share_link

Link to download the MVDA Dataset: https://drive.google.com/drive/folders/1Uu-Ed0jhHw0s3RHGTYxUqq_olxSucSHJ?usp=share_link

Link to download the MVD Andoid App: https://drive.google.com/drive/folders/15I_krtXQWam1Ulm2rCJtrixcGQxTg_wZ?usp=sharing

The datasets will soon be available on Kaggle.

<br>
<br>

The audios in the datasets have been named as follows:

For MVD:

Example 1 - "Recording_1891_O_C"

Here "1891" is the recording number of a particular microphone and "O" corresponds to the microphone name (the mics are named as follows: "O" ,"A","M" and "H") while "C" is the label {C: car , M: Motorbike , T: truck, N: none}. To uniquely identify a sample, the recording number and microphone name must be used together (in the given example, 1891_O can be used to uniquely identify the sample).

Example 2- "Recording_546_H_T"

Here "546_H" is the recording number + microphone name and can be used to uniquely identify the sample while "T" is the label (truck).

For MVDA:

Example 1 - "Recording_1256A1_A_M"

Here "1256A1" is the recording number + augmentation code (A1: Time stretching , A2: Random gain, A3: Noise Injection) and "A" corresponds to the microphone name (the mics are named as follows: "O" ,"A","M" and "H") while "C" is the label {C: car , M: Motorbike , T: truck, N: none}. To uniquely identify a sample, the recording number, augmentation code and microphone name must be used together (in the given example, "1256A1_A" can be used to uniquely identify the sample).

Example 2 - "Recording_454A3_M_N"

Here "454A3_M" is the recording number + augmentation code (A3: Noise Injection) + "M" corresponds to microphone name and can be used to uniquely identify the sample while "N" is the lable (none).

<br>

<img width="500" alt="AppFin" src="https://user-images.githubusercontent.com/82571294/224412610-1451bedd-bb42-4352-a4ab-732923403f63.png">

Above figure succintly explains working of the MVD Android application. The user has the option of recording a new sample or load an existing one. The app then shows the prediction as well as the confidence score.

Acknowledgements: The authors would like to thank Ashad Naushad (Dept. of CSE, Jamia Hamdard) for his invaluable contribution in the app development process. https://www.linkedin.com/in/ashadnaushad/


