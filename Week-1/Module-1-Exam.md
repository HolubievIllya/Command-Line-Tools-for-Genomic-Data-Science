## Module 1 Exam
#### Q1. How many chromosomes are there in the genome?
#### Answer: 3 (grep -c  ">" apple.genome)
#### Q2. How many genes?
#### Answer: 5453 (cut -f1 apple.genes | uniq | wc -l)
#### Q3. How many transript variants?
#### Answer: 5456 (cut -f2 apple.genes | sort -u | wc -l)
#### Q4. How many genes have a single splice variant?
#### Answer: 5450 (cut -f1 apple.genes | uniq -c | grep " 1 " | wc -l)
#### Q5. How many genes have a single splice variant?
#### Answer: 3 (cut -f1 apple.genes | uniq  -c | grep -v " 1 " | wc -l)
#### Q6. How many genes are there on the '+' strand?
#### Answer: 2662 (sort -k 4 -k 1 apple.genes | grep "+" | wc -l)
#### Q7. How many genes are there on the '-' strand?
#### Answer: 2791 (sort -k 4 -k 1 apple.genes | grep "-" | wc -l)
#### Q8. How many genes are there on chromosome chr1?
#### Answer: 1624 (sort -k 4 -k 1 apple.genes | grep "chr1" | wc -l)
#### Q9. How many genes are there on chromosome chr2?
#### Answer: 2058 (sort -k 4 -k 1 apple.genes | grep "chr2" | wc -l)
#### Q10. How many genes are there on chromosome chr3?
#### Answer: 1771 (sort -k 4 -k 1 apple.genes | grep "chr3" | wc -l)
#### Q11. How many trancripts are there on chr1?
#### Answer: 1625 (sort -k 3 -k 5n apple.genes |  grep "chr1" | wc -l)
#### Q12. How many trancripts are there on chr2?
#### Answer: 2059 (sort -k 3 -k 5n apple.genes |  grep "chr2" | wc -l)
#### Q13. How many trancripts are there on chr3?
#### Answer: 1772 (sort -k 3 -k 5n apple.genes |  grep "chr3" | wc -l)
#### Q14. How many genes are in common between condition A and condition B?
#### Answer: 2410 (cut –f1 apple.conditionA | sort –u > apple.condA.sorted.genes | cut –f1 apple.conditionB | sort –u > apple.condB.sorted.genes | comm -1 -2 apple.condA.sorted.genes apple.condB.sorted.genes | wc –l)
#### Q15. How many genes are specific to condition A?
#### Answer: 1205 (comm -2 -3 conditionA conditionB | sort |uniq -u |wc -l)
#### Q16. How many genes are specific to condition B?
#### Answer: 1243 (comm -1 -3 conditionA conditionB | sort |uniq -u |wc -l)
#### Q17. How many genes are in common to all three condtions?
#### Answer: 1608 (comm -1 -2 conditionA conditionB |sort > contionAB | comm -1 -2 conditionAB conditionC |sort |wc -l)
