* Author: [[Dominik Voß]]
* Supervisors: [[Jonas Würzinger]], [[Lukas Heinrich]]

This work aims to improve the sampling efficiency of parameter space exploration in high-
dimensional BSM theory spaces through the application of Active Learning (AL) with Gaus-
sian Processes (GPs). Using this method, contours in the 19D pMSSM parameter space can
be determined more precisely compared to the currently applied random sampling approach.
AL enables the targeted selection of parameter points that provide the highest information
gain, based on the inherent uncertainty estimation of the GPs. As part of this work, an exist-
ing AL selection framework whose acquisition function is specifically designed for the identi-
fication of decision boundaries, is applied on simulated pMSSM data using the dark matter
relic density ΩDMh2 and the cross-section σ as targets. The AL method is first validated on
low-dimensional problems and then extended to the full 19D pMSSM parameter space. The
results show that the AL acquisition strategy can reduce the required number of training sam-
ples by around 50-80 % for the Exact GP and 40-50 % for the Deep GP to reach a targeted
level of accuracy in contour identification, depending on whether the cross-section or the dark
matter relic density is the target. While the Exact GP achieves a stronger overall AL effect, a
Deep GP architecture provides a more accurate modeling of the more complex cross-section
function. Overall, this thesis proves that AL with GPs constitutes a more efficient approach for
the exploration of the 19D pMSSM parameter space compared to the currently used random
sampling approach. Future work could therefore apply AL to refine the exclusion contour
identification within the pMSSM, contributing to the identification of unexpected models and
thus, ultimately, new physics.