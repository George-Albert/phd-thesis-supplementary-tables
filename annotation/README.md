# Feature annotation of Chapter 2

Two tables describe the features Chapter 2 measures. They are written by
`Codes/001_prepare_inputs_and_table_s1.R` and `Codes/003_deseq2_selected_contrasts_tables_s3_s5.R`
of the Chapter 2 workspace.

## feature_data_4191.tsv

The extended annotation, 4191 features: the 4008 features of the RefSeq annotation of ASM19595v2
downloaded on 17 October 2024, plus a curated panel of 183 small noncoding RNAs taken from a
published survey of the *Mtb* small RNA repertoire. Adding them is what makes this class of
features measurable at all, since a coding sequence annotation leaves them outside the measurement.

Composition: 3906 protein coding, 183 added small RNAs, 45 tRNA, 30 pseudogene, 20 annotated
ncRNA, 3 rRNA, 2 misc_RNA and 2 other.

## feature_data_4012.tsv

The 4012 features retained by the low expression filter, which is `filterByExpr` of edgeR applied
after the ribosomal RNA features are set aside. This is the universe every contrast of Chapter 2 is
estimated on, and the background against which functional enrichment is assessed.

Composition: 3908 coding sequences, that is 3877 protein coding, 29 pseudogene and 2 other, and 104
stable RNAs, of which 65 are small RNAs added to the reference and 39 were already present in it.

## One limitation worth stating

The 183 added small RNAs carry **no genomic coordinates** in these tables: their start, end and
strand fields are empty, because the rows were created to match a count matrix produced upstream.
The coordinate annotation that `featureCounts` consumed is not part of this repository.

These two tables therefore document the feature universe of the analysis and support every step
from the count matrix onward. They are not sufficient to recount the small RNAs from raw reads. Any
reanalysis starting from the sequencing data will need the coordinate annotation of the 183 small
RNAs from its published source.
