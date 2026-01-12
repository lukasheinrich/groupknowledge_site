* Author: [[Bryan Bliewert]]
* Supervisors: [[Lukas Heinrich]], [[Jenny List]]

A top priority of future collider programs is to measure the value of the Higgs self-coupling λ.
Through double Higgs production (ZHH), this is possible by direct measurement at lepton col-
liders. However, both reconstruction and analysis face challenges due to the high number of jets,
misclustering eﬀects in the jet clustering procedure and separation of the signal from irreducible
backgrounds (ZZH). In this thesis, approaches and solutions for both are presented. First, a jet
clustering algorithm based on Graph Neural Networks and Spectral Clustering is presented and
shown to produce nearly identical as the benchmark (Durham algorithm). Then, for the analy-
sis, multiple multivariate methods are explored, such as likelihood-ratio testing with the Matrix-
Element-Method and direct classification using machine learning models including transformers
and Deep Sets. The best results give a final average precision and AUROC for separating ZHH
and ZZH events correctly of 67% and 0.78, respectively.