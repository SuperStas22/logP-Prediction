Created in 2022

Here is the English translation of your project description, suitable for GitHub, a portfolio, or a technical report.

Project Title: Prediction of Lipophilicity (LogP) for Drug-Like Compounds Using Machine Learning

Description:
The octanol-water partition coefficient (LogP) is a critical parameter in drug development, influencing bioavailability, membrane permeability, and toxicity (ADME properties). The goal of this project is to develop an accurate computational (in silico) model for LogP prediction, enabling accelerated screening of potential drug candidates without the need for costly experimental procedures.

Data:
A specialized dataset consisting of drug-like molecules was used, ensuring high relevance for medicinal chemistry applications.

Methodology and Pipeline:

    Feature Engineering:

        Physicochemical descriptors (molecular weight, number of hydrogen bond donors/acceptors, topological indices, etc.) were generated from SMILES representations using the RDKit library.

    Data Preprocessing:

        Cleaning: Removal of missing values and invalid chemical structures.

        Feature Selection: Exclusion of features with low variance and high collinearity to reduce dimensionality and prevent overfitting and rfecv.

        Standardization: Scaling data to a unified range (StandardScaler) to ensure the correct performance of distance-sensitive algorithms (e.g., SVR).

    Modeling:

        Training and validation of regression models: Random Forest and Support Vector Regression (SVR).

        Hyperparameter tuning (GridSearch/Optuna).

Results:
A comparative analysis of the algorithms showed that the Support Vector Regression method achieved the best performance.

    SVR (RBF kernel):

            
    R2=0.91
    R2=0.91

          

    — the model demonstrates high generalization capability.

    Random Forest:

            
    R2=0.87
    R2=0.87

          

    .

Conclusion:
The SVR-based model successfully predicts lipophilicity for this specific class of drug-like compounds, outperforming ensemble methods on this feature set following data standardization.
