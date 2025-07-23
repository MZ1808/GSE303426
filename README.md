# Project
Aberrant glycolysis and IGF signaling in hypertensive cartilage development
# Purpose
Energy metabolism is implicated in cell differentiation and development. To delineate the difference in cartilage development between normotensive and hypertensive rats, we harvested chondrocytes from 5-day and 3-month-old rats to represent the developmental process and compared their transcriptomic profiles. 
# Experiment design
Total RNA was extracted from primary chondrocytes isolated from the femorotibial cartilage of 5-day and 3-month-old WKY and SHR (n=3 per group) using E.Z.N.A.® Total RNA Kit. Samples were sequenced using DNBSEQ platform with a paired-end read length of 100 bp (PE100). Reads of low quality, with adaptor sequences, or high levels of N base were filtered with SOAPnuke (v1.5.6). Bowtie2 (v2.4.4) was employed to align the clean reads to the reference genes in genome GCF_000001895.5_Rnor_6.0. Gene expression was quantified using RSEM (v1.2.28). Normalization and differential analysis of gene expression were performed with DESeq2 (v1.42.1) and corrected using the Benjamini-Hochberg procedure. KEGG enrichment analysis was performed on DEGs with unadjusted p-value less than 0.05 using GAGE (v2.52.0). Gene ontology (GO) enrichment analysis was performed on differentially expressed genes with adjusted p-value less than 0.05 using GOstats (v2.68.0). Gene Set Enrichment Analysis was performed using the official software (v4.3.3). The most prominent pathways were compared between different ages of animals from the same strain. Heatmaps depict the differentially expressed genes in each pathway. Pearson’s correlation was used to estimate the association between selected genes. Images were generated with ggplot2 (v3.5.0), ggcorrplot (v0.1.4.1), and ComplexHeatmap (v2.15.4) in RStudio. 
Sample Name | Animal strain | Animal Age | Cells | Batch | Replication 
--- | --- | --- | --- | --- | ---
WKY_Joint_5d_A | WKY | 5-day old | Joint chondrocytes | 1 | 1
WKY_Joint_5d_B | WKY | 5-day old | Joint chondrocytes | 1 | 2 
WKY_Joint_5d_C | WKY | 5-day old | Joint chondrocytes | 2 | 3 
WKY_Joint_3m_A | WKY | 3-month old | Joint chondrocytes | 1 | 1
WKY_Joint_3m_B | WKY | 3-month old | Joint chondrocytes | 1 | 2 
WKY_Joint_3m_C | WKY | 3-month old | Joint chondrocytes | 2 | 3 
SHR_Joint_5d_A | SHR | 5-day old | Joint chondrocytes | 1 | 1
SHR_Joint_5d_B | SHR | 5-day old | Joint chondrocytes | 1 | 2 
SHR_Joint_5d_C | SHR | 5-day old | Joint chondrocytes | 2 | 3 
SHR_Joint_3m_A | SHR | 3-month old | Joint chondrocytes | 1 | 1
SHR_Joint_3m_B | SHR | 3-month old | Joint chondrocytes | 1 | 2
SHR_Joint_3m_C | SHR | 3-month old | Joint chondrocytes | 2 | 3
# File description
<b>countdata.csv</b>: raw read counts <br>
<b>chon_seq.Rmd</b>: codes for analysis and producing figures <br>
<b>ids1.csv</b>: list of target genes <p>
<b>Normalized expression:</b> <br>
<b>exprs_5d.csv</b>: normalized expression of all chondrocytes from 5-day old rats <br>
<b>exprs_3m.csv</b>: normalized expression of all chondrocytes from 3-month old rats <br>
<b>exprs_WKY.csv</b>: normalized expression of all chondrocytes from WKY <br>
<b>exprs_SHR.csv</b>: normalized expression of all chondrocytes from SHR <p>
<b>Differential analysis results:</b> <br>
<b>DESeq_5d.csv</b>: differential analysis comparing WKY and SHR chondrocytes in 5-day-old rats <br>
<b>DESeq_3m.csv</b>: differential analysis comparing WKY and SHR chondrocytes in 3-month-old rats <br>
<b>DESeq_WKY.csv</b>: differential analysis comparing the developmental change from 5-day-old to 3-month-old in WKY <br>
<b>DESeq_SHR.csv</b>: differential analysis comparing the developmental change from 5-day-old to 3-month-old in SHR <p>
