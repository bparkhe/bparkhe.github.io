## Semiconductor Etch Fault Detection

**Project description:** 
The aim of the project was to use statistical methods to detect faults in a semi condutor etching process.
A synthetic dataset was aquired from a LAM 9600 Metal Etcher over the course of etching 129 wafers [Dataaset](http://www.eigenvector.com/data/Etch/)
The experiments were run several weeks apart and data from different experiments has a different mean and somewhat different covariance structure. 108 wafers were normal and 21 wafers had induced faults.

**Principal components analysis**
<br>To segregate the data according to the experiments, principal component analysis was performed on the dataset. Below methods show the variabels in this process. 
<img src="images/semi_etch/classification.PNG?raw=true"/>

A visual feedback of PCA can be obtained by selcting the top 2 principal components for each experiment to obtaina 2d plot. As we can see from the data below that unfolding the variables accross all availble data gives us a significant grouping pattern. This shows that the preprocessed of the data has been performed well.
<img src="images/semi_etch/pca_all.PNG?raw=true"/>

An average across wafers for the unfloded data allows us to check individually the classification and the actual label of the data. As we can see from the below plots, the data is classified accurately according to the respectice experiments. This would aid us in having individual fault charecteristics for each group of data.
<img src="images/semi_etch/pca_avg.PNG?raw=true"/>

**Hotelling's T-square Method**
<img src="images/semi_etch/hot_t2_eq.PNG?raw=true"/>


<img src="images/semi_etch/hotelling_t2.PNG?raw=true"/>



**Error analysis**
<img src="images/semi_etch/error_analysis.PNG?raw=true"/>



**Report**
Here is the report as presented towards the end of the course
[Semi Conductor Etch Classification - Final Presentation](/pdf/etch_fault_ppt.pdf)
