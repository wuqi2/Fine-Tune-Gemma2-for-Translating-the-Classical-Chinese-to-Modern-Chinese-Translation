# Fine-Tune Gemma2 for Translating Classical Chinese to Modern Chinese

## Project Overview
This project aims to achieve translation from Classical Chinese (Wenyanwen) to Modern Chinese by fine-tuning a large language model. The training process leverages an open-source parallel corpus of Classical and Modern Chinese texts.

## Data Source
The training and testing data are sourced from an open repository on [GitHub](https://github.com/NiuTrans/Classical-Modern). This dataset provides numerous pairs of Classical Chinese phrases and their corresponding Modern Chinese translations. For this project, we selected a subset of the corpus focusing on representative historical texts and classical prose, such as *Dream Pool Essays* (*《梦溪笔谈》*) and *The Literary Mind and the Carving of Dragons* (*《文心雕龙》*).

## Technologies and Libraries Used
The following libraries and tools were utilized:

- `os`
- `json`
- `random`
- `jieba`
- `keras`
- `keras_nlp`
- `nltk`
- `matplotlib`
- `seaborn`
- `evaluate`

The model used is **Gemma2**, which was fine-tuned using the **LoRA** technique to optimize the translation of Classical Chinese texts.

## Model Evaluation
The project employs **BLEU** as the primary evaluation metric. The results indicate an average BLEU score of 0.01, which suggests limited effectiveness due to the inherent flexibility of Classical and Modern Chinese languages. To address this, manual analysis of randomly selected samples was conducted to provide deeper insights into the translation quality.

## How to Use
1. **API Configuration**  
   Enter your Kaggle API key for the Gemma2 model in the appropriate section of the code.
   
2. **Load Training Data**  
   Use the parallel corpus provided by GitHub. You can extend the dataset by modifying the relevant code.

3. **Train the Model**  
   Fine-tune the Gemma2 model using the LoRA method.

4. **Test Translation**  
   Replace the sample Classical Chinese text in the code with your desired text to observe translation results.

5. **Evaluate the Model**  
   Evaluate using the BLEU metric and conduct manual analysis to assess the translation quality comprehensively.

## Future Work
Given the limitations of current evaluation metrics for translation tasks, this project aims to explore novel methods better suited for assessing translations of Classical Chinese texts.

## References
- [Classical-Modern Parallel Corpus](https://github.com/NiuTrans/Classical-Modern)
