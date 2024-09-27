# Higgs Composite Framework

This project is a work in progress, focusing on the composite Higgs framework. The goal is to analyze and implement different algorithms such as BDT, DNN, and the traditional cut-and-count method for the process.
<br/><br/>

**Model UFO File:** <a href="#">HC_FormFactor:1.zip</a><br/>
For more information on the model, refer to the following paper: <a href="https://arxiv.org/pdf/2105.01093" target="_blank">arXiv:2105.01093</a>.<br/>
The model is implemented, and the UFO file is included in `HC_FormFactor:1.zip`.
<br/><br/>

**Process Overview:**<br/>
We are studying the process <b>pp &rarr; ZH</b>, where <b>Z &rarr; l⁺l⁻</b> and <b>H &rarr; bb̅</b>.
<br/><br/>

## Step 1: Extracting Particle Information
The extraction of particle information from the `.root` file is implemented. The kinematic variables of interest include `PT(l⁺)`, `PT(l⁻)`, `PT(b)`, `ΔR(l⁺, l⁻)`, `M(l⁺l⁻)`, and `M(l⁺l⁻bb̅)`.  
The script provides elementary kinematic information such as `Eta`, `Phi`, `Px`, `Py`, `Pz`, `E`, as well as derived variables like `M` and `PT`.<br/>
The script can be found in: `particle_extract.csv`.<br/>
To run this script, place it inside `Delphes/examples` and use the following command from the Delphes terminal:<br/>
<code>root -l 'particle_extract.C("/path/to/root/.root")'</code>
<br/><br/>

## Step 2: Data Cleaning and Visualization
The data needs to be cleaned, and as an initial step, histograms of `lepton⁺`, `lepton⁻`, and `b-quark` transverse momentum should be plotted to check their behavior in comparison to existing studies.<br/>
The cleaning process and histogram plots can be found in: `data_organisation.ipynb`.
<br/><br/>

## Step 3: Correlation and Mutual Information
From the cleaned data, four key variables—`Eta`, `Phi`, `PT`, and `Pz`—are required to calculate the correlation matrix and mutual information among the variables.<br/>
To extract this data and save it to a new CSV file, continue using `data_organisation.ipynb`. In the latter part of the notebook, the correlation matrix and mutual information matrix are also computed.


just like you did it for bp1_markers = {
    'M1': (-66.68, 89.68),
    'M2': (-16.50, 64.59),
    'M3': (18.71, 46.98),
    'M4': (53.73, 29.47)
}

i have bp2_marker ,bp3_marker etc upto bp_10marker. I need to include all of that.

also i need to print out at the end a table with coloums BP1,BP2,BP3,BP4 etc.. upto BP10
with row 1 corrsponds to M1 coordinates
row 2 for M2 coordinates
row 3 for M3 coordinates
row 4 for M4 coordinates

the information regarding other markers

 bp2_markers = {
    'M1': (-66.68, 41.04),
    'M2': (, 64.59),
    'M3': (18.71, 46.98),
    'M4': (53.73, 29.47)
}
