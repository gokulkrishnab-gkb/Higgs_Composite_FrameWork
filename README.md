# Higgs_Composite_FrameWork
This is a project under development , where we deal with the composte higgs framewrok and try to see it's analysis implementation using different algorithms such as BDT,DNN and conventional cut and count
<br/>

Model UFO File. : HC_FormFactor:1.zip <br/>

The model information can be found in the reference : https://arxiv.org/pdf/2105.01093 <br/>

The Model is implemented and UFO is attached HC_FormFactor:1.zip <br/>

To Showcase the analysis , we have created two dataset which is extracted from .root file <br/>
The process which we have studies is P P > Z H , ( Z > l+ l- ) , ( H > b b~ )

*Step 1 :* Extraction of Particle information from the .root file is implemented. The Kinematic variables of our interest are , PT(l+),PT(l-),PT(b),DeltaR(l+,l-),M(l+,l-),M(l+l-bb~) <br/>
The Script will provide the elementary kinematic informations such as Eta,Phi,Px,Py,Pz,E also the single entity derived variable like M and PT <br/>
The Script can be found out in : particle_extract.csv <br/>
save this file inside Delphes/examples and to run this script be in Delphes control terminal. Then follow the following command.<br/>
root -l particle_extract.C' ("/path/to/root/.root")' <br/>

*Step2:* The data needs to be cleaned and , as a first hand information need to plot the histogram of lepton+, lepton- and b-quark transverse momentum to check it's behaviour with the existing 

