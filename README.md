## ARCliDS (Adaptive Radiotherapy Clinical Decision Support System)

ARCliDS is a clinician‑facing AI platform designed to support response‑adaptive radiotherapy. It combines predictive modeling with reinforcement‑learning–based decision support to help clinicians personalize treatment strategies.

** What I Built**
- **Artificial Radiotherapy Environment (ARTE):**    
A predictive engine using radiobiology, **graph neural networks** and **multi‑omics** data to model tumor and normal‑tissue response under different dose‑adaptation strategies.

- **Optimal Decision Maker (ODM):**  
A **deep reinforcement learning** system that recommends dose‑adaptation policies balancing tumor control and toxicity.

A patent is pending, so the source code is not public. A live demonstration is available:
- [ARCliDS Shiny App](https://arclids.shinyapps.io/ARCliDS/).

**Note:** The app may take time to load because ARTE performs inference across **20 predictive models** over **45 decision points**, while ODM uses **5 models**. I choose 5 models per step for statistical ensembling to estimate model uncertainty. Since ARCliDS is hosted on **shinyapps.io**, which is not a high‑performance server, this computational workload can increase startup time.

Includes implementations for:
- **NSCLC adaptive Radiotherapy**
- **HCC adaptive SBRT**

**Publication:**
D. Niraula _et al., A clinical decision support system for AI-assisted decision-making in response-adaptive radiotherapy (ARCliDS)_. Scientific Reports 13, 5279 (2023).  
- [Paper](https://www.nature.com/articles/s41598-023-32032-6)
- [Supplementary Materials](https://media.springernature.com/original/springer-static/esm/art%3A10.1038%2Fs41598-023-32032-6/MediaObjects/41598_2023_32032_MOESM1_ESM.pdf). 

## Human-AI Interaction Modules
I developed two interactive platforms that allow clinicians to remotely evaluate ARCliDS using realistic NSCLC and HCC treatment cases. These modules support real‑time exploration of AI‑generated strategies and enable analysis of human–AI decision dynamics.  
- [ARCliDS-NSCLC Interaction Module](https://arclids.shinyapps.io/Eval_NSCLC_v2/) 
- [ARCliDS-HCC Interaction Module](https://arclids.shinyapps.io/Eval_HCC_v2/)

**What These Modules Do**
- Human–AI interaction in dynamic decision‑making
- Visualization of treatment‑response trajectories
- Practical evaluation of AI‑assisted dose‑adaptation strategies

**Publication:**
D. Niraula _et al., Intricacies of Human-AI Interaction in Dynamic Decision-Making for Precision Oncology: A Case Study in Response-Adaptive Radiotherapy_, Nature Communications,16, 1138 (2025).  
More details are available in:
- [Paper](https://www.nature.com/articles/s41467-024-55259-x) 
- [Supplementary Material](https://media.springernature.com/original/springer-static/esm/art%3A10.1038%2Fs41467-024-55259-x/MediaObjects/41467_2024_55259_MOESM1_ESM.pdf)
