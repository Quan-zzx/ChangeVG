<div style="text-align: center; margin: 20px 0; border-top: 3px solid #FF6B35; padding-top: 15px; border-bottom: 1px solid #e0e0e0; margin-bottom: 20px;">
  <h1> Towards Comprehensive Interactive Change Understanding in Remote Sensing: A Large-scale Dataset and Dual-granularity Enhanced VLM</h1>
</div>


<img width="2400" height="1350" alt="image" src="https://github.com/user-attachments/assets/66620d17-e0bc-44dc-a262-7d97f473c1eb" />

## Publication

Our paper has been accepted to **IEEE Transactions on Geoscience and Remote Sensing (TGRS)**!

## <a id="Abstract"></a>Abstract

Remote sensing change understanding (RSCU) is essential for analyzing remote sensing images and understanding how human activities affect the environment. However, existing datasets lack deep understanding and interactions in the diverse change captioning, counting, and localization tasks. To tackle these gaps, we construct ChangeIMTI, a new large-scale interactive multi-task instruction dataset that encompasses four complementary tasks including change captioning, binary change classification, change counting, and change localization. Building upon this new dataset, we further design a novel vision-guided vision-language model (ChangeVG) with dual-granularity awareness for bi-temporal remote sensing images (i.e., two remote sensing images of the same area at different times). The introduced vision-guided module is a dual-branch architecture that synergistically combines fine-grained spatial feature extraction with high-level semantic summarization. These enriched representations further serve as the auxiliary prompts to guide large vision-language models (VLMs) (e.g., Qwen2.5-VL-7B) during instruction tuning, thereby facilitating the hierarchical cross-modal learning. We extensively conduct experiments across four tasks to demonstrate the superiority of our approach. Remarkably, on the change captioning task, our method outperforms the strongest method Semantic-CC by 1.39 points on the comprehensive $S^*_m$ metric, which integrates the semantic similarity and descriptive accuracy to provide an overall evaluation of change caption. Moreover, we also perform a series of ablation studies to examine the critical components of our method.


## <a id="Dataset"></a>Dataset
We introduce ChangeIMTI, a large-scale, multi-task instruction-tuning dataset for vision-language models (VLMs) in remote sensing change understanding. Built upon LEVIR-CC and LEVIR-MCI, ChangeIMTI supports five key tasks:

1. Change Captioning (natural language descriptions of bi-temporal changes),
2. Binary Change Classification (yes/no change detection),
3. Change Counting (number of changed regions),
4. Change Localization (coarse-grained spatial locations in a 3×3 grid), and
5. Multi-turn Dialogue (interactive, task-combined conversations).

The dataset contains 89,628 instruction-response pairs, making it the largest instruction-tuning resource for remote sensing change analysis to date. It enables VLMs to perform fine-grained semantic reasoning, spatial awareness, and interactive querying—key capabilities for real-world remote sensing applications.

Our dataset is available at: [Dataset Link](https://huggingface.co/datasets/Quan999/ChangeIMTI)

<img width="850" height="278" alt="image" src="https://github.com/user-attachments/assets/6460d8a8-ff11-4af2-b6c7-b52e4bb18c05" />


## <a id="Result"></a>Result
We provide a visualization of change captioning results from our model and baselines on the ChangeIMTI dataset:

<img width="1233" height="745" alt="image" src="https://github.com/user-attachments/assets/7d29ac36-b84a-41f6-b4ac-8ebcc550bdd2" />





