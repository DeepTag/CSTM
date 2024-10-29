# CSTM
This is the project page of the WACV 2025 paper CSTM.

## Continuous Spatio-Temporal Memory Networks for 4D Cardiac Cine MRI Segmentation.
We propose a continuous spatio-temporal memory (CSTM) network for semi-supervised whole heart and whole sequence cardiac cine MRI segmentation. Our CSTM network takes full advantage of the spatial, scale, temporal and through-plane continuity prior of the underlying heart anatomy structures, to achieve accurate and fast 4D segmentation.
<div align=center><img width="820" height="406" src="https://github.com/DeepTag/CSTM/blob/main/cstm.png"/><img width="820" height="406" src="https://github.com/DeepTag/CSTM/blob/main/cstm.png"/></div>

## Demo
We aim to register an untagged cine MR (cMR) image to a tagged MR (tMR) image. The non-smooth contrast change between tMR and cMR, i.e., presence of tags, poses a great challenge to this task. We use the proposed method to first translate tMR to fake cMR; then, we register cMR to fake cMR using the NCC-based dissimilarity loss. Our method can learn the **specific image style** of each cMR frame to be registered and boost the multi-modal registration performance significantly. Note how the fake cMR frames can capture the individual image styles of the corresponding real cMR frames.  
<div align=center><img width="185" height="231" src="https://github.com/DeepTag/CSTM/blob/main/patient109_0.gif"/></div>

[**upper**] tMR and unregistered cMR sequence; [**middle**] tMR and fake cMR sequence; [**bottom**] tMR and registered cMR sequence. 

## Acknowledgments
Our code implementation borrows heavily from [STCN](https://github.com/hkchengrex/STCN).
