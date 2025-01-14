# Small Animal and Ex Vivo Diffusion
Code, software, and datasets for small animal and ex vivo diffusion MRI

Here, we compile  a list of existing and freely shared small-animl or ex vivo diffusion datasets (**Table 1 and Table 2**), a list  of available software dedicated to image acquisition (**Table 3**), a list of software  available for data pre-processing (**Table 4**), and a list of software available for model fitting (**Table 5**). 

Citation of paper goes here


## Small Animal Datasets

| URL  | Species | Diffusion Scheme | Other features | Institution |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| https://doi.org/10.14264/de9aa47  | Mouse brain  | DTI | Model of Concussion | University of Queensland
| http://cmrm.med.jhmi.edu/ (M. Aggarwal et al. 2009)  | Mouse brain  | Atlas | Johns Hopkins

## Ex Vivo Datasets

| URL  | Species | Diffusion Scheme | Other features | Institution |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| http://www.drcmr.dk/map-datasets  | Mouse brain  | micro-FA, Multi-shell, multi-resolution, Tractography, Axon diameter, Exchange rate, Axon relaxation | Validation: 3D synchrotron imaging of axons, cell bodies, vacoules and vessels, in vivo tracers | Danish Research Center for MR
| https://www.nature.com/articles/sdata201672 | Rat brain, rat spinal cord, human brain | DKI |  | Aarhus University |
| https://doi.org/10.1016/j.dib.2016.08.020 | Rat, pig and human spinal cords | DTI | Ultra-high resolution (MR microscopy) | U of Florida |
| https://doi.org/10.1016/j.dib.2016.06.061 | Rat brain | Multi-shell, high b-value | Mild chronic stress model | Aarhus University |
| https://github.com/sepehrband/AxonDiameter | Mouse brain | Multi-shell  | Augmented with EM data and manually segmented axon diameter | U of Queensland |
| http://cmrm.med.jhmi.edu/ (M. Aggarwal et al. 2009) | Adult and postnatal developing mouse brains |  | Atlas | Johns Hopkins |
| https://doi.org/10.1016/j.neuroscience.2005.07.014  | Mouse brain |  | Atlas | Several |
| http://doc.pmod.com/pneuro/pneuro.html?mousebrainatlasma-benveniste-mirrione4996.html | Cynomolgus, rhesus monkey and pig  |  | Atlas  | PMOD |
| https://osf.io/yp4qg/ (Cohen-Adad et al. 2019)  | White matter axons |  | Microscopy data (non-MR) | Several |
| https://doi.org/10.1016/j.dib.2015.05.019 |Cynomolgus macaque corpus callosum  |  | Microscopy data (non-MR) | Several |
| http://www.duhs.duke.edu/mouseconnectome | Mouse Connectome in Waxholm Space | HARDI @ 43 um, 120 angle, b-value @ 4000 s/mm2 | Segmented Atlas compared to retroviral tracers WHS Labels | Duke CIVM |
| https://civmvoxport.vm.duke.edu/voxbase/login.php?return_url=%2Fvoxbase%2Fstudyhome.php%3Fstudyid%3D754 | Rat Connectome | MGRE @ 25 um HARDI @ 50 um 60 Angles Single specimen Average (n=6)b=3000 s/mm2 |Segmented Atlas includes downloadable application for display | Duke CIVM |
| http://www.civm.duhs.duke.edu/rhesusatlas |Rhesus | MGRE@75um DTI@150 um 12 angles; b value =1500 s/mm2  | Average N=10 241 labels  | Duke CIVM |
| https://civmvoxport.vm.duke.edu/voxbase/login.php?return_url=%2Fvoxbase%2F | Mouse NODDI @ 50 um | 8 shells B value 1000-8000 s/mm2 384 angles |With comparative histology | Duke CIVM |
| Histology: https://www.nitrc.org/projects/smatlas/ Atlas: https://www.nitrc.org/projects/validate29/ | Squirrel monkey atlas + histology | Multi-shell HARDI acquisition | Atlas + histology | Vanderbilt |


## Data acquisition

| Name  | URL | Institution | Features | Dependencies |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Pulse Sequences | https://osf.io/ngu4a/   | University of Wisconsin  Madison | Custom diffusion sequences (for Bruker Consoles) | ParaVision version
| REMMI | https://remmi-toolbox.github.io/  | Vanderbilt University | Sequences for small animal quantitative MRI including diffusion | Paravision or VNMRJversion
| double PFG directions | [https://remmi-toolbox.github.io/](https://cfin.au.dk/cfinmindlab-labs-research-groups/neurophysics/software/)  | Aarhus University | Output pairs of diffusion directions for dPFG | Matlab

## Pre-processing

| Name  | URL | Institution | Features | Dependencies |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| DICOMIFIER  | https://github.com/lamyj/dicomifier  | University of Strasbourg | Conversion Bruker to DCM and NIFTI format (incl. Diffusion information) | Python
| atlasBREX  | https://github.com/jlohmeier/atlasBREX  | Charité Berlin | Non-human brain extraction | FSL, AFNI, ANTs, ABSORB
| PreQual  | https://github.com/MASILab/PreQual  | Vanderbilt | All pre-processing steps | Python
| SCT  | https://spinalcordtoolbox.com/   | Polytechnique Montreal | Spinal cord MRI | Python
| MChepato  | https://github.com/fragrussu/MChepato | Vall d’Hebron Institute of Oncology | Tools for mouse liver dMRI-histology imaging used in (Grussu et al. 2022) | Python, FSL, QuPath, MRItools, DiPy, NiftyReg, and others
| Tractoflow  | https://doi.org/10.1016/j.neuroimage.2020.116889 | Sherbrooked University | End to end tractography (not small animal specific) | 

## Model Fitting
| Name  | URL | Models | Features | Dependencies |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| qMRINet  | https://github.com/fragrussu/qMRINet  | qMRI models | model fitting using fully-connected deep neural networks | NumPy/Nibabel/SciPy/PyTorch
| Fast Kurtosis  | https://cfin.au.dk/cfinmindlab-labs-research-groups/neurophysics/software/  | Kurtosis metrics | kurtosis metrics from reduced diffusion kurtosis imaging data sets | Matlab

