# clustering-anonymization-utility
A clustering validity pipeline aiming at anonymization utility assessment.

In this study, clustering is conceived as an auxiliary tool to identify groups of special interest.  
Several anonymized clustering scenarios were compared with the original cluster solution. The clustering techniques were explored as data utility models in the context of data anonymization.
We used the partitional clustering algorithm, hard c-means, and analyzed several clustering validity indices (such as Davies-Bouldin, Calinski-Harabasz, and Silhouette) to understand to what extent the data structure is preserved, or not, after data anonymization.
For the assessment of the quality of each partition in this work we choose three indices commonly used in practical applications: Silhouette, Davis-Bouldin and Calinski-Harabasz.  Broadly speaking, these indices estimate the clusters’ cohesion and the clusters’ separation, combining them to produce a quality measure. For Silhouette and Calinski-Harabasz the best partitions correspond to higher values whereas for Davis-Bouldin lower values are better.
