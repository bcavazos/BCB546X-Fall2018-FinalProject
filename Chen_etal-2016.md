# BCB546X-Fall2018-FinalProject #

**Research Paper**

### **Chen et al. 2016. Genome-Wide Association Study and QTL Mapping Reveal Genomic Loci Associated with *Fusarium* Ear Rot Resistance in tropical Maize Germplasm. Gene |Genomes |Genetics, 6,3803-3815**
---

#### **Introduction** ####

*Fusarium* ear rot (FER) is a challenge in maize production because FER reduces not only the maize quality but also the maize production. FER is caused by *Fusarium verticillioides* which produces mycotoxins harmaful and fatal to humans and animals consuming contaminated grains. *F. verticillioides* is an ubiquitous fungi and can survive in soil, healthy seed and plant residue, and infection of maize can be initiated from seedborne or airbone inoculum as well as systemic infection from soil through roots to kernels. Moreover, maize is the main staple food in many developinf countries. solution to the problems of FER and fumonisin contamination is not to strengthen regulations, but rather to reduce fungal infection and mycotoxin levels in grain. The best strategy for controlling FER and reducing incidence of fumonisin contamination is the development and deployment of maize varieties with genetic resitance. 

FER is controlled by minor genes with relatively small effects that vary between environments and are not consistent between populations. Studies reported genotypic correction between FER resistance and fumonisin accumulation; therefore the FER resistance may simultaneously reducing fumonisin contamination. Although genetic variation for resistance to FER exists among maize inbred lines and hybrids, there is no evidence of complete resistance to either FER or fumonisin contamination in maize. Hence, there is a need for search novel resistance genes against *F. verticillioides* for a lasting solution to FER problems in maize production. 

The Quantitative trait Loci (QTL) Mapping is an important tool to identify genomic region containing genes which controlling traits. Additionnally, Genome-Wide Association Study (GWAS) method identified FER resistance genes using Single Nucleotide Polymorphism (SNPs). However, the GWAS method showed limitations for detecting false positives due to presence of population structure. Better approach to identify FER casual loci is to combine GWAS and linkage mapping for exploiting the complementary strengths of both approaches.  

The objectives of this study was to use GWAS to identify genomic regions associated with FER resistance in trpical maize germaplasm populations evaluated across three environments in Mexico, validate GWAS-identified genomic regions through linkage mapping using four biparental populations and Identify maize ingred lines with high levels of FER resistance. 


---

## **Methods**

1. **Germplasm materials and experimental design**
- A total of 940 elite tropical maize inbred lines was assembled. One elite maize inbred line, CML 155, was used as a resistant check. 
- Four biparental-derived populations were evaluated for resistance to FER.

    **POP1**: a doubled hapoid population with 201 lines. The resistant parent is CML 495. LAPOSTASEQ.C7F64-2-6-2-2-B*3

*  **POP2, POP3 and POP4**: F2:3 biparental populations developed from three resistant parents (CML492, CML495, and CML449) crossed to a single susceptible parent (LPSMT), and named POP2 (277 families), POP3 (268 families), and POP4 (272 families), respectively.

2. **Methods**

- **FER inoculations and evaluations**:  *F. verticilloides* was artificially inoculated in maize plant 7 days after flowing. 

- **Genotype data**: DNA was extracted from young levases of four biparental populations. In total, 200 of the polymorphic SNP markers were selected and used to genotype the entire population. Markers with allele frequency between 0.4 and 0.6 for both DH and F2:3 populations were included in the analysis. 

- **Association analysis**: A subset of 2,000 SNP markers randomly selected from 10,736 SNPs remained after removing SNPs with missing values, minor allele frequency, and physical position interval <50 kb. The subset was used for STRUCTURE analysis. 

- **QTL mapping in biparental populations**: Linkage maps were constructed using IciMapping v3.2 with Kosambi method for map distance calculation. Linkage maps were not constructed for POP3 and POP4 as the number of retained markers was small. 

#### **Replication Summary of the Original results**

- **Data Inspection**: All data files were inspected using R (genotype, blues phenotype, and biparental populations). BLUEs phenotype data were inspected only, and not used for any of our replication. Genotype data inspection can also be found in the markdown `data_inspectoin`. The biparental population data are in a format for iciMapping software and therefore we described them but they were not inspected in R. 

- **QTL discovery: two methods**: 

###### - ICMapping v#.2 software: 
from the Chen et al., `bip` files, we were able to reproduce their results, except discovered additional QTLs not listed in the paper. We found errors in their data file. 

###### R/QTL: 
We wrote an R script to easily QC data, plot missing data, determine LOD threshold, plot QTL grpahs and display a summary chart. 

###### Principal Component Analysis (PCA): 
TASSEL was used for PCA. The grouping does not come out correctly because groups  were established based on structure analysis. Our groupings were based on the archaeopteryx NJ tree groups on relatedness. However the pattern on the PCA plots resembles that in the paper.


#### In general, our analysis provided the same results as published. Our analysis had 4 additional QTLs qirh LODs of between 2.8. 













