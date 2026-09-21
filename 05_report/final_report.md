# Computational Analysis of Oculocutaneous Albinism Type 1 (OCA1) and TYR Mutations

**Student:** Ijan, Shane Mae B.  
**Disease:** Oculocutaneous Albinism Type 1 (OCA1)  
**Gene:** TYR (Tyrosinase)  
**Reference Transcript:** NM_000372.5  
**Reference Protein:** NP_000363.1  
**Documented Variant:** c.832C>T (p.Arg278Ter)  
**ClinVar Variation ID:** 99583  
**Galaxy History:** Ijan_OCA1_TYR_Mutation_Lab  
**Date of Analysis:** September 2026  

---

## Disease and Gene Background

Oculocutaneous Albinism Type 1 (OCA1) is a genetic condition associated with variants in the *TYR* gene. It is characterized by reduced or absent melanin pigmentation affecting the skin, hair, and eyes (Thomas et al., 2023).

The *TYR* gene is located on chromosome 11 at 11q14.3 and encodes tyrosinase, an enzyme involved in melanin production. Tyrosinase plays an important role in melanogenesis and is associated with the melanosome, where melanin is synthesized. Changes that reduce or eliminate normal tyrosinase activity can therefore disrupt melanin production and contribute to the hypopigmentation characteristic of OCA1.

---

## Wild-Type Reference Sequence

The normal reference sequence of the *TYR* gene was obtained from the NCBI RefSeq database. The reference transcript **NM_000372.5** was used, with its coding sequence (CDS) located at nucleotides **80–1669** and corresponding to the reference protein **NP_000363.1**.

The wild-type CDS contained **1,590 nucleotides**. Translation using Galaxy transeq produced a predicted protein containing **529 amino acids**. The sequence began with the start codon **ATG** and ended with the stop codon **TAA** in reading frame +1.

The predicted wild-type protein showed an exact amino-acid sequence match with the NCBI reference protein NP_000363.1, confirming the accuracy of the wild-type control.

### Wild-Type Sequence Characteristics

| Characteristic | Result |
|---|---|
| Reference transcript | NM_000372.5 |
| Reference protein | NP_000363.1 |
| CDS length | 1,590 nt |
| Predicted protein length | 529 aa |
| Start codon | ATG |
| Stop codon | TAA |
| Reading frame | +1 |
| First 10 amino acids | MLLAVLYCLL |
| Last 10 amino acids | DYHSLYQSHL |

---

## Documented TYR Mutation

The documented mutation selected for this analysis was **NM_000372.5(TYR):c.832C>T (p.Arg278Ter)**, listed in ClinVar as a pathogenic variant associated with OCA1.

The mutation involves a single-nucleotide substitution in which **cytosine (C) at coding nucleotide position 832 is replaced by thymine (T)**. This changes the normal codon **CGA**, which encodes arginine, to **TGA**, a stop codon.

Because the mutation is a substitution rather than an insertion or deletion, the reading frame is not shifted. However, it introduces a premature stop codon at amino acid position 278.


<img width="1722" height="722" alt="image" src="https://github.com/user-attachments/assets/ce9e0b84-223a-4b58-8a61-dd612fc45095" />

**Figure 1.** Manual introduction of the c.832C>T mutation into the TYR coding sequence.  

Figure 1 shows the manual modification of the TYR coding sequence to introduce the documented c.832C>T mutation, with the affected nucleotide highlighted in blue in both sequences. **a.)** The wild-type sequence contains cytosine (C) at nucleotide position c.832. **b.)** In the mutant sequence, this cytosine was replaced with thymine (T). The single-nucleotide substitution changes the codon from CGA to TGA, producing the predicted nonsense mutation p.Arg278Ter.

---

## Translation of the Documented Mutation

The mutant *TYR* coding sequence containing the **c.832C>T** substitution was translated using the same Galaxy transeq procedure used for the wild-type sequence.

The mutation introduced a premature stop codon at amino acid position **278**. Therefore, the predicted biological protein contains **277 amino acids**, compared with the normal 529-amino-acid protein. Approximately **252 amino acids from the C-terminal portion** of the normal protein are predicted to be absent.

| Characteristic | Result |
|---|---|
| Mutant CDS length | 1,590 nt |
| Mutation | c.832C>T |
| Codon change | CGA → TGA |
| Mutation type | Nonsense (stop-gained) substitution |
| Reading frame changed? | No |
| First amino-acid difference | Position 278 |
| Amino-acid change | Arg278 → Stop |
| Premature stop codon | Yes |
| Predicted mutant protein length | 277 aa |
| Approximate amino acids absent | 252 aa |


<img width="1655" height="748" alt="image" src="https://github.com/user-attachments/assets/175a2bd6-0e82-41c6-8c9d-1025641398bf" />

**Figure 2.** Comparison of the Wild-Type and Mutant TYR Protein Sequences.  

The figure shows the change in the predicted TYR protein caused by the c.832C>T mutation. **a.)** The wild-type TYR protein contains arginine (R) at amino acid position 278. **b.)** In the mutant sequence, arginine is replaced by a premature stop codon (*) at position 278, producing the p.Arg278Ter mutation. Although Galaxy transeq shows amino acids after the premature stop codon, these are not considered part of the predicted truncated protein because translation is expected to stop at position 278.

---

## Wild-Type and Documented Mutant Protein Comparison

The wild-type and documented mutant TYR sequences were compared using EMBOSS Needle global sequence alignment.

The alignment showed that the sequences first differ at amino acid position **278**, where arginine (R) is replaced by a premature stop (*). The alignment reported **529/530 (99.8%) identity**, **529/530 (99.8%) similarity**, and no alignment gaps.

The high sequence identity occurs because Galaxy transeq computationally displays translation downstream of the internal stop codon. Biologically, however, the premature stop is predicted to terminate translation, resulting in a 277-amino-acid protein rather than the normal 529-amino-acid protein.

| Characteristic | Wild-Type TYR | Documented Mutation |
|---|---|---|
| CDS length | 1,590 nt | 1,590 nt |
| Protein length | 529 aa | 277 aa predicted |
| Mutation | None | c.832C>T |
| Mutation type | None | Nonsense substitution |
| Reading frame changed? | No | No |
| Premature stop codon? | No | Yes, at codon 278 |
| Amino-acid effect | None | Arg278 → Stop |

---

## Molecular Consequence of the Documented Mutation

The *TYR* c.832C>T mutation changes a single cytosine (C) to thymine (T), converting the normal **CGA codon for arginine at position 278 into the TGA stop codon**. This produces the predicted **p.Arg278Ter** nonsense mutation.

The premature stop is predicted to terminate translation after 277 amino acids rather than producing the normal 529-amino-acid tyrosinase protein. The resulting predicted protein therefore lacks a large portion of its normal C-terminal sequence, which is expected to interfere with normal tyrosinase function.

Tyrosinase is required for normal melanin synthesis. Therefore, reduced or absent normal tyrosinase function can interfere with melanin production and contribute to the characteristic hypopigmentation of the skin, hair, and eyes associated with OCA1 (Thomas et al., 2023).

<img width="1800" height="762" alt="image" src="https://github.com/user-attachments/assets/b8b1525e-ef8a-43d4-beb3-6f9108700bd2" />

**Figure 3.** Mechanism from the TYR c.832C>T Mutation to the OCA1 Phenotype.

The *TYR* c.832C>T mutation changes a single cytosine (C) to thymine (T) at nucleotide position 832 of the coding sequence, converting the normal CGA codon for arginine at position 278 into a TGA stop codon. This results in the predicted nonsense mutation p.Arg278Ter, causing translation to terminate prematurely after 277 amino acids instead of producing the full-length 529-amino-acid tyrosinase protein. The resulting truncated protein lacks a large portion of its C-terminal region and is therefore predicted to have impaired normal tyrosinase function. Tyrosinase is essential for normal melanin biosynthesis, and disruption of this process can result in abnormal pigmentation (Hearing, 2005). Oculocutaneous albinism is characterized by reduced melanin pigmentation of the skin, hair, and eyes, with OCA1 resulting from abnormalities involving tyrosinase (Grønskov et al., 2007). Therefore, the *TYR* c.832C>T nonsense mutation is predicted to contribute to the OCA1 phenotype by producing a shortened tyrosinase protein that cannot support normal melanin production.

---

## Artificial Mutation Experiment

To further examine how mutation size affects a coding sequence, an artificial three-nucleotide deletion was introduced into the wild-type *TYR* CDS. The artificial mutation was **c.4_6del**, removing the sequence **CTC**.

Because exactly three nucleotides were deleted, the mutation remained in-frame and removed one leucine without shifting the downstream reading frame.

| Characteristic | Prediction/Result |
|---|---|
| Artificial mutation | c.4_6del |
| Deleted sequence | CTC |
| Nucleotides deleted | 3 |
| Amino acid affected | Leucine (L) |
| Frameshift expected? | No |
| WT protein length | 529 aa |
| Artificial mutant protein length | 528 aa |
| Premature stop codon | No |

The artificial three-nucleotide deletion shortened the *TYR* coding sequence from **1,590 nt to 1,587 nt** and reduced the predicted protein length from **529 to 528 amino acids**. Since three nucleotides were removed, the reading frame was maintained and no premature stop codon was introduced.

<img width="1668" height="837" alt="image" src="https://github.com/user-attachments/assets/602efb87-e79d-475f-bf8a-604026a3b87d" />

**Figure 4.** Comparison of the Wild-Type and Artificial Three-Nucleotide Deletion TYR Coding Sequences.  

The figure shows the TYR coding sequences before and after the artificial three-nucleotide deletion. **a.)** The normal wild-type *TYR* coding sequence contains 1,590 nucleotides. **b.)** The artificial mutant contains a three-nucleotide deletion, c.4_6del, reducing the CDS to 1,587 nucleotides. Because three nucleotides were deleted, the downstream reading frame was maintained.

---

## Comparison of Wild-Type, Documented, and Artificial Mutations

After translating the artificial mutation, the wild-type, documented c.832C>T mutation, and artificial c.4_6del mutation were compared to determine how different sequence changes affected the predicted TYR protein.

| Characteristic | Wild-Type TYR | Documented Mutation | Artificial Mutation |
|---|---|---|---|
| Mutation | None | c.832C>T (p.Arg278Ter) | c.4_6del |
| Nucleotide change | None | C>T at c.832 | Deletion of CTC at c.4–c.6 |
| CDS length | 1,590 nt | 1,590 nt | 1,587 nt |
| Mutation type | None | Nonsense (stop-gained) substitution | Three-nucleotide in-frame deletion |
| Reading frame changed? | No | No | No |
| Premature stop codon? | No | Yes, at codon 278 | No |
| Amino acid affected | None | Arg278 → Stop | Leucine deleted |
| Predicted protein length | 529 aa | 277 aa | 528 aa |
| Expected consequence | Normal tyrosinase protein | Truncated protein predicted to impair normal tyrosinase function | One amino acid removed while downstream reading frame remains intact |

The two mutations produced different predicted outcomes because of the type and location of the sequence changes. The documented **c.832C>T** mutation introduced a premature stop codon at amino acid 278, substantially shortening the predicted protein. In contrast, the artificial **c.4_6del** mutation removed exactly three nucleotides, deleting one amino acid without changing the downstream reading frame or introducing a premature stop codon.

---

## Interpretation

The analysis demonstrates that the biological effect of a mutation depends not only on the number of nucleotides affected but also on its exact position and how it changes the coding sequence. A three-nucleotide deletion can preserve the reading frame because codons consist of groups of three nucleotides, whereas deletion of one or two nucleotides can shift the reading frame and alter many downstream codons.

Not every DNA mutation necessarily changes an amino-acid sequence because some nucleotide substitutions are synonymous. Similarly, not every amino-acid substitution completely destroys protein function; the effect depends on the location and importance of the affected residue.

A premature stop codon can have a substantial effect because it may terminate translation before the full protein is produced. In this analysis, the documented c.832C>T mutation changed Arg278 to a stop codon and reduced the predicted TYR protein from 529 to 277 amino acids.

Mutations can also affect protein function without greatly changing protein length. For example, a substitution affecting an important amino acid may alter protein activity even if the overall length remains unchanged. In addition, mutations outside the protein-coding sequence may contribute to disease by affecting gene regulation, transcription, RNA processing, or splicing without directly changing the encoded amino-acid sequence.

Evidence from this computational analysis supports the sequence-level mechanism of the documented mutation: c.832C>T changed the codon from CGA to TGA, introduced a premature stop at position 278, and predicted a shortened TYR protein. Published evidence is still required to establish the biological effects of TYR variants on tyrosinase activity, melanin production, and the OCA1 phenotype. Previous research has identified pathogenic TYR mutations as an important cause of OCA1 (Chaki et al., 2005).

---

## Conclusion

This analysis demonstrated how changes in the *TYR* DNA sequence can produce different predicted effects on the tyrosinase protein. The documented **c.832C>T (p.Arg278Ter)** mutation introduced a premature stop codon and was predicted to shorten the protein from **529 to 277 amino acids**. In comparison, the artificial **c.4_6del** mutation removed three nucleotides and one amino acid while maintaining the reading frame, producing a predicted **528-amino-acid protein**. These results show that the effect of a mutation depends on its type, size, and exact location within the coding sequence.

---

## References

Chaki, M., Mukhopadhyay, A., Chatterjee, S., Das, M., Samanta, S., & Ray, K. (2005). Higher prevalence of OCA1 in an ethnic group of eastern India is due to a founder mutation in the tyrosinase gene. *Molecular Vision, 11*, 531–534.

National Center for Biotechnology Information. (n.d.). *Homo sapiens tyrosinase (TYR), mRNA (NM_000372.5), coding sequence 80–1669*. NCBI Nucleotide. National Library of Medicine.

National Center for Biotechnology Information. (n.d.). *Tyrosinase precursor [Homo sapiens] (NP_000363.1)*. NCBI Protein. National Library of Medicine.

National Center for Biotechnology Information. (n.d.). *NM_000372.5(TYR):c.832C>T (p.Arg278Ter), ClinVar Variation ID 99583*. ClinVar. National Library of Medicine.

Thomas, M. G., Zippin, J., & Brooks, B. P. (2023). *Oculocutaneous albinism and ocular albinism overview*. In M. P. Adam, S. Bick, G. M. Mirzaa, et al. (Eds.), *GeneReviews®*. University of Washington, Seattle.
