## Module 3 Exam
#### Q1. How many sequences were in the genome?
#### Answer: 7 (grep –c “^>” wu_0.v7.fas)

#### Q2. What was the name of the third sequence in the genome file? Give the name only, without the “>” sign.
#### Answer: Chr3 (grep “^>” wu_0.v7.fas | head -3 | tail -1)

#### Q3. What was the name of the last sequence in the genome file? Give the name only, without the “>” sign.
#### Answer: mitochondria (grep “^>” wu_0.v7.fas | tail -1)

#### Q4. How many index files did the operation create?
#### Answer: 6 ()

#### Q5. What is the 3-character extension for the index files created?
#### Answer: bt2 (ls wu_0/)

#### Q6. How many reads were in the original fastq file?
#### Answer: 147354 (wc –l wu_0_A_wgs.fastq)

#### Q7. How many matches (alignments) were reported for the original (full-match) setting? Exclude lines in the file containing unmapped reads.
#### Answer: 137719 ()

#### Q8. How many matches (alignments) were reported with the local-match setting? Exclude lines in the file containing unmapped reads.
#### Answer: 141044 ()

#### Q9. How many reads were mapped in the scenario in Question 7?
#### Answer: 137719 ()

#### Q10. How many reads were mapped in the scenario in Question 8?
#### Answer: 141044 ()

#### Q11. How many reads had multiple matches in the scenario in Question 7? You can find this in the bowtie2 summary; note that by default bowtie2 only reports the best match for each read.
#### Answer: 43939 ()

#### Q12. How many reads had multiple matches in the scenario in Question 8? You can find this in the bowtie2 summary; note that by default bowtie2 only reports the best match for each read.
#### Answer: 56105 ()

#### Q13. How many alignments contained insertions and/or deletions, in the scenario in Question 7?
#### Answer: 2782 ()

#### Q14. How many alignments contained insertions and/or deletions, in the scenario in Question 8?
#### Answer: 2614 ()

#### Q15. How many entries were reported for Chr3?
#### Answer: 360295 ()

#### Q16. How many entries have ‘A’ as the corresponding genome letter?
#### Answer: 1150985 (cat out.full.mpileup.vcf | grep –v “^#” | cut –f4 | grep –P “^A$”)

#### Q17. How many entries have exactly 20 supporting reads (read depth)?
#### Answer: 1816 (cat out.full.mpileup.vcf | grep –v “^#” | grep –c “DP=20;”)

#### Q18. How many entries represent indels?
#### Answer: 1972 (cat out.full.mpileup.vcf | grep –v “^#” | grep –c INDEL)

#### Q19. How many entries are reported for position 175672 on Chr1?
#### Answer: 2 (cat out.full.mpileup.vcf | grep –v “^#” | cut –f1,2 | grep Chr1 | grep 175672)

#### Q20. How many variants are called on Chr3?
#### Answer: 398 ()

#### Q21. How many variants represent an A ->T SNP? If useful, you can use 'grep -P' to  allow tabular spaces in the search term. 
#### Answer: 392 (cat out.final.vcf | grep –v “^#” | cut –f4,5 | grep –P “^A\tT$” | wc -l)

#### Q22. How many entries are indels?
#### Answer: 320 (cat out.final.vcf | grep –v “^ #” | grep –c INDEL)

#### Q23. How many entries have precisely 20 supporting reads (read depth)?
#### Answer: 2 (cat out.final.vcf | grep –v “^#” | grep –c “DP=20;”)

#### Q24. What type of variant (i.e., SNP or INDEL) is called at position 11937923 on Chr3?
#### Answer: SNP (cat out.final.vcf | grep –v “^#” | cut -f1-5 | grep Chr3 | grep 11937923)
