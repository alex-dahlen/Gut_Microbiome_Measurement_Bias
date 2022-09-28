# Gut_Microbiome_Measurement_Bias
This is Python code to accompany the statistical analysis in an upcoming paper called "Achieving quantitative and accurate measurement of the human gut microbiome".  

Robust benchmarking studies have highlighted how measured relative microbial abundances can vary dramatically depending on how DNA is extracted, made into libraries, sequenced, and analyzed. To build upon prior research, we investigated how sample preservation and storage choices impact observed absolute microbial load and relative metagenomic and metatranscriptomic measurements. Specifically, we studied how two common stool preservatives (OMNIgene GUT OMR200 and Zymo DNA/RNA PowerShield) perform across a range of storage temperatures (-80°C, 23°C and 40°C).

We tested for systematic differences by kit and by temperature with a Generalized Estimating Equations (GEE) approach: we used an unadjusted regression model with fixed effects for the 7 conditions, and an exchangeable correlation structure between the participant-level clusters to account for repeat measurements.

The attached code cleans the abundance data, averages over 16S copy numbers to compute absolute microbial abundance, and fits the GEE model.
