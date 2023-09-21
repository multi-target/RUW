# RUW
This repository provides a reference implementation of the paper:  
RUW: A Dataset of Tweets on Multi-Target Stance Detection about the Russia-Ukraine War  
which is under review.
# Abstract
In this paper, we introduce RUW, an artificially annotated multi-target stance detection dataset. This dataset is set against the backdrop of the Russia-Ukraine conflict and is designed to analyze Twitter users' stances on both sides of the conflict during the Russia-Ukraine war. RUW is composed of 6,000 tweets collected through the Twitter API, with each tweet manually annotated as favor, against, or neutral toward each target. We explored the dataset by analyzing and modeling it using the Latent Dirichlet Allocation (LDA) model. We then conducted further analysis of our dataset using both machine learning and deep learning models to validate its feasibility. Additionally, we introduced a knowledge distillation model based on contrastive learning (KDCL). This model enables the effective learning of limited textual information through contrastive learning and knowledge distillation. We demonstrated the effectiveness of this approach on multiple datasets. We are making our new dataset publicly available to foster further research in multi-target stance detection.
# Environment settings
- python==3.7.4  
- numpy==1.21.6  
- pandas==1.3.5  
- tweet-preprocessor==0.6.0  
- scikit-learn==1.0.2  
# Basic usage
We provide one processed dataset:   
Ruw is used for the target stance detection task.
# Contact info
Please contact Guantong Liu at lgt@dlmu.edu.cn with any questions.
