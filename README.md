# dssat-csm-data
The DSSAT Cropping System Model - experimental data

These datasets are distributed with the DSSAT Cropping System Model 
(https://github.com/dssat/dssat-csm-os) and contain at least one 
experimental dataset for each crop simulation model, including management,
soils, and weather data.

Read more about DSSAT at http://dssat.net/about

See also: [The DSSAT Crop Modeling Ecosystem](https://dssat.net/wp-content/uploads/2020/03/The-DSSAT-Crop-Modeling-Ecosystem.pdf) and
[The DSSAT cropping system model](https://dssat.net/jones_2003_the_dssat_cropping_system_model).
and: [Non-threatening best practice DSSAT Fortran coding guidelines](https://dssat.net/non-threatening-best-practice-dssat-fortran-coding-guidelines). 


## Structure of the data ##
    .
    ├── Alfalfa
    ├── Bahia
    ├── ...
    ├── Soil
    ├── ...
    ├── Weather
    ├── Wheat
    ├── YieldForecast
    └── README.md

Additional model-specific data files are included in the DSSAT source code repository under the "Data" folder. 
(https://github.com/DSSAT/dssat-csm-os/tree/develop/Data). These include model-specific data for genotypes, pest, 
standard model data, code files, DSSATPRO files, etc. 

    .
    ├── Genotype
    ├── Pest
    ├── StandardData
    ├── Data.CDE
    ├── Detail.CDE
    ├── DSSATPRO.v47
    ├── ...
    └── README.md
 
The files in this repository can be combined with the files in the Data folder of the source repository to 
replicate the directory structure of the Windows installation of DSSAT v4.7 (e.g., with Genotype directory at the
same level as the Alfalfa directory and the CDE files in the root directory).

## Test your CSM installation ##

To test your DSSAT-CSM model installation, execute the model from the Maize data directory using the following command line structure:

  *path+executable* A UFGA8201.MZX
  
where UFGA8201.MZX is the name of a file containing details of a field experiment. This command should run the model for this particular experimnt and generate outputs for six treatments in files Summary.OUT, PlantGro.OUT, and other files.


## How to Cite DSSAT ##

If you are planning to use DSSAT in any reports or publications, please make sure to refer to the version number you used.
The version and sub-version numbers can be found in the top section of your output files, e.g., 4.8.X (replace X with current version).
In addition, please use the following two references for DSSAT and the Cropping System Model. Other related publications can be found
in the Documentation section under DSSAT References and Model References.

Hoogenboom, G., C.H. Porter, K.J. Boote, V. Shelia, P.W. Wilkens, U. Singh, J.W. White, S. Asseng, J.I. Lizaso, L.P. Moreno, W. Pavan, R. Ogoshi, L.A. Hunt, G.Y. Tsuji, and J.W. Jones. 2019. The DSSAT crop modeling ecosystem. In: p.173-216 [K.J. Boote, editor] Advances in Crop Modeling for a Sustainable Agriculture. Burleigh Dodds Science Publishing, Cambridge, United Kingdom (http://dx.doi.org/10.19103/AS.2019.0061.10)

Hoogenboom, G., C.H. Porter, V. Shelia, K.J. Boote, U. Singh, J.W. White, W. Pavan, F.A.A. Oliveira, L.P. Moreno-Cadena, J.I. Lizaso, S. Asseng, D.N.L. Pequeno, B.A. Kimball, P.D. Alderman, K.R. Thorp, M.R. Jones, S.V. Cuadra, M.S. Vianna, F.J. Villalobos, T.B. Ferreira,  J. Koo, L.A. Hunt, and J.W. Jones. 2021. Decision Support System for Agrotechnology Transfer (DSSAT) Version 4.8 (www.DSSAT.net). DSSAT Foundation, Gainesville, Florida, USA.

Jones, J.W., G. Hoogenboom, C.H. Porter, K.J. Boote, W.D. Batchelor, L.A. Hunt,  P.W. Wilkens, U. Singh, A.J. Gijsman, and J.T. Ritchie. 2003. DSSAT Cropping System Model. European Journal of Agronomy 18:235-265.

