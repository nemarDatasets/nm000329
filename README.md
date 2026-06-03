[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.nm000329-blue)](https://doi.org/10.82901/nemar.nm000329)

Brandl2020
==========

Motor Imagery under distraction dataset from Brandl and Blankertz 2020.

Dataset Overview
----------------
  Code: Brandl2020
  Paradigm: imagery
  DOI: 10.3389/fnins.2020.566147
  Subjects: 16
  Sessions per subject: 1
  Events: left_hand=1, right_hand=2
  Trial interval: [0, 4.5] s
  Runs per session: 7
  File format: MAT (HDF5 v7.3)

Acquisition
-----------
  Sampling rate: 1000.0 Hz
  Number of channels: 63
  Channel types: eeg=63
  Channel names: AF3, AF4, AF7, AF8, AFz, C1, C2, C3, C4, C5, C6, CP1, CP2, CP3, CP4, CP5, CP6, CPz, Cz, F1, F2, F3, F4, F5, F6, F7, F8, FC1, FC2, FC3, FC4, FC5, FC6, FCz, FT7, FT8, Fp1, Fp2, Fpz, Fz, O1, O2, Oz, P1, P2, P3, P4, P5, P6, P7, P8, PO3, PO4, PO7, PO8, POz, Pz, T7, T8, TP10, TP7, TP8, TP9
  Montage: standard_1005
  Hardware: 2x BrainAmp (Brain Products)
  Software: BBCI Toolbox (MATLAB)
  Reference: nose
  Sensor type: Ag/AgCl wet
  Line frequency: 50.0 Hz
  Cap manufacturer: EasyCap
  Cap model: Fast'n Easy Cap

Participants
------------
  Number of subjects: 16
  Health status: healthy
  Age: mean=26.3
  Gender distribution: female=6, male=10
  BCI experience: mostly naive (3/16 had prior BCI experience)

Experimental Protocol
---------------------
  Paradigm: imagery
  Number of classes: 2
  Class labels: left_hand, right_hand
  Trial duration: 4.5 s
  Tasks: calibration, clean, eyesclosed, news, numbers, flicker, stimulation
  Study design: Motor imagery under distraction: 1 calibration run (no feedback, no distraction) + 6 feedback runs with different distraction conditions (clean, eyes closed, news, number search, flicker, vibro-tactile stimulation)
  Feedback type: auditory
  Stimulus type: auditory
  Stimulus modalities: auditory
  Primary modality: auditory
  Synchronicity: cue-based
  Mode: online
  Training/test split: False
  Instructions: Subjects received auditory cues ('links' for left, 'rechts' for right) and performed motor imagery of left or right hand movement

HED Event Annotations
---------------------
  Schema: HED 8.4.0 | Browse: https://www.hedtags.org/hed-schema-browser

  left_hand
    ├─ Sensory-event, Experimental-stimulus, Visual-presentation
    └─ Agent-action
       └─ Imagine
          ├─ Move
          └─ Left, Hand

  right_hand
    ├─ Sensory-event, Experimental-stimulus, Visual-presentation
    └─ Agent-action
       └─ Imagine
          ├─ Move
          └─ Right, Hand

Paradigm-Specific Parameters
----------------------------
  Detected paradigm: motor_imagery
  Imagery tasks: left_hand, right_hand
  Imagery duration: 4.5 s

Data Structure
--------------
  Trials: 504
  Trials per class: left_hand=252, right_hand=252
  Blocks per session: 7
  Trials context: 7 runs per subject: 1 calibration (72 trials) + 6 feedback runs (72 trials each, 6 distraction conditions)

Preprocessing
-------------
  Data state: raw
  Preprocessing applied: False

Signal Processing
-----------------
  Classifiers: CSP+LDA
  Feature extraction: CSP, bandpower
  Frequency bands: mu=[8.0, 13.0] Hz; beta=[13.0, 30.0] Hz
  Spatial filters: CSP

Cross-Validation
----------------
  Method: holdout
  Evaluation type: within_subject

BCI Application
---------------
  Applications: motor_control
  Environment: laboratory
  Online feedback: True

Tags
----
  Pathology: Healthy
  Modality: Motor
  Type: Motor Imagery

Documentation
-------------
  DOI: 10.3389/fnins.2020.566147
  License: CC-BY-NC-ND-4.0
  Investigators: Stephanie Brandl, Benjamin Blankertz, Tobias Dahne
  Senior author: Benjamin Blankertz
  Institution: Technische Universitaet Berlin
  Department: Department of Neurotechnology
  Country: DE
  Repository: DepositOnce TU Berlin
  Data URL: https://depositonce.tu-berlin.de/handle/11303/10934.2
  Publication year: 2020
  Funding: BMBF/BIFOLD (01IS18025A, 01IS18037A)
  Ethics approval: Approved by the ethics committee of the Charite University Medicine Berlin
  How to acknowledge: Please cite: Brandl, S. and Blankertz, B. (2020). Motor Imagery Under Distraction -- An Open Access BCI Dataset. Frontiers in Neuroscience, 14, 566147. https://doi.org/10.3389/fnins.2020.566147
  Keywords: brain-computer interface, motor imagery, EEG, distraction, open access, BCI

Abstract
--------
We present an open-access dataset of a motor imagery brain-computer interface (BCI) experiment conducted under six different distraction conditions. Sixteen healthy participants performed left vs. right hand motor imagery while being distracted by flickering video, number search tasks, news listening, eyes closed, vibro-tactile stimulation, or no distraction. Each participant completed one calibration run without feedback and six feedback runs under the different distraction conditions, resulting in 504 trials per subject.

Methodology
-----------
Participants completed one session with 7 runs of 72 trials each. Run 1 was calibration (no feedback, no distraction). Runs 2-7 included auditory feedback and one of six distraction conditions. Auditory cues indicated left or right hand imagery. Trial duration was 4.5 s with 2.5 s ITI. Online classification used CSP with LDA. EEG recorded at 1000 Hz with 63 channels, nose reference, using two BrainAmp amplifiers.

References
----------
Brandl, S. and Blankertz, B. (2020). Motor Imagery Under Distraction -- An Open Access BCI Dataset. Frontiers in Neuroscience, 14, 566147. https://doi.org/10.3389/fnins.2020.566147

Notes

.. versionadded:: 1.2.0
Appelhoff, S., Sanderson, M., Brooks, T., Vliet, M., Quentin, R., Holdgraf, C., Chaumon, M., Mikulan, E., Tavabi, K., Hochenberger, R., Welke, D., Brunner, C., Rockhill, A., Larson, E., Gramfort, A. and Jas, M. (2019). MNE-BIDS: Organizing electrophysiological data into the BIDS format and facilitating their analysis. Journal of Open Source Software 4: (1896). https://doi.org/10.21105/joss.01896

Pernet, C. R., Appelhoff, S., Gorgolewski, K. J., Flandin, G., Phillips, C., Delorme, A., Oostenveld, R. (2019). EEG-BIDS, an extension to the brain imaging data structure for electroencephalography. Scientific Data, 6, 103. https://doi.org/10.1038/s41597-019-0104-8

---
Generated by MOABB 1.5.0 (Mother of All BCI Benchmarks)
https://github.com/NeuroTechX/moabb
