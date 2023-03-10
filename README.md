# MVD

This is the main branch for the code, data an application associated with the paper titled " MVD: A Novel Benchmark Dataset and Methodology for Robust Acoustic Vehicle Sub-type Classification"

Abstract- Traffic monitoring has emerged as an essential research area for improved traffic management on account of the surging population of urban cities. Acoustic traffic monitoring (ATM) has emerged to be a cost-effective and efficient alternative to more computationally expensive methods of monitoring traffic such as those involving computer vision technologies. In this paper we present MVD and MVDA: two open datasets for the development of acoustic traffic monitoring and  moving vehicle sub-type classification algorithms, which contains audio recordings of moving vehicles. The dataset contain four classes— Trucks, Cars, Motorbikes and a No-vehicle class. Additionally, we propose a novel and efficient way to classify these acoustic signals with great accuracy using cepstrum and spectrum based local and global audio features, and a multi-input neural network. Experimental results show that our methodology improves upon the established baselines on the IDMT-Traffic and IDMT-Augmented datasets and achieves an accuracy of 91.98% and 96.66% on our MVD and MVDA Datasets respectively. Finally, we deploy the proposed model through an Android application to make it accessible for testing and demonstrate its efficacy.   

Link to download the MVD Dataset: https://drive.google.com/drive/folders/1kB-rEWlXDwuIPmEKp_qszpTqWRy_Gtmh?usp=sharing

Link to download the MVDA dataset:

Link to download the MVD app:

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

<img width="1199" alt="AppFin" src="https://user-images.githubusercontent.com/82571294/224412610-1451bedd-bb42-4352-a4ab-732923403f63.png">

