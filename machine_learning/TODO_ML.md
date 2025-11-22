# TODO: Baseline Biomarker Discovery Implementation using ML.

## Main Aim
Identify baseline genetic biomarkers that predict treatment response by analyzing variant allele frequency (VAF) data from all patients in the PRJNA714799 dataset using machine learning.

## Data Preparation

- [ ] Run data availability check on PRJNA714799 dataset
- [ ] Verify minimum 9 patients exist for ML analysis
- [ ] Confirm all patients have baseline (pre-treatment) timepoint data
- [ ] Check available disk space (50-100 GB) and compute time (10-12 hours)

## Run VCA Pipeline

- [ ] Update pipeline_config.yml to process all patients (patient_id_filter: null)
- [ ] Set up logging and monitoring
- [ ] Execute batch processing for all patients
- [ ] Verify all_variants.csv contains data for all patients

## Build Biomarker Discovery Script

- [ ] Create biomarker_discovery.py
- [ ] Define treatment response outcomes (responder vs non-responder)
- [ ] Extract baseline features (VAF stats, variant counts, read depth)
- [ ] Train multiple ML models (Random Forest, Gradient Boosting, Logistic Regression)
- [ ] Use Leave-One-Out cross-validation
- [ ] Calculate feature importance scores

## Identify Top Biomarkers

- [ ] Rank features by importance
- [ ] Select top 10 predictive biomarkers
- [ ] Test statistical significance
- [ ] Compare responders vs non-responders for each biomarker

## Generate Results

- [ ] Create visualizations (feature importance plots, ROC curves, distributions)
- [ ] Save results (baseline_features.csv, top_biomarkers.csv, plots)
- [ ] Write biomarker discovery report with clinical interpretation
- [ ] Document model performance and limitations

## Documentation

- [ ] Update main README with biomarker discovery workflow
- [ ] Create results folder README
- [ ] Document validation approach and limitations
- [ ] Add disclaimer for research use only