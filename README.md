# mordred_descriptor_calculation (python 3.7.3)

Mordred is a freely available software application that can calculate >1800 2- and 3-dimensional molecular descriptors. See https://mordred-descriptor.github.io/documentation/master/descriptors.html for a list of descriptors and Moriwaki, H.; Tian, Y.-S.; Kawashita, N.; Takagi, T. J. Cheminf. 2018, 10, 4 for further details.

In this notebook, molecules are imported as a list of SMILES strings from an excel file. SMILES are typically downloaded from Reaxys after a substructure search, for example see Baran, P. S. et. al J. Am. Chem. Soc. 2021, 143, 7859 (SI page S140) and Dotson, J. J.;  Anslyn, E. V.; Sigman, M. S. 143, 19187 J. Am. Chem. Soc. 2021, (SI page 18).

2D and 3D mordred descriptors are calculated and filtered to remove errors and based on collinearity. An excel sheet of the final descriptors can be exported for other applications.

Dimensionality reduction (PCA) and clustering (K-means) is performed in order to test the resulting descriptors. If an error occurs, section 5 can be used to identify the improper descriptors or molecules (some molecules have been found to be particularly problematic for descriptor calculation).
