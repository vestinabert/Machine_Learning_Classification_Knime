# Machine Learning Classification Project

### Download KNIME Workflow

You can download the KNIME workflows from the following links:

- [Decision tree](https://vgtuitsc-my.sharepoint.com/:u:/g/personal/vestina_bertasiute_stud_vilniustech_lt/EWs7jCkhUShFnuOZVBvaCV0Bsn6SIzRDFiF-zZtlRcCQJQ?e=dyPwjJ)
- [Random forest](https://vgtuitsc-my.sharepoint.com/:u:/g/personal/vestina_bertasiute_stud_vilniustech_lt/ERueHh7MA8FDlW4W5yZ099MBLwG8ycEuuI12IyOMXnQlKg?e=HezwVU)
- [Gradient boosted trees](https://vgtuitsc-my.sharepoint.com/:u:/g/personal/vestina_bertasiute_stud_vilniustech_lt/ERZiYQQzieJIrzMUf_fLQrAB3PMo_NPb58sEZHoHZDy-ng?e=tY2xva)
- [NaiveBayes](https://vgtuitsc-my.sharepoint.com/:u:/g/personal/vestina_bertasiute_stud_vilniustech_lt/EVoqjB7-07NLrdjfVikRfY4BnKksuToP93dKM_mpYazu2A?e=RWFwjL)


This project focuses on applying machine learning techniques to classify data using various algorithms and data preparation methods. The main steps of the project are as follows:

- **Dataset Selection**: A dataset was selected from a publicly available source (e.g., [UCI Machine Learning Repository](https://archive.ics.uci.edu/)).
- **Algorithm Selection**: Four classification algorithms were chosen and used to build machine learning models.
- **Data Preprocessing**: Different data preparation techniques were tested, and their impact on the results was analyzed.
- **Parameter Optimization**: The models were experimentally evaluated with parameter optimization techniques to improve performance.
- **Implementation**: The project was implemented in KNIME, with all program steps properly named for clarity and reproducibility.
- **Results**: The final models and results were documented in a structured spreadsheet, with results evaluated and commented on.

All code or workflows are shared in this repository, along with the final analysis and insights derived from the experiments.
## Data tables
#### Naive Bayes

| Threshold | **With Data Normalizer** |  **With Data Normalizer**   | **Without Data Normalizer** | **Without Data Normalizer** | |
|-----------|--------------------------|------------------------|-----------------------------|------------------------|-------------------|
|           | **SMOTE Balancing**       | **SMOTE Oversampling**  | **SMOTE Balancing**          | **SMOTE Oversampling**  | **Without SMOTE**   |
| **0.1**   | 0.1555                   | 0.1937                 | 0.1481                      | 0.1789                 | 0.1540            |
| **0.2**   | 0.1465                   | 0.1742                 | 0.1457                      | 0.1644                 | 0.1535            |
| **0.3**   | 0.1441                   | 0.1613                 | 0.1445                      | 0.1574                 | 0.1535            |
| **0.4**   | 0.1441                   | 0.1555                 | 0.1441                      | 0.1552                 | 0.1535            |
| **0.5**   | 0.1441                   | 0.1551                 | 0.1437                      | 0.1542                 | 0.1535            |
| **0.6**   | 0.1441                   | 0.1549                 | 0.1441                      | 0.1538                 | 0.1535            |
| **0.7**   | 0.1441                   | 0.1547                 | 0.1441                      | 0.1536                 | 0.1535            |
| **0.8**   | 0.1441                   | 0.1546                 | 0.1441                      | 0.1537                 | 0.1535            |
| **0.9**   | 0.1441                   | 0.1546                 | 0.1441                      | 0.1537                 | 0.1535            |
| **1.0**   | 0.1441                   | 0.1546                 | 0.1441                      | 0.1537                 | 0.1535            |


#### Gardient Boosted Trees
| Nr. Model | **With Normalization** |  **With Data Normalizer**    | **Without Normalization** | **Without Data Normalizer** | |
|-----------|------------------------|------------------------|---------------------------|-----------------------|-------------------|
|           | **SMOTE Balancing**     | **SMOTE Oversampling**  | **SMOTE Balancing**        | **SMOTE Oversampling** | **Without SMOTE**   |
| **100**   | 0.970                  | 0.9978                 | 0.9711                    | 0.9988                | 0.9668            |
| **150**   | 0.972                  | 0.9986                 | 0.9723                    | 0.9992                | 0.9664            |
| **200**   | 0.973                  | 0.9986                 | 0.9731                    | 0.9994                | 0.9668            |
| **250**   | 0.973                  | 0.9989                 | 0.9731                    | 0.9994                | 0.9678            |
| **300**   | 0.973                  | 0.9985                 | 0.9666                    | 0.9994                | 0.9683            |
| **350**   | 0.970                  | 0.9986                 | 0.9617                    | 0.9991                | 0.9692            |
| **400**   | 0.970                  | 0.9986                 | 0.9617                    | 0.9990                | 0.9692            |
| **450**   | 0.970                  | 0.9974                 | 0.9609                    | 0.9990                | 0.9692            |
| **500**   | 0.970                  | 0.9971                 | 0.9609                    | 0.9990                | 0.9692            |

#### Decision Trees
| Min Record Numbers Per Node | **With Normalization** | **With Data Normalizer**  | **Without Normalization** | **Without Data Normalizer** |  |
|-----------------------------|------------------------|------------------------|---------------------------|-----------------------|-------------------|
|                             | **SMOTE Balancing**     | **SMOTE Oversampling**  | **SMOTE Balancing**        | **SMOTE Oversampling** | **Without SMOTE**|
| **100**                     | 0.7945                 | 0.9337                 | 0.7912                    | 0.9304                | 0.7499            |
| **150**                     | 0.7127                 | 0.9300                 | 0.7127                    | 0.9223                | 0.6831            |
| **200**                     | 0.6764                 | 0.9187                 | 0.6756                    | 0.9113                | 0.6646            |
| **250**                     | 0.6500                 | 0.9048                 | 0.6504                    | 0.8963                | 0.6026            |
| **300**                     | 0.6097                 | 0.9025                 | 0.6097                    | 0.8907                | 0.4619            |
| **350**                     | 0.4803                 | 0.8920                 | 0.4811                    | 0.8858                | 0.4628            |
| **400**                     | 0.4701                 | 0.8802                 | 0.4685                    | 0.8823                | 0.4031            |
| **450**                     | 0.4229                 | 0.8748                 | 0.4221                    | 0.8777                | 0.3946            |
| **500**                     | 0.4180                 | 0.8725                 | 0.4180                    | 0.8690                | 0.3903            |

#### Random Forest
| Nr. Model | **With Data Normalizer** |**With Data Normalizer**     | **Without Data Normalizer** | **Without Data Normalizer** | |
|-----------|--------------------------|------------------------|-----------------------------|------------------------|-------------------|
|           | **SMOTE Balancing**       | **SMOTE Oversampling**  | **SMOTE Balancing**          | **SMOTE Oversampling**  |  **Without SMOTE**  |
| **100**   | 0.9569                   | 0.9978                 | 0.9536                      | 0.99914                | 0.9550            |
| **150**   | 0.9556                   | 0.9977                 | 0.9528                      | 0.99914                | 0.9559            |
| **200**   | 0.9560                   | 0.9980                 | 0.9548                      | 0.99914                | 0.9545            |
| **250**   | 0.9569                   | 0.9980                 | 0.9569                      | 0.99914                | 0.9541            |
| **300**   | 0.9573                   | 0.9980                 | 0.9548                      | 0.99905                | 0.9541            |
| **350**   | 0.9581                   | 0.9981                 | 0.9565                      | 0.99910                | 0.9550            |
| **400**   | 0.9589                   | 0.9981                 | 0.9569                      | 0.99910                | 0.9564            |
| **450**   | 0.9585                   | 0.9981                 | 0.9565                      | 0.99910                | 0.9555            |
| **500**   | 0.9581                   | 0.9981                 | 0.9560                      | 0.99910                | 0.9559            |

## Summary of Top Model Performances
| **Model**               | **Accuracy** | **Normalization** | **SMOTE**               | **Parameter**                 | **Value**    |
|-------------------------|--------------|-------------------|-------------------------|-------------------------------|--------------|
| Naive Bayes              | 0.1937       | With normalization | SMOTE oversample by 10   | Threshold                      | 0.1          |
| Gradient Boosted Trees   | 0.9994       | Without normalization | SMOTE oversample by 10   | Nr. Model                      | 400-500      |
| Decision Trees           | 0.9337       | With normalization | SMOTE oversample by 10   | Min Record Numbers per Node    | 100          |
| Random Forest            | 0.9991       | Without normalization | SMOTE oversample by 10   | Nr. Model                      | 100-250      |
## Model Performance Insights

- **Naive Bayes**: 
  - Lower threshold values (0.1 - 0.3) yield higher performance, especially with normalization and using SMOTE. This suggests that a lower threshold allows the model to better capture minority class examples (higher sensitivity). As the threshold increases (0.4 - 1), most performance metrics become similar, indicating that higher thresholds reduce model sensitivity.

- **Gradient Boosted Trees**: 
  - Performance with SMOTE oversampling is significantly higher compared to just using SMOTE balancing, with values nearing 0.9998–0.9997. The highest results are achieved with 200–250 models.

- **Decision Trees**: 
  - When the minimum record numbers per node is low (e.g., 100), performance is higher, particularly when using SMOTE oversampling with normalization, as the tree has more nodes and can better adapt to the data. For example, SMOTE oversampling with normalization results in a very high score of 0.9337, while without SMOTE, the score drops to 0.7499. As the minimum record numbers per node increases (e.g., 500), performance decreases as the tree becomes simpler with fewer nodes.

- **Random Forest**: 
  - A higher number of models (e.g., 400–500 models) generally improves accuracy, though the difference is not very significant compared to a smaller number of models (e.g., 100–200). SMOTE oversampling by 10 (without data normalization) shows the highest results (around 0.9991), indicating that the increased amount of data improves model performance.
