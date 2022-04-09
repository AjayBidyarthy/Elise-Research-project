# Elise-Research-project

#### The links for all the models:

### Base model (Risk neutral, Deterministic):    
https://colab.research.google.com/drive/1PmFu4ag0u-NyT3VuozFW7SLzySX3IUt7
### Base model (Risk neutral, softmax):          
https://colab.research.google.com/drive/1KY-ka-OCxh9041ljZgDk3am7zDkpfoUT
### Base model (prospect theory, Deterministic): 
https://colab.research.google.com/drive/1VGiiu2DhEdwVbodbJ39R-5HkjUvaT6uG#scrollTo=s3d5eXUPhCbk
### Base model (prospect theory, softmax):        
https://colab.research.google.com/drive/18EwjnBz0eb6jYY5sp28JWcWYmTLGttSx#scrollTo=u_lMk7H0dEMb
### Base model with Gambler's Fallacy:           
https://colab.research.google.com/drive/1D7tC_xfKbl2bHJWqD_Tx_vNGA4VGTEQO#scrollTo=1fjX2jxWyl67
### Base model augmented with CbD (Risk neutral, Deterministic):     
https://colab.research.google.com/drive/1Tbn_-kuHqtI-GY_zJtBpEVB8o4YScOgt#scrollTo=p_5RB0lxTzER
### Base model augmented with CbD (Risk neutral, softmax):           
https://colab.research.google.com/drive/1D7tC_xfKbl2bHJWqD_Tx_vNGA4VGTEQO  
### Base model augmented with CbD (prospect theory, Deterministic): 
https://colab.research.google.com/drive/1xq-PNAiFLNn3YvDMVlzU41dEmHPFcKda
### Base model augmented with CbD (prospect thoery, softmax):       
https://colab.research.google.com/drive/1JNYxjhVVdtVgYyk74zhbYQYhtm8Fhq9i
### Base model augmented with CbD (modified probability function, Risk neutral, softmax):  
https://colab.research.google.com/drive/1SPueKt7STUlSWRJyFl7Rh0VlqrY_EGNt
### Base model with CbD(Risk neutral,Deterministic,multiplicative):     
https://colab.research.google.com/drive/1cu5LVgnAqIZ3_E-RCG--ckQrRmCl60gk#scrollTo=HEdAMHXFQ3B4
### Base model with CbD model (Prospect theory,Deterministic, same alphas): 
https://colab.research.google.com/drive/1j17U27bnjx8BLrCHe6Hk6GJ2ewXVZRch#scrollTo=u_lMk7H0dEMb

----------------------------------------
### Pre-Requisites

For any given dataset, User needs to run all the cells in a model (in respective order) to get the results.

Parameter optimization and obtaining results are seperate parts in each model:

1. One can look at the output of the hyperparameter optimization step in a code to get the values of all the free parameters.

2. The results for a dataset (accuracy score of a particular model in %) can be obtained from the output of the bottom-most code cell. 

In some datasets, the 'betting column' (whether or not the subject chooses to bet, denoted by 1 or 0 respectively) is col.No.4 and in some datasets, it is col.No.5, so while training 
the model, variable 'Y' (which is actually the betting column) needs to be changed (to df[4] or df[5]) depending on datasets.

User needs to change the drive link in each code to whatever is the location of dataset.

In CbD models, n-value of 4 is used, meaning that DA is zero for any trial t such that 1<= t <= 4

There are no seperate codes for the varying n-value test (as everything is exactly the same except for n-value), so user may change the value of n in the CbD model 
(Prospect theory, Deterministic) code for that test.
