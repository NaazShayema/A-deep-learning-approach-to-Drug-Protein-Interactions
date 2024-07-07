# A-deep-learning-approach-to-Drug-Protein-Interactions(DPIs)


Objective: Our model is designed to forecast interactions between unknown drug-protein pairs by transforming features of these pairs into a condensed latent representation and predicting the specific class of DPIs for those samples.


Dataset preparation: 
- DrugBank database is used
- smiles_output_2.csv contains drug_ID and SMILES sequence
- gene.fasta contains protein_ID and the nucleotide sequence 
- Interactive.csv contains the drug-protein interactive pairs
- non_interacting_pairs.csv contains  the non-interactive drug-protein pairs
- Interactive_pair_with_features_1.csv contains the drug-protein interactive pairs with features
- Non_Interactive_pair_with_features_20000.csv contains  the non-interactive drug-protein pairs with features


Feature extraction:
- Rcpi toolkit is used to extract drug and protein features


Files:
- Drug_feature_extractor.ipynb contains the drug feature extraction code
- Protein_feature_extractor.ipynb contains the protein feature extraction code
- Interactive_pair_with_featues.ipynb contains the code for the creation of drug-protein interactive pairs with features file
- Non_interactive_pair_20000.ipynb contains the code for the creation of drug-protein non interactive pairs with features file
- MDS_Dissertation_Final.ipynb contains the code for the data preprocessing, data splitting, model building, model training and model evaluation







                      
