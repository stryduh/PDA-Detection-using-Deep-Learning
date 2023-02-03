# PDA-Detection-using-Deep-Learning
## About the Project
This project aims to use deep learning technologies for the task of detecting Patent Ductus Arteriosus (PDA), a congenital heart defect, in the echocardiograms of infants. The dataset of infant echocardiograms was provided by the Children's Hospital of Orange County (CHOC) and the project was worked on by a team of 4 in conjunction with CHOC. This is the second iteration of this specific project and the purpose is to achieve better performance, i.e. higher accuracy, sensitivity, etc..., than the previous iteration done by CHOC. Multiple convolutional neural networks were selected due to their high performance on other classification tasks using medical data and were trained using transfer learning on the echocardiograms. In particular, MobileNet-V2, EFficientNet B0, EfficientNet B3, and MobileNASNET were picked.
## Technologies Used
- Python
- PyTorch
- Numpy
- scikit-learn
- Nvidia Deep Learning Examples for torchhub
- matplotlib
## Data and Code
As stated previously, this dataset was provided by CHOC and contains echocardiogram frames from multiple infants. As a result, this data will not be shared and only the model code is in this repository. The final report is also provided as a pdf in this respository.
## Results
`Threshold Experiments.ipynb` contains work involving using different classification thresholds in an effort to increase classification metrics for each model. An alpha, beta, and g-means threshold were used for each model as outlined in the report. The model with the best performance as well with one of the best efficiencies was MobileNet-V2 with a 94.4% overall detection accuracy, 91.2% sensitivity, and 97.4% specificity. These were higher than the metrics from the previous iteration of the project done by CHOC by 12%, 15%, and 10% respectively. 
## Future Work
Limitations to hardware limited batch and epoch sizes, which did not allow the MobileNASNET model to converge during training. As a result, with cloud computing services such as AWS, a more thorough training process for MobileNASNET may return even better metrics than the one returned by MobileNet-V2 currently. In addition, time series information could be employed in the future due to the video nature of echocardiogram clips. Additional future work is discussed in the report. 
## References
Previous CHOC work: https://www.sciencedirect.com/science/article/pii/S2666521222000072
