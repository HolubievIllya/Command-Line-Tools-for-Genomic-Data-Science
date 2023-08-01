## Module 2 Quiz
#### Q1. Which of the following strings cannot denote a DNA sequence:
- [x] APCTSYFPEITHI
- [ ] AAAAAAAAA
- [ ] AGCTACTACGAGCT
- [x] CCCCCCCCCC
#### Q2. How many lines does it take to specify: i) one fasta sequence? and ii) one fastq sequence? Select the best answer:
- [ ] Fasta – 1 line; fastq – 4 lines
- [x] Fasta – a fasta header followed by any number of sequence lines; fastq – 4 lines
- [ ] Fasta – any number of  lines, including a fasta header; fastq – 2 lines
- [ ] Fasta – 100 lines; fastq – 2 lines
#### Q3. Which of the following is incorrect:
- [ ] The SAM format is used to represent alignments.
- [ ] The BED format can be used to represent gene features. 
- [x] SAMtools flagstats reports the total number of mapped reads. 
- [ ] The GTF format can be used to represent gene features.
#### Q4. Which of the following strings cannot denote a DNA sequence:
- [ ] Soft clipping 
- [ ] Cut and paste 
- [x] Hard clipping 
- [ ] Padding
#### Q5. What is the minimum number of columns that are sufficient to specify a BED format?
- [ ] 1
- [ ] 2 
- [x] 3
- [ ] 4
#### Q6. Which of the following represents the most accurate conversion into BED of the GTF record?
- [ ] chr1	516	3312	genA.1	100	+	800	900	0	3	296,115,303	0,485,2494
- [ ] chr1 515 3312 genA.1 + 515 3312 0 3 296,115,303 516,1001,3010
- [ ] chr1 516 3312 genA + 516 3312 0 2 296,303 0,2494 
- [x] chr1	515	3312	genA.1	100	+	515	3312	0	3	296,115,303	0,485,2494
#### Q7. Determine the number of genes, transcripts, exons per transcript, gene orientation (strand), and the length of 5' most exon(s) from the GTF snippet below. Select the correct answer.
- [x] Genes: 1; Transcripts: 2; Exons: 2,2;  Strand: -; Length of 5’ exon(s): 2736, 2194.
- [ ] Genes: 1; Transcripts: 2; Exons: 2,2;  Strand: -; Length of 5’ exon(s): 2735, 2193.
- [ ] Genes: 1; Transcripts: 1; Exons: 4;  Strand: -; Length of 5’ exon(s): 2736.
- [ ] Genes: 1; Transcripts: 4; Exons: 1,1,1,1;  Strand: -; Length of 5’ exon(s): 2736, 1417,2194,795.
#### Q8. Which of the following is FALSE for the following read alignments:
- [ ] R1 maps uniquely to the genome.
- [x] R2’s mate is unmapped.
- [ ] R3 is unmapped. 
- [ ] The R1 alignment is the primary mapping (hit index 0) for that read.
#### Q9. For the alignment below, which statements are FALSE? The binary encoding for 97 is 972 = 0000 0110 00012. Select all answers that apply.
- [x] The two mates are identical in sequence.
- [x] The alignment represents a potential PCR or optical duplicate.
- [ ] The read and its mate are not properly aligned as a pair. 
- [ ] Both the read and its mate are mapped. 
- [ ] This is the first read in the pair. 
- [ ] The sequence of the read’s mate is reverse complemented in its alignment. 
#### Q10. Files 'A.bed. and 'B.bed' contain the following sets of intervals
- [ ] 5, 5, 5
- [ ] 3, 4, 2
- [ ] 9 , 2, 2
- [x] 3, 2, 2 
