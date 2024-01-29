# Semi-Quantitative Group Testing for Efficient and Accurate qPCR Screening of Pathogens with a Wide Range of Loads

Background: Pathogenic infections pose a significant threat to global health, affecting millions
of people every year and presenting substantial challenges to healthcare systems worldwide.
Efficient and timely testing plays a critical role in disease control and transmission prevention.
Group testing is a well-established method for reducing the number of tests needed to screen
large populations when the disease prevalence is low. However, it does not fully utilize the
quantitative information provided by qPCR methods, nor is it able to accommodate a wide range
of pathogen loads.
Results: To address these issues, we introduce a novel adaptive semi-quantitative group testing
(SQGT) scheme to efficiently screen populations via two-stage qPCR testing. The SQGT method
quantizes cycle threshold (Ct) values into multiple bins, leveraging the information from the
first stage of screening to improve the detection sensitivity. Dynamic Ct threshold adjustments
mitigate dilution effects and enhance test accuracy. Comparisons with traditional binary outcome
GT methods show that SQGT reduces the number of tests by 24% on the only complete real-
world qPCR group testing dataset from Israel, while maintaining a negligible false negative rate.
Conclusion: In conclusion, our adaptive SQGT approach, utilizing qPCR data and dynamic
threshold adjustments, offers a promising solution for efficient population screening. With a
reduction in the number of tests and minimal false negatives, SQGT holds potential to enhance
disease control and testing strategies on a global scale.

## Required packages
* pandas
* numpy
* scipy
* matplotlib
* sklearn

## Downloading the data
The data for our simulations come from  (Barak et al., 2021) and (Jones et al., 2021). You can also download the data from our Google Drive folder: https://drive.google.com/drive/folders/1Xn7iAHW9alDlbCaaNRNq-EBdQ5Q9cr6J?usp=sharing

## Notebooks

This repository contains three different notebooks:
* errorFreePCR.ipynb: This notebook contains simulations for individual testing, Dorfman's GT and SQGT under the assumption that PCR tests are error free. The data that underlies this simulation comes from Barak, Netta, et al. "Lessons from applied large-scale pooling of 133,816 SARS-CoV-2 RT-PCR tests." Science Translational Medicine 13.589 (2021): eabf2823.
* noisyPCR.ipynb: This notebook contains simulations for the same three testing schemes but with the assumption that PCR tests sometimes include false negatives with a false negative rate as described in the Controlling and Modelling FNRs of PCR Tests section of the paper.
* noisyPCR_science.ipynb: This notebook performes the same simulation as noisyPCR.ipynb. However, it is done using data from Jones, Terry C., et al. "Estimating infectiousness throughout SARS-CoV-2 infection course." Science 373.6551 (2021): eabi5273.