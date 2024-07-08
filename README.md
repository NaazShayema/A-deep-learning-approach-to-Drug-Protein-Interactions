# A-deep-learning-approach-to-Drug-Protein-Interactions(DPIs)


Abstract: 
The accurate prediction of drug-protein interactions (DPIs) is crucial for the development of effective pharmaceuticals and the identification of potential off-target effects. This project explores the application of deep learning models to predict DPIs, leveraging their ability to analyze complex datasets and uncover intricate patterns. Drug-protein interactions are fundamental to the efficacy and safety of therapeutic agents. Traditional experimental approaches to studying these interactions can be time-consuming and costly. Computational methods, particularly deep learning models, offer a promising alternative by efficiently processing large datasets and making accurate predictions.
We implemented a deep learning framework for predicting drug-protein interactions (DPIs) using a combination of convolutional and recurrent neural networks. The model is trained on an extensive dataset of known DPIs, incorporating various features such as chemical structures of drugs, protein sequences, and interaction profiles. The architecture includes multiple 1D convolutional layers to capture spatial features, followed by an LSTM layer to capture sequential information. The model is designed with regularization techniques like dropout to prevent overfitting. And, we utilized the Rcpi toolkit for feature extraction and TensorFlow for model implementation. The performance is evaluated using metrics like percentage accuracy, precision, recall, and micro-averaged F1 score, demonstrating high predictive accuracy and outperforming traditional machine learning approaches. The model's ability to generalize to unseen data underscores its potential for large-scale DPI prediction and drug repurposing efforts.



Objective: 
Our model is designed to forecast interactions between unknown drug-protein pairs by transforming features of these pairs into a condensed latent representation and predicting the specific class of DPIs for those samples.


Dataset preparation: 
- DrugBank database is used
- smiles_output_2.csv contains drug_ID and SMILES sequence
- gene.fasta contains protein_ID and the nucleotide sequence 
- Interactive.csv contains the drug-protein interactive pairs
- non_interacting_pairs.csv contains  the non-interactive drug-protein pairs
- Interactive_pair_with_features_1.csv contains the drug-protein interactive pairs with features
- Non_Interactive_pair_with_features_20000.csv contains  the non-interactive drug-protein pairs with features
- All other files used in this project is available in DrugBank database


Feature extraction:
- Rcpi toolkit is used to extract drug and protein features


Files:
- Drug_feature_extractor.ipynb contains the drug feature extraction code
- Protein_feature_extractor.ipynb contains the protein feature extraction code
- Interactive_pair_with_featues.ipynb contains the code for the creation of drug-protein interactive pairs with features file
- Non_interactive_pair_20000.ipynb contains the code for the creation of drug-protein non interactive pairs with features file
- MDS_Dissertation_Final.ipynb contains the code for the data preprocessing, data splitting, model building, model training and model evaluation


Experimental Result and Analysis:
- The proposed method employs 26881 samples for training and 2987 samples for validation. The graph for training and validation accuracy over the epochs helps in assessing the model's performance and diagnosing potential issues such as overfitting or underfitting. And, we observe training accuracy is higher than the validation accuracy. This graph also shows how the accuracy increases over the epochs for both training and validation phases.
- The graph for training and validation losses over the epochs helps in assessing the model's performance and diagnosing potential issues such as overfitting (where the validation loss increases while the training loss decreases) or underfitting (where both training and validation losses are high). This graph clearly show a consistent reduction in loss for both phases over the epochs. And, we observe that validation loss is higher than training loss.
- Our test dataset consists of 20% non-interacting and interacting DPI samples i.e., we have 7467 DPI samples. The DPI predictions achieved by our proposed model are presented by the confusion matrix. From this confusion matrix, it can be seen that out of a total of 7467 DPI samples, the proposed method accurately predicted 3486 drug-protein pairs that interact. Additionally, the model correctly classified 2602 samples as non-interacting. The proposed method achieved an overall accuracy of 81.53%, with precision, recall, and F1 values of 0.8153, 0.8153, and 0.81, respectively.








                      
