# clustering-anonymization-utility
A clustering validity pipeline aiming at anonymization utility assessment.

In this study, clustering is conceived as an auxiliary tool to identify groups of special interest.  
Several anonymized clustering scenarios were compared with the original cluster solution. The clustering techniques were explored as data utility models in the context of data anonymization.
We used the partitional clustering algorithm, hard c-means, and analyzed several clustering validity indices (such as Davies-Bouldin, Calinski-Harabasz, and Silhouette) to understand to what extent the data structure is preserved, or not, after data anonymization.

Clustering was applied to the original dataset, and to four resulting anonymization schemata. The first, DS1, was obtained by k-anonymization with k = 20; the remaining three were obtained by (ε, δ)-differential privacy with fixed ε = 1, and δ = 0.01, δ = 0.001 and δ = 0.0001 for DS2, DS3 and DS4 respectively. The parameters k, ε, δ were chosen in such way that the re-identification risk is less than 5%. The anonymization was performed with ARX (version 3.9.0). The parameters were: suppression limit - 100%; utility measure - loss; aggregate function - sum; population size - 5000. 

The original data, RAIDES files, are protected by the General Data Protection Regulation (GDPR). The consent for their use in the data safe center in Lisbon may be obtained by any researcher (https://www.dgeec.mec.pt/np4/contactos/). 
The anonymized datasets are as follows:

DS1 k-anonymization with k = 20;

DS2 (ε, δ)-Differential privacy with ε = 1 and δ = 0.01;

DS3 (ε, δ)-Differential privacy with ε = 1 and δ = 0.001;

DS4 (ε, δ)-Differential privacy with ε = 1 and δ = 0.0001.

For the assessment of the quality of each partition we choose three indices commonly used in practical applications: Silhouette, Davis-Bouldin and Calinski-Harabasz.  Broadly speaking, these indices estimate the clusters’ cohesion and the clusters’ separation, combining them to produce a quality measure. For Silhouette and Calinski-Harabasz the best partitions correspond to higher values whereas for Davis-Bouldin lower values are better.

