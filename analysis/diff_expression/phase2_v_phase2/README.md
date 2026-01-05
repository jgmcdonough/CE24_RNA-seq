# Phase 2 vs. Phase 2
Analysis of oysters that experienced both phase 1 and phase 2

(to jump to [File Info](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2#file-info))

## Comparison Info
Investigating **multiple stressors** across **two timepoints** in oysters

### 1. Priming vs. No Priming
The effect of early exposures in the response to later exposures
#### A. matched stressors
- **HH vs. CH**
- **WW vs. CW**
- **BB vs. CB**
#### B. semi-matched stressors
the oyster experienced both a repeated *and* a novel stress in later exposure
- **WB vs. CB**
- **HB vs. CB**

### 2. Single vs. Multiple Stressor Priming ...
#### A.  ...when later exposed to *single* stressors
- **BH vs. HH**
- **BW vs. WW**
#### B. ...when later exposed to *multiple* stressors
- **HB vs. BB**
- **WB vs. BB**

### 3. Timing of Stress Exposure
- **CH vs. HC**
- **CW vs. WC**
- **CB vs. BC**

### 4. Effect of Early Exposure in Subsequent Response
- **HH vs. HC**
- **WW vs. WC**
- **BB vs. BC**

### 5. Shared/Unique Responses In...
#### A. ...Different *Early* Stress Exposures
>similar to [p1 v. p1 analyses](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase1), but looking at this when oysters are older and returned to control conditions
- **WC vs. HC**: single early stress 
- **BC vs. HC**: multiple vs. single early stress
- **BC vs. WC**: multiple vs. single early stress
#### B. ...Different *Later* Stress Exposures
- **CW vs. CH**: single early stress 
- **CB vs. CH**: multiple vs. single early stress
- **CB vs. CW**: multiple vs. single early stress

### 6. Order of Stressors
Does the order of when stress is experienced matter? Maybe one stressor is an informative cue for a later environment? 
- **WH vs. HW**

## File Info
- [deseq_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/deseq_p2.v.p2.ipynb) - using `DESeq2` to identify DEGs
      - outputs are located in [deseq_res_files](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/deseq_res_files)