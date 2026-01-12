* Author: [[Lukas Böckelmann]]
* Supervisors: [[Matthias Vigl]], [[Lukas Heinrich]], [[Michael Kagan]]

Particle physics has established the Standard Model (SM) as a highly successful theory
that describes fundamental particles and their interactions, yet it leaves many essential
questions unanswered. The quest to understand the limits of the SM and seek new phys-
ical phenomena beyond the SM is supported by the enormous data samples generated
by proton-proton collisions at the Large Hadron Collider (LHC). Reconstruction of these
collisions-events combined with simulation allows for precision measurements through
likelihood methods. Due to difficulties in directly computing likelihood functions, tradi-
tional analysis pipelines in high-energy physics (HEP) separate the reconstruction into
multiple sections. This work adopts a foundation-model perspective from previous re-
search to show the potential for joint optimization of the entire pipeline.
The thesis continues the work on a masked particle modeling (MPM) technique for jets,
taking inspiration from masked, transformer-based autoencoders in natural language and
computer vision tasks, with the goal of producing large foundation models through self-
supervised pretraining and finetuning to multiple downstream tasks. Through compre-
hensive experiments on simulated jet data, this work confirms that masking a portion of
jet constituents and reconstructing their features allows models to learn detailed latent
representations of jets, which significantly improve performance on downstream tasks, in
particular in areas with limited labeled data.

Key findings in this thesis reveal that neural scaling laws reminiscent of those in language
models also emerge in collider-based data applications. Scaling experiments show that
increasing model capacity tends to reduce the validation loss according to approximate
power-law relationships. Although performance gains gradually diminish, systematic
improvements remain evident for higher parameter counts. For dataset size, we observe a
plateau beyond roughly ten million jet samples, suggesting that more complex end-to-end
tasks with richer, full-detector information may be needed to fully exploit the massive
real datasets at the LHC.

The thesis also explores different finetuning methods, including parameter-efficient meth-
ods like LoRA and softprompt, which can closely match or exceed full finetuning while
drastically reducing computational and memory overheads. The results underscore that
the masked modeling paradigm, combined with specific finetuning strategies, can unify
and optimize key stages of jet data analysis, opening up a pathway for future work to
focus on extending these techniques to more complete event reconstructions, as well as
investigating domain shifts between simulated and real detector data. This thesis thus illustrates that self-supervised learning can be successfully adapted to high-energy physics,
offering a scalable and flexible route to improved collider analyses.