# Summary statistics methods — practicals

Teaching practicals (Jupyter notebooks) for the **SMARTbiomed summer school**, covering
statistical-genetics methods that work directly on **GWAS summary statistics**:
heritability, genetic correlation, rare-variant association testing, and meta-analysis.
Each notebook runs on **Google Colab** — click its badge to open it. The emphasis is on
understanding what the methods do *under the hood*, with open-ended challenge questions at
the end of each practical and inline collapsible answers.

## Practicals

| Notebook | Topic | Open |
|---|---|---|
| [`LDSC_Practical_1_h2.ipynb`](LDSC_Practical_1_h2.ipynb) | SNP heritability ($h^2$) via univariate LD Score Regression (R) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/astheeggeggs/testing_colab/blob/main/LDSC_Practical_1_h2.ipynb) |
| [`LDSC_Practical_2_rg.ipynb`](LDSC_Practical_2_rg.ipynb) | Genetic correlation ($r_g$) via bivariate LDSC (R) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/astheeggeggs/testing_colab/blob/main/LDSC_Practical_2_rg.ipynb) |
| [`meta_analysis_Practical.ipynb`](meta_analysis_Practical.ipynb) | Meta-analysis: IVW, random effects, Stouffer & Cauchy combination (Python) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/astheeggeggs/testing_colab/blob/main/meta_analysis_Practical.ipynb) |
| [`rare_variant_Fisher.ipynb`](rare_variant_Fisher.ipynb) | Rare-variant testing with Fisher's exact test (Python) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/astheeggeggs/testing_colab/blob/main/rare_variant_Fisher.ipynb) |
| [`rare_variant_SAIGE.ipynb`](rare_variant_SAIGE.ipynb) | Gene-based rare-variant testing with SAIGE-Gene (Python) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/astheeggeggs/testing_colab/blob/main/rare_variant_SAIGE.ipynb) |

## Notes

- The LDSC and Fisher practicals use a **Python** Colab runtime but run R via the `%%R`
  cell magic; the meta-analysis practical is pure Python and SAIGE mixes shell, R and Python.
- Data files are downloaded into the Colab session from public Google Drive folders using
  `gdown`. 
