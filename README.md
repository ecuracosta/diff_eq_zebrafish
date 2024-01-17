## Differential Equation Model Analysis

An analysis of a system of differential equations to model the local control of cellular proliferation during organ regeneration in zebrafish. The objective is to fit the model to observed data, estimate parameters and visualize the model predictions with uncertainties.

### Dataset
The dataset used in this analysis consists of Hair, Mantle and Sustentacular cells number as a function of time in days.

### Model

The model is a system of differential equations:

$$
\frac{dH}{dt} = 2 \left(1 - p_{\text{SS}} - p_{\text{MM}} - p_{\text{SM}}\right) \frac{\nu S_{50}^{h} S}{S_{50}^{h} + S^{h}} 
$$

$ \frac{dM}{dt} = \left(2 p_{\text{MM}} + p_{\text{SM}}\right) \frac{\nu S_{50}^{h} S}{S_{50}^{h} + S^{h}} + \frac{2f\nu M_{50}^{h} M}{M_{50}^{h} + M^{h}} $

$ \frac{dS}{dt} = \left(3 p_{\text{SS}} + 2 p_{\text{SM}} - 1\right) \frac{\nu S_{50}^{h} S}{S_{50}^{h} + S^{h}} $

### Methodology
The analysis includes parameter estimation using Approximate Bayesian Computation (ABC), followed by visualization of parameter distributions and model predictions against observed data.
