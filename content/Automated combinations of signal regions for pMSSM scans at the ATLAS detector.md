Author: [[Leon Renn]]

One of the biggest accomplishments of the Large Hadron Collider (LHC) at CERN was to
find the Higgs particle that concluded the search for elementary particles in the Standard
Model (SM). However, the mass of the Higgs particle does not follow the principles of the
SM itself. Hence, there must be physics behind the SM (BSM). One of the theories that
elegantly solves the Higgs mass problem is Supersymmetry (SUSY). SUSY introduces
supersymmetric partners to the already known particles from SM. This theory must be
broken, since no superpartners at the same mass as SM particles have been found. The
phenomenological Minimal Super Symmetric Model (pMSSM) contains 19 free parameters
describing the masses of supersymmetric partners. Hundreds of analyses have been made
to find SUSY particles at the LHC. However, no SUSY particle has been found yet. These
analyses range from diﬀerent types of decays such as electroweak (EWK), strong (QCD),
etc. to varying quantities of particles and physical phenomenons such as leptons, jets,
etc. When summarizing the results from all analyses, the most sensitive one is taken
and used to increase the exclusion regions for potential SUSY particles. This approach is
however not optimal since information from all other analyses is not used. Nevertheless,
trying to combine analyses eﬀectively is an enormous task that scales quadratically with
the number of analyses. In my thesis, a way is presented to combine a huge number of
analyses in an automated way by first identifying statistically uncorrelated analyses in
an overlap matrix and then using a highest sensitivity path algorithm to eﬃciently find
the best combination. In the scope of this thesis, the implementation of the combination
procedure into the pMSSM analysis framework is described based on the TACO (Testing
Analyses’ Correlations) algorithm. A global overlap matrix is generated from data of the
EWK scan. The estimation of the overlap matrix is validated and used to generate model
point wise combinations for 6307 points of the EWK sector. Improvements in the exclusion
limits are found for the vast majority (>99.92%) of model points. Additionally, 442 model
points are found to be excluded and additional 636 model points are now in the range
of exclusion by running a computational expensive simulation and reconstruction. The
integration of more regions is motivated and the testing of the conceptually introduced
AL (Active Learning) is suggested to be able to sample events eﬃciently for combinations
of analyses.