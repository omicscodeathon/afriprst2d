A Reproducible Polygenic Risk Score Pipeline for Type 2 Diabetes in African Populations

# Author<sup>1\*</sup>, Author<sup>1,2</sup>, Author<sup>3</sup>, Author<sup>4\*</sup> …. and Olaitan I. Awe<sup>5,6\*</sup>

# <sup>1</sup> Department of xyz, School of ABC, University of PQR, Nairobi, Kenya

# <sup>2</sup> Department of xyz, School of ABC, University of PQR, Cape Town, South Africa

# <sup>3</sup> Department of xyz, School of ABC, University of PQR, Accra, Ghana

# <sup>4</sup> Department of xyz, School of ABC, University of PQR, Tunis, Tunisia

# <sup>5</sup> Institute for Genomic Medicine Research, West Hartford, CT, USA

# <sup>6</sup> African Society for Bioinformatics and Computational Biology, Cape Town, South Africa

# \* Corresponding Authors: Author1; <author1@gmail.com>

# Success Shepherd; <success_shepherd@gmail.com>

# Olaitan I. Awe; [laitanawe@gmail.com](mailto:laitanawe@gmail.com)

# Abstract

**Background:** Type 2 Diabetes continues to be among the most prevalent metabolic disorders globally, with rising incidence in African populations. Current genomic tools often lack the specificity or reproducibility required for diverse genetic backgrounds.

**Methodology:**

**Results:**

**Conclusion:**

**Keywords:** Polygenic Risk Score, Type 2 Diabetes, African Populations, Reproducible Pipeline, Bioinformatics

# Introduction

Type 2 diabetes (T2D) is a highly prevalent metabolic disorder that has evolved into a major global public health burden, characterized by rising incidence, debilitating micro- and macrovascular complications, and profound economic impact (Olamoyegun et al., 2024). In 2019, the global prevalence of diabetes was estimated at 463 million adults, with approximately 79% of affected individuals residing in low- and middle-income countries. This burden is particularly alarming in continental African settings, which accounted for approximately 19.4 million of these global cases, with T2D representing 90% of the diabetes burden in the region. Furthermore, Africa currently has the highest proportion of undiagnosed diabetes globally at 59.7%, and is projected to experience the world's largest increase in diabetes prevalence—an estimated 143% to 149% surge by 2045 (Olamoyegun et al., 2024). The etiology of T2D is multifactorial, driven by a complex interplay between environmental factors—such as urbanization, sedentary lifestyles, and dietary transitions—and substantial genetic heritability (Olamoyegun et al., 2024). While lifestyle modifications are critical for management, genetics contribute meaningfully to risk stratification and to a deeper understanding of the underlying disease etiology (Adam et al., 2022). Continental Africa harbors the greatest human genetic diversity globally, characterized by deeper population structure, more genetic variants, and shorter linkage disequilibrium (LD) blocks compared to non-African populations (Martin et al., 2019; Sibomana, 2024). Despite this, there is a severe underrepresentation of African populations in genome-wide association studies (GWAS) and global genomic databases, where they historically comprise a very small fraction of participants (Adam et al., 2022; Martin et al., 2019; Sibomana, 2024). Furthermore, many African ancestry samples in these databases are derived from admixed African American cohorts, which capture only a portion of the extensive continental African diversity (Chikowore et al., 2022; Irvin et al., 2024). This scarcity has severe consequences, leading to the limited discovery of ancestry-relevant or African-specific signals, a poorer understanding of genetic architecture, and significant challenges for equitable precision medicine (Martin et al., 2019; Sibomana, 2024). It is vital to distinguish continental African cohorts from African American ones, as their allele frequencies, LD patterns, and environmental contexts differ markedly (Chikowore et al., 2022; Sibomana, 2024). This profound genetic and environmental divergence naturally motivates why European-centric genomic tools consistently underperform in African populations (Adam et al., 2022; Martin et al., 2019). Polygenic risk scores (PRS) predict genetic liability by aggregating the weighted effects of many common variants across the genome (Irvin et al., 2024). These scores are typically derived from GWAS summary statistics using methods such as clumping and thresholding, Bayesian approaches like PRS-CS, or multi-ancestry frameworks (Adam et al., 2022; Ge et al., 2019; Irvin et al., 2024). Predictive performance depends heavily on matching ancestry between the discovery and target samples, primarily because of population-specific differences in allele frequencies and LD (Adam et al., 2022; Martin et al., 2019). Consequently, most existing T2D PRSs—developed primarily in European-ancestry data—show substantially reduced predictive accuracy, lower effect sizes, and less variance explained when applied to African-ancestry groups (Irvin et al., 2024; Martin et al., 2019). Prior efforts have explored African American-focused or multi-ancestry T2D PRSs, some of which improve performance relative to purely European scores and have been tested in continental African samples with mixed but encouraging results (Chikowore et al., 2022; Irvin et al., 2024). However, these efforts underscore the remaining limitations regarding sample size, representation of continental diversity, and cross-population transferability (Chikowore et al., 2022; Sibomana, 2024). This study addresses the specific gap of PRS development and validation in continental African cohorts, aiming to provide better risk stratification, facilitate earlier intervention, and ultimately reduce health disparities in precision medicine (Adam et al., 2022; Chikowore et al., 2022; Martin et al., 2019).

# Materials and Methods

## Data collection

Here we state the inclusion and exclusion criteria of the data we used, the sources of the data and filtrations we apply to extract the data of interest. And the separation of the data into training, validation and test datasets in addition to all transformations and operations done on our data to prepare them for the pipeline

## Model building Workflow

This section discusses the whole pipeline to build the model and the tools used.

## Model testing and validation and Benchmarking

Here we mention the parameters we measure to assess the model performance on the data and (optionally we can use previously built models and compare them with our model when applied to the same data)

# Results

**Data descriptive analysis:**

This section is meant to show our data, their full numbers, average age, sex ratio, and other available meta-data like subjects' distribution within Africa and so on.

**Model performance and comparison to previous models:**

This section will be made to show the outputs of the model we built and its performance on African Cohort data compared to the performance of previous models built on data from European and mixed ethnicities when applied on African data.

# Discussion

This section provides context as to why the software tool was developed and what needs it addresses regarding equity in precision medicine. In addition to highlighting the strengths of our model if it performed better than previous models using the evaluation parameters we presented in the results section.

# Conclusions and next steps

This section includes a brief discussion of allowances made for controlling bias or unwanted sources of variability, such as population stratification, and the limitations of any novel datasets. Future steps include the integration of multi-omic data to further refine risk prediction.

# Availability and Requirements

- **Project name:** Reproducible Polygenic Risk Score Pipeline
- **Project home page:** File
- **Operating system(s):** Platform independent if using the associated Docker/Singularity images. Mac OS X or Linux CLI if run outside Docker/Singularity images.
- **Programming language:** Bash, R 3.5, Perl, Python.
- **Other requirements:** Python 3.6 or higher, Java JDK, Chrome, Firefox, and Safari web browser.
- **License:** MIT
- **Any restrictions to use by non-academics:** None.

# Availability of data and materials

The dataset analyzed during the current study as a case study is publicly available at File and NCBI database File. The data supporting the results reported in this manuscript is included within the article and its additional files. The generated progress reports are in HTML format and can be viewed using any preferred browser such as Chrome, Safari, Internet Explorer and Firefox. The Project repository which also includes the entire code and other requirements can be downloaded from File. The guidelines for implementing this tool and related updates are available at: File.

# Abbreviations

- **CLI:** Command-Line Interface
- **FDR:** False Discovery Rate
- **GUI:** Graphical User Interface

# References

Adam, Y., Sadeeq, S., Kumuthini, J., Ajayi, O., Wells, G., Solomon, R., Ogunlana, O., Adetiba, E., Iweala, E., Brors, B., & Adebiyi, E. (2022). Polygenic Risk Score in African populations: progress and challenges. _F1000Research_, _11_, 175. <https://doi.org/10.12688/f1000research.76218.1>

Chikowore, T., Ekoru, K., Vujkovi, M., Gill, D., Pirie, F., Young, E., Sandhu, M. S., McCarthy, M., Rotimi, C., Adeyemo, A., Motala, A., & Fatumo, S. (2022). Polygenic Prediction of Type 2 Diabetes in Africa. _Diabetes Care_, _45_(3), 717–723. <https://doi.org/10.2337/dc21-0365>

Ge, T., Chen, C. Y., Ni, Y., Feng, Y. C. A., & Smoller, J. W. (2019). Polygenic prediction via Bayesian regression and continuous shrinkage priors. _Nature Communications_, _10_(1). <https://doi.org/10.1038/s41467-019-09718-5>

Irvin, M. R., Ge, T., Patki, A., Srinivasasainagendra, V., Armstrong, N. D., Davis, B., Jones, A. C., Perez, E., Stalbow, L., Lebo, M., Kenny, E., Loos, R. J. F., Ng, M. C. Y., Smoller, J. W., Meigs, J. B., Lange, L. A., Karlson, E. W., Limdi, N. A., & Tiwari, H. K. (2024). Polygenic Risk for Type 2 Diabetes in African Americans. _Diabetes_, _73_(6), 993–1001. <https://doi.org/10.2337/db23-0232>

Martin, A. R., Kanai, M., Kamatani, Y., Okada, Y., Neale, B. M., & Daly, M. J. (2019). Clinical use of current polygenic risk scores may exacerbate health disparities. _Nature Genetics_, _51_(4), 584–591. <https://doi.org/10.1038/s41588-019-0379-x>

Olamoyegun, M. A., Alare, K., Afolabi, S. A., Aderinto, N., & Adeyemi, T. (2024). A systematic review and meta-analysis of the prevalence and risk factors of type 2 diabetes mellitus in Nigeria. _Clinical Diabetes and Endocrinology_, _10_(1). <https://doi.org/10.1186/s40842-024-00209-1>

Sibomana, O. (2024). Genetic Diversity Landscape in African Population: A Review of Implications for Personalized and Precision Medicine. In _Pharmacogenomics and Personalized Medicine_ (Vol. 17, pp. 487–496). Dove Medical Press Ltd. <https://doi.org/10.2147/PGPM.S485452>

&nbsp;

# Acknowledgements

The authors thank the National Institutes of Health (NIH) Office of Data Science Strategy (ODSS) for their immense support before and during the October 2026 Omics codeathon organized by the Institute for Genomic Medicine Research (IGMR) in collaboration with the African Society for Bioinformatics and Computational Biology (ASBCB).

# Funding

The authors declare that no financial support was received for the research, authorship, and/or publication of this article.

# Author Information

## Affiliations

## Author ORCID

# Author Contributions

This section mention all authors using their initials with their contributions in the study All authors read and approved the final manuscript.

# Declarations

Ethics approval and consent to participate: Not applicable.

**Consent for publication**: Not applicable.

**Competing interests**: The authors declare that they have no competing interests.