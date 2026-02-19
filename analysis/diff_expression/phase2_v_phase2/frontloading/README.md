# Transcriptional Frontloading
Frontloading is the idea that there are genes that have higher expression if primed with a stressor, with a reduced response when encoutnering the stressor again. This framework/pipeline was described in [Barshis et al., 2013](https://www.pnas.org/doi/full/10.1073/pnas.1210224110) and further used by [Collins et al., 2020](https://onlinelibrary.wiley.com/doi/full/10.1111/eva.13142) and [Gurr et al., 2022](https://onlinelibrary.wiley.com/doi/abs/10.1111/mec.16644).

## General Workflow
1. Identify stress-inducible genes (DEGs that are unique to, for example, CH vs. CC - both experience control conditions/not primed, then look at effect of later exposure to stress)
2. Calculate the "control ratio"
    - vst expression of (HC / CC) - looking at ratio of "primed" vs. control oysters in control oysters
    - *if control ratio is > 1*, there's higher transcription in the "primed" oysters than control oysters
3. Calculate the "response ratio"
    - vst expression of  ( (HH / HC) / (CH / CC) ) - looking at the response of "primed" oysters in stress or control conditions, vs. control oysters in stress or control conditions
    - *if the response ratio is < 1*, there's a reduced response (lower expression) when "primed" oysters experienced stress again
4. Identify frontloaded genes - control ratio > 1, response ratio < 1