## Module 4 Quiz
#### Q1. Which of the following is FALSE:
- [ ] Alternative splicing is a common phenomenon in both animals and plants.
- [ ] The coding region with a protein-coding gene is used as the template for forming a protein.
- [ ] A codon is a nucleotide triplet that is translated into one amino acid.
- [x] A human gene can express at most 12 splice variants.

#### Q2. Which of the following is FALSE about the organization of a eukaryotic gene:
- [ ] Genes that have only one exon are not alternatively spliced
- [ ] Some eukaryoyic genes are single exon
- [ ] The length of the coding region in a transcript must be a multiple of 3
- [x] The length of intron cannot be a multiple 3

#### Q3. What programs could you use to align RNA-seq reads to: i) a reference genome, and ii) a transcript database?
- [ ] cufflinks, bowtie
- [ ] tophat, split
- [x] tophat, bowtie
- [ ] tophat, cufflinks

#### Q4. Which of the following is FALSE:
- [ ] As measures of gene expression, RPKM is determined at the level of reads and FPKM is determined at the level of fragments.  
- [ ] FPKM stands for fragments-per-kilobase of cDNA sequence-per million reads. 
- [x] The sums of FPKM values of all genes in a sample is 1,000,000.
- [ ] The sums of FPKMs of all transcripts of a gene is equal to the gene’s expression level.  

#### Q5. What programs could be used to i) assemble transcripts from RNA-seq reads, and ii) identify potentially novel transcripts and genes
- [x] cufflinks, cuffcompare
- [ ] tophat, cuffcompare
- [ ] tophat, bowtie
- [ ] tophat, samtools

#### Q6. Which of the following is FALSE about the gene annotations in the following GTF snippet:
- [x] The two transcripts for gene MG051951 overlap on the genome.
- [ ] It contains only one gene, MG051951.
- [ ] Gene MG051951 has two transcripts, MT162897 and MT070533.
- [ ] Transcript MT162897 has a single exon.

#### Q7. What does the following code NOT do:
- [x] Report spliced reads with at most 6 mismatches in the anchor site
- [ ] Create the output in the /home/me/SRR100000 directory
- [ ] Run multi-threaded, with 10 threads
- [ ] Report only reads with 10 or fewer alignments on the genome

#### Q8. What does the following code NOT do:
- [ ] Label cufflinks transcripts with the prefix ‘Test1’
- [x] Use the default reference transcript annotation to guide assembly
- [ ] Run cufflinks to assemble transcripts
- [ ] Create a soft link to the BAM read alignment file in the Test1 directory

#### Q9. Which of the following is NOT described in the following summary file produced by tophat:
- [x] 94.0% of the mate 2 reads were mapped
- [ ] Of the mapped mate 1 reads, 11.7% had multiple matches on the genome  
- [ ] The library was strand-specific
- [ ] Of the mapped mate 2 reads, 5.0% had multiple matches on the genome  

#### Q10. Which of the following is NOT TRUE about the output below, obtained from a cuffdiff differential expression analysis:
- [ ] Locus XLOC_000004 corresponds to gene AT1G01073
- [x] There are too many alignments for testing for differential expression at locus XLOC_000004
- [ ] Locus XLOC_000042 corresponds to gene AT1G01580
- [ ] There are not enough alignments for testing for differential expression at locus XLOC_000004
