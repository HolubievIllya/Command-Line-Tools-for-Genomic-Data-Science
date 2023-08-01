## Module 2 Exam

#### Q1. How many alignments does the set contain?
#### Answer: 221372 (samtools view athal_wu_0_A.bam | cut –f3 | grep –v ’*’ | wc -l)

#### Q2. How many alignments show the read's mate unmapped?
#### Answer: 65521 (samtools view athal_wu_0_A.bam | cut –f7 | grep –c ‘*’)

#### Q3. How many alignments contain a deletion (D)?
#### Answer: 2451 (samtools view athal_wu_0_A.bam | cut –f6 | grep –c ‘D’)

#### Q4. How many alignments show the read's mate mapped to the same chromosome?
#### Answer: 150913 (samtools view athal_wu_0_A.bam | cut –f7 | grep –c ‘=’)

#### Q5. How many alignments are spliced?
#### Answer: 0 (samtools view athal_wu_0_A.bam | cut –f6 | grep –c ‘N’)

#### Q6. How many alignments does the set contain?
#### Answer: 7081 ()

#### Q7. How many alignments show the read's mate unmapped?
#### Answer: 1983 (samtools view athal_wu_0_A.region.bam | cut –f7 | grep –c ‘*’)

#### Q8. How many alignments contain a deletion (D)?
#### Answer: 31 (samtools view athal_wu_0_A.region.bam | cut –f6 | grep –c ‘D’)

#### Q9. How many alignments show the read's mate mapped to the same chromosome?
#### Answer: 4670 (samtools view athal_wu_0_A.bam | cut –f7 | grep –c ‘=’)

#### Q10. How many alignments are spliced?
#### Answer: 0 (samtools view athal_wu_0_A.bam | cut –f6 | grep –c ‘N’)

#### Q11. How many sequences are in the genome file?
#### Answer: 7@SQ (samtools view –H athal_wu_0_A.bam | grep –c “SN:”)

#### Q12. What is the length of the first file secuence in the genome file?
#### Answer: 29923332 (samtools view –H athal_wu_0_A.bam | grep “SN:” | more)

#### Q13. What alignment tool was used?
#### Answer: stampy (samtools view –H athal_wu_0_A.bam | grep “^@PG”)

#### Q14. What is the read identifier (name) for the first alignment?
#### Answer: GAii05_00 ()

#### Q15. What is the start position of this read’s mate on the genome? Give this as ‘chrom:pos’ if the read was mapped, or ‘*” if unmapped.
#### Answer: 11700332 ()

#### Q16. How many overlaps (each overlap is reported on one line) are reported?
#### Answer: 3101 (bedtools intersect –abam athal_wu_0_A.region.bam –b athal_wu_0_A_annot.gtf –bed -wo > overlaps.bed)

#### Q17. How many of these are 10 bases or longer?
#### Answer: 2899 (cut –f22 overlaps.bed | sort –nrk1 > lengths)

#### Q18. How many alignments overlap the annotations?
#### Answer: 3103 (cut –f1-12 overlaps.bed | sort –u | wc -l)

#### Q19. Conversely, how many exons have reads mapped to them?
#### Answer: 21 (cut –f13-21 overlaps.bed | sort –u | wc -l)

#### Q20. If you were to convert the transcript annotations in the file “athal_wu_0_A_annot.gtf” into BED format, how many BED records would be generated?
#### Answer: 4 (cut –f9 athal_wu_0_A.annot.gtf | cut –d ‘ ‘ –f1,2 | sort –u | wc -l)
