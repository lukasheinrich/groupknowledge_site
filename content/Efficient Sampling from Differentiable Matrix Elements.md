Author: [[Annalena Kofler]]

Generating high quality events from non-trivial, high-dimensional distributions is essential in
various physics fields such as High Energy Physics (HEP). Since significantly more particle
collisions will be measured in the coming years, more simulated events have to be produced
from matrix elements. As standard Monte Carlo (MC) methods might not provide the required
computational speed up, Machine Learning (ML) approaches such as normalizing flows can
be employed as efficient surrogate models of standard generators. Different ways of training
normalizing flows exist and the most promising approaches are compared in this thesis. The
standard training method is based on a training data set that was generated beforehand by
some MC method. If the generation of events is expensive or results in low-quality samples,
this approach is not the best choice. The second method is based on the efficient generation
of samples from the normalizing flow which are evaluated on the distribution of the selected
matrix element. For this type of training, the gradients have to be propagated through the target
distribution requiring a differentiable matrix element calculation provided by implementations
such as ComPWA or MadJax. The third training approach is called Flow Annealed Importance
Sampling Bootstrap (FAB) and relies on samples from the flow as well. These samples are passed through an Annealed Importance Sampling (AIS) sequence that results in samples with a lower importance weight variance. A prioritized replay buffer can be utilized to reduce the number of target evaluations. In this thesis, the mentioned training methods are compared on five different matrix elements of increasing complexity, starting from a two-dimensional phase space to the full 14-dimensional phase space of t¯t-production. It is observed that the normalizing flows outperform the baseline method pyvegas. The flow based on differentiable matrix elements shows similar final results as training FAB without the prioritized replay buffer. Including the buffer increases the performance of FAB, but becomes unstable in higher dimensions. To the best of the author’s knowledge, this is the first account where successful training with differentiable matrix elements was shown without pre-training on samples or aiding the training with such events. When comparing the different training approaches in terms of the number of target evaluations that are required to reach a specific performance, this method shows the best results in high dimensions.