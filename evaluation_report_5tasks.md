# MedSAM Sequential Training - Evaluation Report
Generated on: 2025-06-03 10:34:56
## Training Summary
- **Task01_BrainTumour**: 8 epochs, Loss: 0.0417 → 0.0086 (79.4% improvement)
- **Task02_Heart**: 8 epochs, Loss: 0.0104 → 0.0022 (78.6% improvement)
- **Task03_Liver**: 8 epochs, Loss: 0.2064 → 0.0639 (69.1% improvement)
- **Task04_Hippocampus**: 8 epochs, Loss: 0.7453 → 0.0574 (92.3% improvement)
- **Task05_Prostate**: 8 epochs, Loss: 0.0194 → 0.0083 (57.1% improvement)

## Evaluation Results
### Dice Score Comparison
| Task               |   Mean |    Std |   Median |   Samples |
|:-------------------|-------:|-------:|---------:|----------:|
| Task05_Prostate    | 0.8655 | 0.2053 |   0.9292 |        20 |
| Task02_Heart       | 0.6777 | 0.3486 |   0.8159 |        20 |
| Task01_BrainTumour | 0.6162 | 0.3133 |   0.7306 |        20 |
| Task04_Hippocampus | 0.4886 | 0.3432 |   0.5615 |        20 |
| Task03_Liver       | 0.4438 | 0.4453 |   0.4155 |        20 |
### Detailed Metrics by Task

#### Task01_BrainTumour
- **Samples evaluated**: 20
- **DICE**: 0.6162 ± 0.3133 (range: 0.0000 - 0.9400)
- **IOU**: 0.5116 ± 0.2974 (range: 0.0000 - 0.8867)
- **HAUSDORFF**: 63.3085 ± 24.9416 (range: 25.0799 - 100.0000)
- **PRECISION**: 0.5737 ± 0.3195 (range: 0.0000 - 0.9571)
- **RECALL**: 0.7276 ± 0.3418 (range: 0.0000 - 0.9972)
- **F1**: 0.6162 ± 0.3133 (range: 0.0000 - 0.9400)

#### Task02_Heart
- **Samples evaluated**: 20
- **DICE**: 0.6777 ± 0.3486 (range: 0.0000 - 0.9593)
- **IOU**: 0.5963 ± 0.3211 (range: 0.0000 - 0.9218)
- **HAUSDORFF**: 41.0260 ± 30.3598 (range: 15.5242 - 100.0000)
- **PRECISION**: 0.6197 ± 0.3312 (range: 0.0000 - 0.9284)
- **RECALL**: 0.7598 ± 0.3813 (range: 0.0000 - 0.9924)
- **F1**: 0.6777 ± 0.3486 (range: 0.0000 - 0.9593)

#### Task03_Liver
- **Samples evaluated**: 20
- **DICE**: 0.4438 ± 0.4453 (range: 0.0000 - 0.9578)
- **IOU**: 0.4009 ± 0.4053 (range: 0.0000 - 0.9190)
- **HAUSDORFF**: 89.5108 ± 21.8293 (range: 46.5296 - 113.8508)
- **PRECISION**: 0.4827 ± 0.4830 (range: 0.0000 - 0.9886)
- **RECALL**: 0.4147 ± 0.4212 (range: 0.0000 - 0.9555)
- **F1**: 0.4438 ± 0.4453 (range: 0.0000 - 0.9578)

#### Task04_Hippocampus
- **Samples evaluated**: 20
- **DICE**: 0.4886 ± 0.3432 (range: 0.0000 - 0.9162)
- **IOU**: 0.3895 ± 0.2957 (range: 0.0000 - 0.8453)
- **HAUSDORFF**: 204.5065 ± 94.3986 (range: 85.6037 - 321.2880)
- **PRECISION**: 0.4962 ± 0.4052 (range: 0.0000 - 0.9797)
- **RECALL**: 0.5726 ± 0.3924 (range: 0.0000 - 0.9736)
- **F1**: 0.4886 ± 0.3432 (range: 0.0000 - 0.9162)

#### Task05_Prostate
- **Samples evaluated**: 20
- **DICE**: 0.8655 ± 0.2053 (range: 0.0000 - 0.9815)
- **IOU**: 0.7990 ± 0.2024 (range: 0.0000 - 0.9638)
- **HAUSDORFF**: 36.8711 ± 17.5079 (range: 15.1327 - 100.0000)
- **PRECISION**: 0.8686 ± 0.2139 (range: 0.0000 - 0.9982)
- **RECALL**: 0.8698 ± 0.2115 (range: 0.0000 - 0.9929)
- **F1**: 0.8655 ± 0.2053 (range: 0.0000 - 0.9815)
