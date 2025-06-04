# medsam_bowanglab
AI Model for Medical Segmentation, with Adapters and Dataset Training

References:
MedSAM - Bowanglab: https://github.com/bowang-lab/MedSAM?tab=readme-ov-file
SAM - Meta: https://github.com/facebookresearch/segment-anything

### 🔧 **Training Overview**  
- **Method**: Sequential training on 5 medical segmentation tasks  
- **Configuration**: 8 epochs per task  
- **Loss Reduction** (Highest → Lowest):  
  - Hippocampus (92.3% ↓)  
  - Brain Tumour (79.4% ↓)  
  - Heart (78.6% ↓)  
  - Liver (69.1% ↓)  
  - Prostate (57.1% ↓)  

### 📊 **Key Results (DICE Score)**  
| Task               | Mean   | Stability (Std) | Rank |  
|--------------------|--------|-----------------|------|  
| **Prostate**       | 0.8655 | ±0.2053         | 🥇 **Best** |  
| **Heart**          | 0.6777 | ±0.3486         | 🥈 |  
| **Brain Tumour**   | 0.6162 | ±0.3133         | 🥉 |  
| **Hippocampus**    | 0.4886 | ±0.3432         |     |  
| **Liver**          | 0.4438 | ±0.4453         | ⚠️ **Weakest** |  

### 🔍 **Critical Findings**  
1. **Prostate (Task05)**:  
   - Outstanding performance (DICE 0.8655)  
   - Balanced precision/recall (~0.87)  
   - Lowest spatial error (Hausdorff: 36.87)  

2. **Liver (Task03)**:  
   - Lowest score (DICE 0.4438)  
   - Highest instability (±0.4453 std)  
   - Suboptimal precision/recall  

3. **Hippocampus (Task04)**:  
   - Best loss reduction (92.3%)  
   - Severe spatial errors (Hausdorff: 204.51)  

4. **Consistency Issues**:  
   - High standard deviations across all tasks  
   - Extreme performance variations between samples  

### 💎 **Conclusion**  
- **Strongest Task**: Prostate segmentation (robust, accurate)  
- **Weakest Task**: Liver segmentation (low accuracy, high variability)  
- **Key Concern**: Spatial accuracy in Hippocampus and stability in Liver require urgent attention.  
- **Positive**: All tasks showed >57% loss reduction during training.
