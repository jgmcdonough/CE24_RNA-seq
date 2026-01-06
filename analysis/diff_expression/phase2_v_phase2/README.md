# Phase 2 vs. Phase 2
Analysis of oysters that experienced both phase 1 and phase 2

(to jump to [File Info](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2#file-info))

## Comparison Info
Investigating **multiple stressors** across **two timepoints** in oysters

### Control Comparisons
#### 1. Single exposure affects GE after a period of recovery
- CC vs. WC
- CC vs. HC
- CC vs. BC

#### 2. Sinlge exposure only experienced later in life affects GE
- CC vs. CW
- CC vs. CH
- CC vs. CB

#### 3. Effect of timing of initial stress exposure
- CW vs. WC
- CH vs. HC
- CB vs. BC

#### 4. No stress vs. most stress
- CC vs. WW
- CC vs. HH
- CC vs. BB

#### 5. Effect of initial exposure on response in later exposure
>matched priming
- WW vs. CW
- HH vs. CH
- BB vs. CB
> semi-matched priming

    >in context of later single stress
- CH vs. BH
- CW vs. BW
    >in context of later multiple stress
- CB vs. WB
- CB vs. HB

#### 6. Effect of initial exposure on subsequent response to stress
- WW vs. WC
- HH vs. HC
- BB vs. BC

### Interactions Between Stressors
#### 7. Effect of initial single/multiple stress on response in ...
>continuation of priming

**A. ...later *single* stress**
- BH vs. HH
- BW vs. WW

**B. ...later *multiple* stressors**
- HB vs. BB
- WB vs. BB

#### 8. Shared/unique responses among stressors with ...
**A. different *early* stressors**
>similar to [phase 1 vs. phase 1](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase1), can check for long-term trends/GE
- WC vs. HC
- BC vs. HC
- BC vs. WC

**B. different *late* stressors**
- CW vs. CH
- CB vs. CH
- CW vs. CB

#### 9. Effect of order of stresses on GE
>Does the order of when stress is experienced matter? Maybe one stressor is an informative cue for a later environment?
- WH vs. HW
- WB vs. BW
- HB vs. BH

## File Info
- [deseq_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/deseq_p2.v.p2.ipynb) - using `DESeq2` to identify DEGs
      - outputs are located in [deseq_res_files](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/deseq_res_files)