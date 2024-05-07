# antibody-binding-affinity
Predict the binding affinity (Kd) between single-chain variable fragments (scFv) variants and the SARS-CoV-2 peptide.

| Notebook | Keywords                           |
|--------|-------------------------------------------------------------------------------------|
| [Machine learning guided binding affinity prediction from antibody libraries - 1](https://github.com/arjan-hada/antibody-binding-affinity/blob/main/00_ml_antibody_bind_affinity.ipynb) | Protein Language Models, Transformers, Fine-tune, AbLang_heavy, antiberta2, antiberta2-cssp, ESM2_t33_650M_UR50D|
| [Machine learning guided binding affinity prediction from antibody libraries - 2](https://github.com/arjan-hada/antibody-binding-affinity/blob/main/01_ml_antibody_bind_affinity.ipynb) | Protein Language Models, Transformers, Fine-tune,  ESM2_t33_650M_UR50D, Error analysis|

**Key Takeaways**

🔹 We finetune antibody specific and general protein language model for predicting binding affinity (Kd) between single-chain variable fragments (scFv) and the target the SARS-CoV-2 peptide.

🔹 esm2_t33_650M_UR50D model demonstrated superior performance compared to antibody-specific language models, namely antiberta2-cssp, antiberta2, and ablang-H. Notably, while the performance of ablang-H lagged significantly behind, the remaining three models showed relatively comparable results. However, it is important to note, esm2_t33_650M_UR50D is larger, containing about 650 million parameters, whereas both antiberta2 and antiberta2-cssp have around 202 million parameters.

🔹 We exceeded the original study's Spearman rho (0.64 vs ~0.50) on hold-out set using just a single model, as opposed to the original study's ensemble of 16 models. 
