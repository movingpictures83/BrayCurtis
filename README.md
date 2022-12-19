# BrayCurtis
# Language: R
# Input: TXT
# Output: PREFIX
# Tested with: PluMA 1.1, R 4.0.0
# Dependency:psadd_0.1.3,ape_5.4-1,microbiome_1.12.0,ggplot2_3.3.5,phyloseq_1.34.0

PluMA plugin that takes a community data matrix and computes the Bray-Curtis disbeta-diversity (Bray and Curtis, 1957) value between sample groups.

The plugin accepts as input a parameter file of keyword-value pairs.  Abundances and taxonomy are formatted according to PhyloSeq (McMurdie et al, 2013):

otufile: Abundances
mapping: Sample data
tree: Taxonomy
column: Attribute to use for grouping

Distances are output to a CSV file.  A PDF is also produce for the graph.  Both use the user-specified prefix.

