# MISP
Marker Imputation for Spatial Proteomics (MISP) based imaging data

![MISP_overview](https://github.com/user-attachments/assets/697cab69-4d38-464b-84b2-e827718f38bf)

Proteomics based multiplexed imaging can be limited due to the i) availability/limit of the markers in the panel, ii) imaging artefacts, and iii) high experimental costs. An example is the *[BRUCE](https://bruce.parkerici.org/pages/query-builder.html)* dataset, where consecutive tissue sections were imaged with two marker panels; immune and tumor panels. While both panels have an overlap of around 20 markers, each contain specific markers towards immune cell types and tumor cell types respectively. Inspired from *[7UP](https://academic.oup.com/pnasnexus/article/2/6/pgad171/7173167?login=true)*, we implement a simple explainable XGBoost based imputation of unseen markers from a overlap of existing antibody markers between two different panels.

![test_image_prediction](https://github.com/user-attachments/assets/93c82cf9-bd0e-44b3-8fec-fd3d5f0a92b2)

On a test split of immune panel, the model is able to achieve the following metrices
|  MSE     | PCC      |
| ------------- | ------------- |
| 0.0003 | 0.643 |


