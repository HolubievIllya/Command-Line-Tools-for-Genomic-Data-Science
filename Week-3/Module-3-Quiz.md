## Module 3 Quiz
#### Q1. Which of the following statements is FALSE:
- [ ] Differences in the genomes of individuals are strong contributors to their phenotypic variations.
- [ ] Different versions of a gene resulted from genomic mutations are called alleles.
- [ ] SNV refers to a Single Nucleotide Variant.
- [x] SNP refers to a Single Non-defined Polymorhism

#### Q2. Which of the following statements is FALSE:
- [x] The VCF format shows the changes in amino acid resulting from the nucleotide mutation, in column 3.
- [ ] The VCF INFO lines describe characteristics of the variant, included in column 8.
- [ ] The BCF format is a binary compressed version of VCF.
- [ ] VCF stands for Variant Call Format.

#### Q3. What program can be used to generate a list of candidate sites of variation in an exome data set:
- [ ] samtools
- [ ] mkdir
- [x] bcftools
- [ ] bedtools

#### Q4. In a comprahansive effort to study genome variation in a patient cohort, you sequence and call variants in the exome. whole genome shotgun and RNA-seq data from each patient. Which of the following is FALSE when comparing these three types of resources:
- [x] Exome sequencing comprehensively captures variants in the 3’ and 5’ UTRs of genes.
- [ ] Exome sequencing can capture variants in a pre-defined set of coding exons and their immediate surrounding area.
- [ ] Exome sequencing cannot determine variants in novel polymorphic alternative splicing events.
- [ ] Exome sequencing captures fewer variants than whole genome sequencing.

#### Q5. Which of the following options can be used to allow bowtie2 to generate partial alignments?
- [x] --local
- [ ] -D
- [ ] –ignore-quals
- [ ] --sensitive

#### Q6. Select the correct interpretation for the snippet of 'mpileup' output below.
- [ ] Only site 2 shows potential variation;

     the alternate letter for site 2 is ‘.’;

     site 1 has 8 supporting reads, and site 2 has 16


- [ ] Only site 2 shows potential variation;

     the alternate letter for site 2 is G;

     site 1 has 8 supporting reads, and site 2 has 16


- [x] Only site 2 shows potential variation;

     the alternate letter for site 2 is A;

     site 1 has 8 supporting reads, and site 2 has 16


- [ ] Only site 2 shows potential variation; 

     the alternate letter for site 2 is A;

     the alternate allele for site 2 is supported by 9 reads

#### Q7. Given the set of variants described in the VCF excerpt below, which of the following is FALSE?
- [x] Average mapping quality for variant 3 is 40
- [ ] The sample contains only the alternate allele for variant 1
- [ ] The sample contains only the alternate allele for variant 3
- [ ] The sample contains both alleles for variant 2

#### Q8. What does the following code do:
- [ ] Run bowtie2 with a set of single-end reads, reporting the best alignment only;

    then determine the number of matches on each genomic sequence


- [x] Run bowtie2 with a set of single-end reads, reporting up to 5 alignments per read; then determine the number of matches on each genomic sequence


- [ ] Run bowtie2 with a set of paired-end reads, allowing for local matches;

   then report the numbers of alignments containing insertions and deletions, respectively;


- [ ] Run bowtie2 with a set of paired-end reads, allowing up to 10 matches per read;

   then report the number of matches on each genomic sequence

#### Q9. What does the following snippet of code do NOT do:
- [ ] Produce a 7-column intermediate mpileup file that is piped to ‘cut’
- [x] Report an empty column
- [ ] Report in the intermediate mpileup output the qualities of all read bases aligned at that position
- [ ] Require a sorted BAM file

#### Q10. What does the following code do NOT do:
- [ ] Write the output to file out.vcf.gz
- [x] Report all candidate sites
- [ ] Take input from the file in.vcf.gz
- [ ] Take input from a VCF compressed file
