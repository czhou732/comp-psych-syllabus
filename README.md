# Computational Psychiatry: An Undergraduate Syllabus

> **Curated by Peter Zhou** | PRAXIS — Computational Psychiatry at USC
>
> *20 papers across 5 modules. Start at Module 1. Each paper builds on the last.*
>
> **How to use this:** Read papers in order within each module. The study questions guide journal club discussion. Estimated pace: 1 paper/week = one semester.

---

## Module 1: Foundations — What Is Computational Psychiatry?

> *Before you model a disorder, you need to understand what "computational" means in this context — and why psychiatry needs it.*

### 1.1 The Founding Vision
**Montague PR, Dolan RJ, Friston KJ, Dayan P.** (2012). Computational psychiatry. *Trends in Cognitive Sciences*, 16(1), 72–80.

The paper that named the field. Montague and colleagues argue that psychiatric disorders can be understood as "aberrant computations" across biological and cognitive scales. Introduces reinforcement learning and game-theoretic frameworks for modeling clinical behavior.

- **Read this first.** Everything else in the syllabus builds on this paper.
- **Study questions:** What does it mean to call a psychiatric symptom an "aberrant computation"? How is this different from saying it's a "chemical imbalance"?

---

### 1.2 The Bridge to Clinical Applications
**Huys QJM, Maia TV, Frank MJ.** (2016). Computational psychiatry as a bridge from neuroscience to clinical applications. *Nature Neuroscience*, 19, 404–413.

Four years after Montague et al., Huys, Maia, and Frank assess what's actually been accomplished. They map specific computational frameworks (RL, Bayesian inference, dynamical systems) to specific disorders and evaluate the field's progress toward clinical utility.

- **Study questions:** Which computational framework seems most mature for clinical use? Which disorder has the strongest computational evidence base?

---

### 1.3 A Mathematical Framework
**Adams RA, Huys QJM, Roiser JP.** (2016). Computational psychiatry: towards a mathematically informed understanding of mental illness. *Journal of Neurology, Neurosurgery, and Psychiatry*, 87, 53–63.

A more technical companion to Huys et al. Adams and colleagues walk through the math of reinforcement learning (Rescorla-Wagner, temporal difference learning) and predictive coding (Bayesian inference) as applied to depression and schizophrenia.

- **Study questions:** What is a "prediction error" in RL? How does the Bayesian brain framework explain hallucinations?

---

### 1.4 Computational Assays for Psychiatry
**Stephan KE, Mathys C.** (2014). Computational approaches to psychiatry. *Current Opinion in Neurobiology*, 25, 85–92.

Introduces the concept of "computational assays" — standardized modeling procedures that extract clinically meaningful parameters from behavior. Describes the Hierarchical Gaussian Filter (HGF), a generative model that quantifies how individuals update beliefs under uncertainty.

- **Study questions:** What is a "computational assay" and how is it different from a questionnaire? Why does hierarchical inference matter for understanding psychosis?

---

## Module 2: Reinforcement Learning in Psychiatry

> *RL is the workhorse of computational psychiatry. These papers show how reward, punishment, and learning from experience go wrong in depression, addiction, and schizophrenia.*

### 2.1 Reward, Happiness, and the Dopamine Connection
**Rutledge RB, Skandali N, Dayan P, Dolan RJ.** (2014). A computational and neural model of momentary subjective well-being. *Proceedings of the National Academy of Sciences*, 111(33), 12252–12257.

The "happiness equation" paper. Rutledge et al. show that momentary happiness is driven not by absolute reward, but by recent reward prediction errors — the gap between what you expected and what you got. Validated in 18,420 participants via smartphone.

- **Study questions:** If happiness depends on prediction errors, what does that imply about chronically depressed patients? How would anhedonia alter the parameters of this model?

---

### 2.2 Anhedonia and Reward Processing
**Pizzagalli DA.** (2014). Depression, stress, and anhedonia: toward a synthesis and integrated model. *Annual Review of Clinical Psychology*, 10, 393–423.

The definitive review on why depressed patients can't enjoy things. Pizzagalli integrates behavioral, preclinical, and clinical data to argue that stress disrupts mesocorticolimbic dopamine circuits, impairing reward learning, motivation, and hedonic capacity — three dissociable components, not one.

- **Study questions:** What's the difference between "wanting" and "liking" in the context of anhedonia? How does the Probabilistic Reward Task measure reward learning computationally?

---

### 2.3 RL Models of Decision-Making in Clinical Populations
**Maia TV, Frank MJ.** (2011). From reinforcement learning models to psychiatric and neurological disorders. *Nature Neuroscience*, 14(2), 154–162.

Frank and Maia show how specific parameters in RL models (learning rate, exploration-exploitation tradeoff, Go/NoGo balance) map onto specific symptoms in Parkinson's disease, ADHD, schizophrenia, and addiction. The paper that convinced many neuroscientists that computational models have clinical relevance.

- **Study questions:** How does dopamine medication change the learning rate in Parkinson's patients? What would a "high exploration" parameter look like clinically?

---

### 2.4 Effort, Motivation, and Computational Models of Apathy
**Husain M, Roiser JP.** (2018). Neuroscience of apathy and anhedonia: a transdiagnostic approach. *Nature Reviews Neuroscience*, 19(8), 470–484.

Bridges RL models to the clinical reality of apathy — the inability to initiate motivated behavior. Husain and Roiser distinguish apathy from anhedonia and show how effort-based decision-making tasks, modeled computationally, can dissect motivational deficits across depression, Parkinson's, and schizophrenia.

- **Study questions:** How is apathy different from anhedonia? Can a computational model tell them apart when a clinician can't?

---

## Module 3: The Bayesian Brain and Psychosis

> *The "predictive brain" framework offers a radically different explanation for hallucinations, delusions, and psychotic symptoms. These papers lay out the theory and evidence.*

### 3.1 The Predictive Brain
**Clark A.** (2013). Whatever next? Predictive brains, situated agents, and the future of cognitive science. *Behavioral and Brain Sciences*, 36(3), 181–204.

Not a psychiatry paper — but the theoretical foundation for everything in this module. Clark argues that the brain is fundamentally a prediction machine that minimizes surprise. Understanding this framework is prerequisite for understanding computational models of psychosis.

- **Study questions:** What does "prediction error minimization" mean? What happens when the brain's predictions are systematically wrong?

---

### 3.2 Aberrant Precision and Hallucinations
**Corlett PR, Horga G, Fletcher PC, Alderson-Day B, Schmack K, Powers AR III.** (2019). Hallucinations and strong priors. *Trends in Cognitive Sciences*, 23(2), 114–127.

Applies predictive coding to hallucinations. The authors argue that hallucinations arise when the brain assigns too much weight ("precision") to prior beliefs relative to incoming sensory data — you perceive what you expect rather than what's there.

- **Study questions:** If hallucinations are "strong priors," what would a computational treatment intervention look like? How would you test this model experimentally?

---

### 3.3 Computational Models of Delusions
**Corlett PR, Taylor JR, Wang XJ, Fletcher PC, Krystal JH.** (2010). Toward a neurobiology of delusions. *Progress in Neurobiology*, 92(3), 345–369.

Traces delusions to aberrant prediction error signaling — specifically, inappropriately large prediction errors that force belief updating when none is warranted. Connects to dopamine (prediction errors are encoded by dopamine neurons) and explains why antipsychotics (dopamine blockers) reduce delusions.

- **Study questions:** Why would a "noisy" prediction error signal produce delusions rather than random behavior? How does this connect to the dopamine hypothesis of schizophrenia?

---

### 3.4 Computational Phenotyping in Psychosis
**Powers AR, Mathys C, Corlett PR.** (2017). Pavlovian conditioning-induced hallucinations result from overweighting of perceptual priors. *Science*, 357(6351), 596–600.

The landmark experimental test of the "strong priors" theory. Powers et al. used a Pavlovian conditioning task with the HGF model (from Stephan & Mathys, Module 1) to show that people who hallucinate have a measurably different precision-weighting parameter. Published in *Science*.

- **Study questions:** How did the researchers make people hallucinate in the lab? What specific model parameter differed between hallucinators and non-hallucinators?

---

## Module 4: Biomarkers and Classification

> *Can we use brain data + computational models to diagnose, predict, or stratify patients? These papers tackle the promise and pitfalls of neuroimaging-based biomarkers.*

### 4.1 Building Brain-Based Biomarkers
**Woo CW, Chang LJ, Lindquist MA, Wager TD.** (2017). Building better biomarkers: brain models in translational neuroimaging. *Nature Neuroscience*, 20(3), 365–377.

The methodological manifesto for neuroimaging biomarkers. Woo et al. lay out the framework for how multivariate pattern analysis and machine learning should be used to build clinically useful brain signatures — and where the field has gone wrong with circular analyses and overfitting.

- **Study questions:** What is the difference between "prediction" and "inference" in neuroimaging? Why is cross-validation critical for biomarker development?

---

### 4.2 Neuroimaging-Based Subtypes of Depression
**Drysdale AT, Grosenick L, Downar J, Dunlop K, Mansouri F, Meng Y, ... Liston C.** (2017). Resting-state connectivity biomarkers define neurophysiological subtypes of depression. *Nature Medicine*, 23(1), 28–38.

Drysdale et al. used resting-state fMRI from 1,188 patients to identify four neurophysiological subtypes of depression — each with distinct connectivity patterns and different responses to TMS treatment. A landmark paper in precision psychiatry, though subsequent replication efforts have been mixed.

- **Study questions:** Why is it important that depression might have subtypes? What are the risks of building clinical decisions on neuroimaging clusters that may not replicate?

---

### 4.3 Machine Learning in Psychiatry — Promise and Pitfalls
**Dwyer DB, Falkai P, Koutsouleris N.** (2018). Machine learning approaches for clinical psychology and psychiatry. *Annual Review of Clinical Psychology*, 14, 91–118.

A comprehensive and honest review of where ML has succeeded and failed in psychiatric classification. Covers support vector machines, deep learning, and cross-validation methodology. Essential reading before claiming any ML result is "clinically useful."

- **Study questions:** Why do most ML classifiers for psychiatric diagnosis fail to generalize to new samples? What methodological standards should the field adopt?

---

### 4.4 Digital Phenotyping — Smartphones as Sensors
**Torous J, Kiang MV, Lorme J, Onnela JP.** (2016). New tools for new research in psychiatry: a scalable and customizable platform to empower data-driven smartphone research. *JMIR Mental Health*, 3(2), e16.

Introduces the concept of "digital phenotyping" — using passive smartphone data (GPS, accelerometer, call/text logs, screen time) to continuously monitor psychiatric symptoms. Torous et al. present the mindLAMP platform and discuss how digital data streams complement traditional clinical assessment.

- **Study questions:** What behavioral signals can a smartphone capture that a clinician can't? What are the privacy implications of continuous psychiatric monitoring?

---

## Module 5: Ethics, Equity, and Clinical Translation

> *The field's hardest questions. Computational psychiatry can't succeed without confronting bias, consent, access, and the limits of algorithmic medicine.*

### 5.1 The Clinical Translation Gap
**Paulus MP, Huys QJM, Maia TV.** (2016). A roadmap for the development of applied computational psychiatry. *Biological Psychiatry: Cognitive Neuroscience and Neuroimaging*, 1(5), 386–392.

A pragmatic roadmap for moving computational models from research papers to clinical tools. Paulus, Huys, and Maia identify the key bottlenecks: lack of prospective clinical trials, absence of regulatory frameworks, and insufficient communication between modelers and clinicians.

- **Study questions:** What would it take for a computational model to be approved as a clinical diagnostic tool? Who needs to be in the room for that to happen?

---

### 5.2 Ethics of Algorithmic Psychiatry
**Starke G, De Clercq E, Borgwardt S, Elger BS.** (2020). Computing schizophrenia: ethical challenges for machine learning in psychiatry. *Psychological Medicine*, 51(15), 2515–2521.

Confronts the ethical dimensions head-on. When an algorithm predicts psychosis risk, who bears responsibility for false positives? How do we handle the stigma of a "predicted" diagnosis? What happens when training data reflects the biases of the psychiatric system that generated it?

- **Study questions:** Should a patient be told their algorithm predicts a 70% chance of developing schizophrenia? What are the ethical differences between a human and an algorithmic diagnosis?

---

### 5.3 Bias, Fairness, and Representation
**Obermeyer Z, Powers B, Vogeli C, Mullainathan S.** (2019). Dissecting racial bias in an algorithm used to manage the health of populations. *Science*, 366(6464), 447–453.

Not a psychiatry paper — but arguably the most important paper in this syllabus. Obermeyer et al. show that a widely used healthcare algorithm systematically underestimated the health needs of Black patients because it used healthcare spending (biased by access disparities) as a proxy for illness. The same risks exist in every computational psychiatry model trained on clinical data.

- **Study questions:** How could the bias Obermeyer identified manifest in a computational psychiatry tool? What would a "fair" algorithm for psychiatric diagnosis look like?

---

### 5.4 The Future: Where Is the Field Going?
**Gu X, Duman RS.** (2022). Toward a transdiagnostic computational approach in psychiatry. *Biological Psychiatry*, 91(1), 1–3.

An editorial from Xiaosi Gu (your CPC host and #1 target PI) on the future of the field. Gu argues for transdiagnostic approaches — modeling processes (reward, prediction, control) rather than DSM categories. Short, forward-looking, and written by the person who will likely define the field's next decade.

- **Study questions:** What does "transdiagnostic" mean and why does it matter for computational models? How does this vision connect to NIMH's RDoC framework?

---

## Supplementary Resources

### Textbooks
- **Computational Psychiatry: New Perspectives on Mental Illness** — Redish & Gordon, eds. (2016). MIT Press. The first textbook in the field.
- **An Introduction to Model-Based Cognitive Neuroscience** — Forstmann & Wagenmakers, eds. (2015). Springer. For the mathematical foundations.

### Online Courses
- **Neuromatch Academy — Computational Neuroscience** (free, annual summer school)
- **Coursera — Computational Neuroscience** (University of Washington)
- **OITE/FAES courses at NIH** (for trainees on the Bethesda campus)

### Conferences
- **Computational Psychiatry Conference (CPC)** — cpconf.org
- **Society for Biological Psychiatry (SOBP)** — annual meeting
- **Society for Neuroscience (SfN)** — nanosymposia in computational psychiatry track

### Key Journals
- *Computational Psychiatry* (Editor-in-Chief: Xiaosi Gu)
- *Biological Psychiatry: Cognitive Neuroscience and Neuroimaging*
- *Nature Neuroscience*
- *PNAS*

---

## How to Contribute

This syllabus is a living document. If you think a paper should be added, replaced, or reordered, open an issue or submit a pull request.

**Curated by Peter Zhou** — Founder, PRAXIS: Computational Psychiatry at USC | NIH Summer Intern, NIMH ETPB

*Last updated: June 2026*
