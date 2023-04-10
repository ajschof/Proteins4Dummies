|Logo|

|LastCommit| |PythonVer| |Fork|

Proteins4Dummies (P4D)
======================

A proof of concept project to predict protein secondary structures.

Dumb Polypeptide Generator (DumbPG)
===================================

Method
-------------

In principle, this should be the easiest to make.

Pre-Training
************

* Train the model on a large dataset of random protein sequences
* This helps the model learn the general statistical properties of protein sequences to become familiar with the sequence space

Fine-Tuning
************

* The model is then fine-tuned with experimentally verified functional proteins with known structures and functions
* This helps the model learn specific seqeunce patterns that are associated with functional proteins


Dumb Uninformed Model For Assuming Secondary Structures (DUMFASS)
====================================================================

Complications
--------------

Whilst predicting the secondary structure is easier than predicting the tertiary structure, it is still challenging as it depends on multiple factors. Once we know the amino acid sequence, from there we also need information regarding:

1. Hydrophobicity
2. Hydrogen bonding
3. Steric constraints
4. Electrostatic interactions
5. Torsion angles (psi, phi)
6. Sequence motifs
7. Evolutionary information
8. Experimental data

Post-Training
--------------

Part of this project will be trying to utilise all this data to make a functional prediction model that, once trained, will be able to accurately predict secondary structures. The accuracy of the model will be determined using:

1. Q3 scores (three-state accuracy)
2. Q8 scores (eight-state accuracy)
3. Segment Overlap (SOV) scores
4. Matthew's Correlation Coefficient (MCC)
5. Precision, Recall and F1 scores
6. Confusion matrix

Predicting Tertiary Structure (Future Project)
==============================================

TBC

.. |Fork| image:: https://img.shields.io/badge/Fork%20Me-yellow?style=flat-square&logo=GitHub
   :alt: ForkMe

.. |PythonVer| image:: https://img.shields.io/badge/Python-3.10.10-blue?style=flat-square&logo=python
   :alt: PythonVersion

.. |LastCommit| image:: https://img.shields.io/github/last-commit/ajschof/Proteins4Dummies?logo=GitHub&style=flat-square
   :alt: PythonVersion
   
.. |Logo| image:: https://i.imgur.com/mZxD0hu.png
   :alt: logo
   :width: 300
