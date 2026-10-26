# Electronic supplementary material

Gene level tables and feature annotation of the doctoral thesis

**Computational Modeling of Transcriptional Responses to Growth Arrest in *Mycobacterium
tuberculosis*: Interaction Between Iron Availability and Carbon Source**

Jorge A. Cárdenas-Pestana. Programa de Doctorado en Física, Universidad de Zaragoza, 2026.

---

## What this repository is

The thesis reports gene level results that run to thousands of rows, so they are supplied as files
instead of being printed. Tables 1.8 and 2.8 of the thesis list them by name, and this repository
holds exactly those files, under exactly those names, together with the feature annotation on
which Chapter 2 rests.

The same ten files accompany the deposited thesis as its electronic annex. This repository is the
online copy, for a reader who has the PDF and wants the tables without unpacking the deposit.

## What is here

| Thesis | File | Content |
|---|---|---|
| 1.S3 | `chapter_1/Table_1.S3_counts.xlsx` | Read counts of the 3899 retained genes in the eight samples |
| 1.S4 | `chapter_1/Table_1.S4_DESeq2_contrasts.xlsx` | DESeq2 results for the five contrasts of Table 1.2, five sheets |
| 1.S5 | `chapter_1/Table_1.S5_GO_enrichment.xlsx` | Gene Ontology enrichment, a Readme sheet and four term sheets |
| 2.S2 | `chapter_2/Table_2.S2.xlsx` | Count matrix of the 4191 features in the thirty-two samples |
| 2.S3 | `chapter_2/Table_2.S3.xlsx` | Growth arrest differential expression, one sheet per carbon setting |
| 2.S4 | `chapter_2/Table_2.S4.xlsx` | Iron deprivation differential expression, one sheet per carbon setting |
| 2.S5 | `chapter_2/Table_2.S5.xlsx` | Interaction of iron with growth arrest, one sheet per carbon setting |
| 2.S6 | `chapter_2/Table_2.S6.xlsx` | Terms enriched among enhanced downregulated genes |
| 2.S7 | `chapter_2/Table_2.S7.xlsx` | Terms enriched among enhanced upregulated genes |
| 2.S8 | `chapter_2/Table_2.S8.xlsx` | Regulons enriched among enhanced upregulated genes |

[`annotation/`](annotation/) holds the extended feature table of Chapter 2, 4008 annotated features
plus 183 curated small RNAs, and the 4012 features its expression filter retains. Its own
[README](annotation/README.md) says what those tables do and do not contain.

[`MAPPING.tsv`](MAPPING.tsv) pairs every file with the thesis item it answers, its size and its
SHA-256.

## A note on the file names

These tables were first numbered as the supplementary material of the published article of Chapter
1 and of the manuscript of Chapter 2, where they are `Table_S3` to `Table_S10`. The thesis numbers
them by chapter, as 1.S3 and 2.S2. This repository carries the thesis numbering, because it is
what a reader arriving from the thesis will look for, and `MAPPING.tsv` records the correspondence.

## The sheets of Chapter 2 carry two rows above their headers

Files 2.S3 to 2.S8 open with a title row and a blank row before the column headers, as they were
prepared for the manuscript. A raw row count therefore gives two more rows than the figures stated
in the thesis.

## What is not here

- **The analysis code**, which lives in a separate repository together with the figure sources. It
  opens to the public when the manuscript reporting the thirty-two samples of Chapter 2 is
  published.
- **The raw sequencing data.** Chapter 1 is deposited in the Gene Expression Omnibus under
  accession [GSE213943](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE213943). The
  thirty-two samples of Chapter 2 will be deposited there on publication of the corresponding
  manuscript.
- **The figures**, which are printed in the thesis.

## License

The tables and the annotation are released under the Creative Commons Attribution 4.0
International license, [CC BY 4.0](LICENSE). The Chapter 1 tables are reproduced from Alebouyeh,
Cárdenas-Pestana et al., *Front Microbiol* 2022;13:956602, published under the same license.
