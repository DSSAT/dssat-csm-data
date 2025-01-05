<p align="center">
<img width="400px" alt="DSSAT" src="https://dssat.net/wp-content/uploads/2014/05/DSSAT-color-update.png">
</p>
<p align="center">
<a href="http://dssat.net">[DSSAT Homepage]</a> | 
<a href="http://dssat.net/about">[About DSSAT]</a> | 
<a href="http://dssat.net/contact-us">[Contact us]</a>
</p>
<hr>
The Decision Support System for Agrotechnology Transfer (DSSAT) Version is a software 
application program that comprises crop simulation models for more than 45 different crops. The most recent version is DSAT v4.8.5 released in December, 2024 <a href="https://github.com/DSSAT/dssat-csm-os/releases/tag/v4.8.5.0">(Check latest RELEASE here)</a>.

For DSSAT to be functional it is supported by data base management programs for soil, 
weather, crop management, and experimental data, and by utilities and application 
programs. The crop simulation models simulate growth and development and predict yield, yield components, and many other traits and variables as a 
function of the soil-plant-atmosphere dynamics.

Questions about usage of the DSSAT Crop Modeling Ecosystem <a href="http://dssat.net/contact-us">[contact us]</a>.

Do not know how to use DSSAT? Consider participating in the <a href="https://dssat.net/training/upcoming-workshop/">[upcoming DSSAT training workshop]</a>

Read more about DSSAT at <a href="http://dssat.net/about">[DSSAT Homepage]</a>

## The data directory structure ##


The experimental datasets are distributed with the DSSAT Cropping System Model 
<a href="https://github.com/dssat/dssat-csm-os">(see dssat-csm-os GitHub repository)</a> and contain at least one experimental dataset 
for each crop simulation model, including management, soils, and weather data.

## Structure of the data ##
    .
    ├── Alfalfa
    ├── Amaranth
    ├── Bahia
    ├── ...
    ├── Maize
    ├── ...
    ├── Soil
    ├── ...
    ├── Soybean
    ├── ...
    ├── Weather
    ├── Wheat
    ├── YieldForecast
    └── README.md

Additional model-specific data files are included in the DSSAT source code repository under the <a href="https://github.com/DSSAT/dssat-csm-os/tree/develop/Data">"Data"</a> folder. 
These include model-specific data for genotypes, pest, standard model data, code files, DSSATPRO files, etc. 

    .
    ├── Genotype
    ├── Pest
    ├── StandardData
    ├── Data.CDE
    ├── Detail.CDE
    ├── DSSATPRO.v48
    ├── ...
    └── README.md
 
The files in this repository can be combined with the files in the Data folder of the source repository to 
replicate the directory structure of the Windows installation of DSSAT v4.8.5 (e.g., with Genotype directory at the
same level as the Alfalfa directory and the CDE files in the root directory).

## Test your CSM installation ##

To test your DSSAT-CSM model installation, execute the model from the Maize data directory using the following command line structure:

  *path+executable* A UFGA8201.MZX
  
where UFGA8201.MZX is the name of a file containing details of a field experiment. 
This command should run the model for this particular experimnt and generate outputs for six treatments in files Summary.OUT, PlantGro.OUT, and other files.


## How to Cite DSSAT ##

If you are planning to use DSSAT in any reports or publications, please make sure to refer to the version number you used.
The version and sub-version numbers can be found in the top section of your output files, e.g., 4.8.X (replace X with current version).
In addition, please use the following two references for DSSAT and the Cropping System Model. Other related publications can be found
in the Documentation section under DSSAT References and Model References.

Hoogenboom, G., C.H. Porter, K.J. Boote, V. Shelia, P.W. Wilkens, U. Singh, J.W. White, S. Asseng, J.I. Lizaso, L.P. Moreno, W. Pavan, R. Ogoshi, L.A. Hunt, G.Y. Tsuji, and J.W. Jones. 2019. The DSSAT crop modeling ecosystem. In: p.173-216 [K.J. Boote, editor] Advances in Crop Modeling for a Sustainable Agriculture. Burleigh Dodds Science Publishing, Cambridge, United Kingdom (https://dx.doi.org/10.19103/AS.2019.0061.10).

See also: [The DSSAT crop modeling ecosystem](https://dssat.net/wp-content/uploads/2020/03/The-DSSAT-Crop-Modeling-Ecosystem.pdf)

Hoogenboom, G., C.H. Porter, V. Shelia, K.J. Boote, U. Singh, W. Pavan, F.A.A. Oliveira, L.P. Moreno-Cadena, T.B. Ferreira, J.W. White, J.I. Lizaso, D.N.L. Pequeno, B.A. Kimball, P.D. Alderman, K.R. Thorp, S.V. Cuadra, M.S. Vianna, F.J. Villalobos, W.D. Batchelor, S. Asseng, M.R. Jones, A. Hopf, H.B. Dias, A. Jintrawet, R. Jaikla, E. Memic, L.A. Hunt, and J.W. Jones. 2024. Decision Support System for Agrotechnology Transfer (DSSAT) Version 4.8.5 (www.DSSAT.net). DSSAT Foundation, Gainesville, Florida, USA.

Jones, J.W., G. Hoogenboom, C.H. Porter, K.J. Boote, W.D. Batchelor, L.A. Hunt, P.W. Wilkens, U. Singh, A.J. Gijsman, and J.T. Ritchie. 2003. The DSSAT cropping system model. European Journal of Agronomy 18:235-265 (https://doi.org/10.1016/S1161-0301(02)00107-7).

See also: [The DSSAT cropping system model](https://dssat.net/jones_2003_the_dssat_cropping_system_model).
