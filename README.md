# A Multiscale Recurrent Neural Network Model forLong-Term Prediction of Geothermal Reservoir Energy Production

Optimization of energy production from geothermal reservoirs relies on the reliable prediction of energy production performance under alternative development scenarios. Data-driven predictive models can serve as efficient alternatives, which provide rapid evaluation and screening of alternative production and development plans as well as facilitating daily operation and surveillance decisions. We evaluate the use of recurrent neural networks (RNN), as machine learning architectures for the representation and prediction of sequential/dynamic data, for the long-term prediction of brine enthalpy from the geothermal reservoir. RNN primarily exploits statistical relations in training data to generate predictions. Thus it can be challenging to apply RNN in applications where the extrapolation beyond the training data range is needed. In addition, geothermal data usually involves features on multiple scales, which makes complex deep learning models more vulnerable to overfitting. To overcome these issues, we have developed a multiscale architecture for RNN to improve its generalization power for the long-term prediction of geothermal data. The long-term model in the multiscale structure is designed to only capture the smooth low-frequency patterns. The rest features that have a higher frequency and are more nonlinear are picked up by a short-term model. The final prediction is the addition of the long-term and short-term predictions. We have evaluated multiscale RNN on both synthetic and field data. The accuracy is compared against RNN and autoregressive models (AR). The results suggest that the multiscale architecture can improves the long-term prediction and makes the model more resistant to noise. 

<p align="center">
<img src="https://github.com/AnyueJ/Geothermal_Multiscale/blob/main/Image/Figure4.png" width="722" height="440">
</p>

## Prerequisites
Python 3.8.8

Tensorflow 2.3.0

## Data
Due to the data confidentiality, we are not allowed to share the field examples that were used in our paper. Only the synthetic examples are available in this repo

## Citation
@inproceedings{jiang2022multiscale,
  title={A Multiscale Recurrent Neural Network Model for Long-Term Prediction of Geothermal Energy Production},
  author={Jiang, Anyue and Qin, Zhen and Cladouhos, Trenton T and Faulder, Dave and Jafarpour, Behnam},
  booktitle={47th Workshop on Geothermal Reservoir Engineering Stanford University, Stanford, California},
  pages={1--8},
  year={2022}
}

## Acknowledgments
This material is based upon work supported by the U.S. Department of Energy's Office of Energy Efficiency and Renewable Energy (EERE) under the Geothermal Technologies Office award number DE-EE0008765. The authors acknowledge the Energi Simulation support of the Center for Reservoir Characterization and Forecasting at USC.
