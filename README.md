# **Transancestral TWAS Reveals Ancestry-Structured Convergence of Bipolar Genetic Liability on Polycomb-Vulnerable GABAergic and Synaptic Maintenance Pathways**

## **Abstract**

Bipolar disorder is marked by wide clinical variation, uneven treatment response, and persistent cognitive and functional impairment even outside acute mood episodes. Genomic studies have expanded the number of bipolar disorder risk loci, but the biological interpretation of these findings remains incomplete, particularly across ancestries. Synaptic dysfunction, altered inhibitory tone, and glutamate–GABA imbalance have been repeatedly implicated in mood and psychotic disorders, yet these findings have not been well integrated with age-related epigenetic mechanisms that may affect neuronal identity and synaptic maintenance.

We performed a secondary analysis of ancestry-stratified bipolar disorder TWAS meta-Z statistics from African ancestry, East Asian ancestry, and European ancestry strata. We tested whether bipolar TWAS signal showed preferential proximity to Polycomb-derived neuronal aging modules, represented by KEGG pathways linked to cell adhesion and neuronal identity, synaptic scaffold and neurotransmission, and stress/homeostasis pathways. These modules were compared against an antipsychotic-related gene-set comparator derived from drug–gene interaction data. Analyses included absolute-Z gene-set enrichment, head-to-head differential testing, leading-edge extraction, transancestry recurrence analysis, hub prioritization, signed-Z directionality testing, and ancestry-differential follow-up.

No Polycomb module outperformed the antipsychotic comparator across all three ancestries, and no module passed combined FDR across ancestries. However, the GABAergic synapse pathway was the only module meeting the prespecified European-dominant criterion. In the European stratum, this pathway outperformed the antipsychotic comparator, with NES 1.3334, p \= 0.0105, and dNES 0.2836. Across ancestries, 69 core leading-edge genes were shared, anchored by five universal hubs: CACNA1B, DRD2, GABRA6, GABRB2, and LIMK1. Within this core, a compact seven-gene GABA/glutamatergic/calcium subnetwork emerged: CACNA1B, GABRA6, GABRB2, GRIK2, GRM3, SLC1A7, and SLC38A3.

These findings support an ancestry-structured convergence model in which bipolar genetic liability intersects with Polycomb-vulnerable synaptic maintenance nodes. The results do not show uniform pan-ancestry Polycomb superiority or consistent directional repression. Instead, they point to magnitude-based convergence, strongest in the European stratum and centered on inhibitory tone, presynaptic calcium signaling, and excitatory–inhibitory balance. This framework may help guide ancestry-aware stratification and functional validation in bipolar disorder.

## **Introduction**

### **Clinical burden and treatment challenges in bipolar disorder**

Bipolar disorder remains one of the most disabling psychiatric illnesses because it affects mood, cognition, functioning, and physical health over long periods of life. The diagnosis covers a broad clinical range, from recurrent mania and depression to mixed states, residual symptoms, cognitive dysfunction, and substantial medical comorbidity. Even when acute mood episodes are controlled, many patients continue to experience impaired attention, reduced processing speed, executive dysfunction, and difficulty returning to previous social or occupational functioning. This gap between symptomatic stabilization and functional recovery is one reason why bipolar disorder continues to be difficult to treat in ordinary clinical practice.

Current treatments are effective for many patients, but they are not precision treatments. Mood stabilizers, antipsychotics, antidepressant strategies used with caution, neuromodulation, and adjunctive anti-inflammatory or glutamatergic approaches are chosen mainly on clinical grounds rather than on mechanism-based biomarkers. Treatment response is variable, adverse effects often limit adherence, and the same medication class can have very different outcomes across patients. Real-world studies from Asian clinical settings have also shown how treatment practices vary across regions, adding another layer of complexity to interpretation and generalizability \[1,2\]. This clinical heterogeneity makes bipolar disorder a strong candidate for biologically informed stratification.

### **Genetic architecture of bipolar disorder and remaining ancestry gaps**

Large genomic studies have shown that bipolar disorder is highly polygenic and genetically heterogeneous. The most recent large multi-ancestry GWAS of bipolar disorder analyzed 158,036 cases and 2.8 million controls across European, East Asian, African American, and Latino ancestry groups. It identified 298 genome-wide significant loci and 36 credible genes, and it reported differences in genetic architecture by ascertainment source and bipolar subtype \[3\]. The same study also implicated GABAergic interneurons and medium spiny neurons, giving a strong cell-type context for downstream biological interpretation.

These advances are important, but they do not remove the problem of ancestry imbalance. Most discovery power in psychiatric genetics still comes from European-ancestry cohorts. This affects locus discovery, polygenic risk scoring, TWAS portability, and pathway interpretation. A Korean bipolar disorder GWAS recently identified a genome-wide significant locus in SLC25A12 and showed that multi-ancestry bipolar GWAS data gave the strongest polygenic risk score performance in the Korean sample, supporting the need for ancestry-specific and multi-ancestry analyses rather than simple transfer of European-derived models \[4\].

### **Synaptic dysfunction and excitatory–inhibitory imbalance**

Synaptic biology has become one of the most consistent themes in bipolar disorder genetics and neurobiology. The 2025 bipolar GWAS reported cell-type enrichment in GABAergic interneurons and medium spiny neurons, and broader psychiatric genomics reviews have emphasized that common and rare variant findings are beginning to converge on synaptic, neurodevelopmental, and circuit-level mechanisms \[3,5\]. Owen and colleagues also emphasized that genomic findings are reshaping how schizophrenia, bipolar disorder, and major depressive disorder are understood, including their shared and distinct genetic architectures \[5\].

The GABAergic system is particularly relevant. GABAergic neurons regulate pyramidal cell firing, synchronize cortical networks, and shape cortico-striatal and cortico-limbic signaling. Earlier postmortem and translational work reported downregulation of GAD67 and reelin in schizophrenia and bipolar disorder brains, consistent with impaired GABAergic interneuron function \[6\]. A broader GABAergic deficit framework has also been developed for mood disorders, with reduced GABA levels, altered GABAA receptor composition, stress sensitivity, and antidepressant-related neuroplasticity all forming part of the same biological picture \[7\].

Glutamatergic abnormalities are also relevant. Magnetic resonance spectroscopy and postmortem studies have linked bipolar disorder and related mood states to altered glutamate, glutamine, and receptor biology \[8,9\]. Recent imaging-transcriptomic work in bipolar disorder has further connected functional brain abnormalities to synaptic, neurodevelopmental, and treatment-related molecular pathways \[10,11\].

### **Epigenetic aging and Polycomb-vulnerable synaptic maintenance genes**

A separate but related line of work concerns chromatin regulation in aging neurons. Polycomb repressive complex 2 deposits H3K27me3, a histone mark associated with transcriptional repression and long-term regulation of cell identity programs \[12,13\]. Cheung \[14\] reanalyzed H3K27me3 ChIP-seq data from purified mouse forebrain neurons and described focal Polycomb-mediated repression of neuronal identity and synaptic maintenance genes in aging neurons. In that analysis, 1,500 high-confidence age-associated region–gene assignments were identified, with a strong imbalance toward H3K27me3 gain. The dominant gain modules involved protocadherin and neuronal adhesion genes, synaptic scaffold and neurotransmission genes, and receptor-related pathways, while a smaller loss module involved chromatin, stress, lysosomal, iron-homeostasis, and cytoskeletal genes.

This model is not a claim that aging directly causes bipolar disorder. Rather, it suggests that genes needed for neuronal identity, synaptic stability, and neurotransmission may become epigenetically vulnerable over time. If bipolar genetic liability and age-associated Polycomb remodeling converge on the same synaptic nodes, then TWAS signal may reveal biologically meaningful overlap between inherited risk and neuronal maintenance failure.

### **Rationale and study aims**

The present analysis was designed to test that convergence. We asked whether ancestry-stratified bipolar TWAS signals were closer to Polycomb-derived neuronal aging modules than to a pharmacology-relevant antipsychotic comparator. This comparator was not treated as a negative control in the strict sense, because antipsychotic targets are clinically relevant to bipolar disorder. Instead, it provided a useful benchmark: Polycomb modules had to show stronger transcriptomic proximity than a broad set of known psychiatric drug-related genes.

The study had four aims. First, we characterized ancestry patterns of Polycomb-module enrichment in African, East Asian, and European bipolar TWAS strata. Second, we identified leading-edge genes shared across ancestries and prioritized recurring hubs. Third, we examined whether a compact synaptic subnetwork could be extracted from the shared core. Fourth, we interpreted the findings in relation to ancestry-aware stratification, inhibitory tone, presynaptic calcium signaling, and translational validation.

## **Methods**

### **Data sources**

This was a secondary analysis of ancestry-stratified bipolar disorder TWAS summary statistics. The three analyzed strata were labeled bip\_afr, bip\_eas, and bip\_eur, corresponding to African ancestry, East Asian ancestry, and European ancestry bipolar datasets. These TWAS meta-Z statistics were derived from bipolar disorder genetic resources aligned with the large multi-ancestry GWAS context reported by O’Connell et al. \[3\]. The present work did not use individual-level genotype or phenotype data.

### **Gene-set construction**

Polycomb-derived modules were based on the biological themes described by Cheung \[14\], in which age-associated H3K27me3 remodeling in mouse forebrain neurons was organized into coherent gene programs. These modules were mapped to standardized KEGG pathways for reproducible analysis in human TWAS space.

Module A represented neuronal identity and adhesion biology, including cell adhesion molecules, axon guidance, and adherens junction pathways. In the present human KEGG mapping, these were represented by HSA04514\_CELL\_ADHESION\_MOLECULES\_CAMS, HSA04360\_AXON\_GUIDANCE, and HSA04520\_ADHERENS\_JUNCTION.

Module B represented synaptic scaffold, neurotransmission, and receptor signaling. It included HSA04080\_NEUROACTIVE\_LIGAND\_RECEPTOR\_INTERACTION, HSA04725\_CHOLINERGIC\_SYNAPSE, HSA04724\_GLUTAMATERGIC\_SYNAPSE, HSA04721\_SYNAPTIC\_VESICLE\_CYCLE, HSA04720\_LONG\_TERM\_POTENTIATION, HSA04726\_SEROTONERGIC\_SYNAPSE, and HSA04727\_GABAERGIC\_SYNAPSE.

Module C represented stress, homeostasis, and dual H3K27me3 dynamics, including HSA04142\_LYSOSOME, HSA04216\_FERROPTOSIS, HSA04810\_REGULATION\_OF\_ACTIN\_CYTOSKELETON, HSA03020\_RNA\_POLYMERASE, HSA04614\_RENIN\_ANGIOTENSIN\_SYSTEM, and HSA03040\_SPLICEOSOME.

### **Comparator gene set**

The comparator was an antipsychotic-related gene set generated from DGIdb drug–gene interaction data. Drugs under the antipsychotic ATC class were parsed, drug–gene interaction tables were converted into gene sets, and the resulting genes were flattened into a single antipsychotic-related comparator set. This comparator included broad psychiatric pharmacology targets and was used as a clinically relevant benchmark rather than as an inert background.

### **Analytical pipeline**

The primary enrichment analysis used absolute TWAS meta-Z ranking. For each ancestry, genes were ranked by absolute Z score, and weighted GSEA-like enrichment was performed for each Polycomb-derived pathway and the antipsychotic comparator. Head-to-head testing compared each Polycomb pathway against the antipsychotic gene set within each ancestry. The main differential statistic was dNES, defined as the normalized enrichment score of the Polycomb set minus the normalized enrichment score of the comparator. Permutation testing used 2,000 permutations in the supplied pipeline outputs.

Post-hoc analyses extracted leading-edge genes, tested overlap between Polycomb and antipsychotic leading edges, removed comparator-overlapping genes and retested enrichment, and performed leave-one-out analysis for comparator genes. Stage 4 integrated results across all three ancestries. Stage 5 focused on ancestry-specific divergence, especially European versus non-European effects.

### **Cross-ancestry integration**

Stage 4 evaluated transancestry meta-NES consistency, verdict concordance, shared versus ancestry-specific leading-edge genes, hub recurrence, ancestry-by-set differences in absolute Z distributions, drug-repurposing overlap, and signed-versus-absolute directionality. Stage 5 evaluated European advantage in median absolute Z, ancestry-unique leading-edge genes, differential hub influence, ancestry-stratified drug prioritization, differential repression signatures, European-dominant set ranking, and dNES heterogeneity.

A core gene was defined as a Polycomb leading-edge gene present in all three ancestries. Universal hubs were tracked genes that appeared in the leading edge across all ancestries. A compact GABA/glutamatergic/calcium subnetwork was then extracted from the core list using gene family membership and functional relevance.

### **Directionality and repression testing**

Because the primary analysis used absolute Z scores, a separate signed-Z analysis was performed to test whether the signal reflected directional repression. Directionality was assessed using the proportion of negative signed Z scores within leading-edge genes, mean signed Z, and sign tests. This analysis was treated as mechanistic context rather than as the primary enrichment result.

### **Ethics and data availability**

The analysis used existing summary-level TWAS and derived gene-set outputs. No individual-level data were analyzed. All reported results are based on the supplied pipeline summaries and accompanying output tables.

## **Results**

### **Ancestry-structured enrichment with GABAergic synapse as the standout European-dominant module**

The first major finding was negative in a useful way: no Polycomb pathway beat the antipsychotic comparator in all three ancestries. In Stage 4, 16 Polycomb sets were evaluated. None won across all ancestries, and none passed combined FDR below 0.05. Three pathways showed partial ancestry-level wins: lysosome, adherens junction, and GABAergic synapse. This argues against a simple pan-ancestry claim that Polycomb-derived pathways are globally stronger than antipsychotic-related genes in bipolar TWAS signal. The Stage 4 transancestry meta-NES and consistency results are summarized in Table 1\.

**Table 1\. Stage 4 transancestry meta-NES and consistency of Polycomb sets**

| Polycomb set | Mean NES | NES SD | Mean dNES | Fraction wins | Combined p | FDR | Consistency score |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| HSA04142\_LYSOSOME | 1.115 | 0.038 | 0.170 | 0.333 | 0.0149 | 0.1190 | 0.254 |
| HSA04520\_ADHERENS\_JUNCTION | 1.196 | 0.108 | 0.251 | 0.333 | 0.0090 | 0.1190 | 0.107 |
| HSA03040\_SPLICEOSOME | 1.122 | 0.109 | 0.177 | 0.000 | 0.0494 | 0.2632 | 0.000 |
| HSA04727\_GABAERGIC\_SYNAPSE | 1.118 | 0.159 | 0.173 | 0.333 | 0.0808 | 0.3233 | 0.000 |
| HSA04614\_RENIN\_ANGIOTENSIN\_SYSTEM | 1.086 | 0.110 | 0.141 | 0.000 | 0.2497 | 0.7990 | 0.000 |
| HSA04726\_SEROTONERGIC\_SYNAPSE | 0.988 | 0.117 | 0.042 | 0.000 | 0.5297 | 0.8821 | 0.000 |
| HSA04724\_GLUTAMATERGIC\_SYNAPSE | 0.986 | 0.110 | 0.040 | 0.000 | 0.5234 | 0.8821 | 0.000 |
| HSA04810\_REGULATION\_OF\_ACTIN\_CYTOSKELETON | 0.978 | 0.124 | 0.032 | 0.000 | 0.6479 | 0.8821 | 0.000 |
| HSA03020\_RNA\_POLYMERASE | 0.950 | 0.039 | 0.004 | 0.000 | 0.6443 | 0.8821 | 0.000 |
| HSA04360\_AXON\_GUIDANCE | 0.949 | 0.129 | 0.003 | 0.000 | 0.7652 | 0.8821 | 0.000 |
| HSA04720\_LONG\_TERM\_POTENTIATION | 0.947 | 0.078 | 0.002 | 0.000 | 0.6764 | 0.8821 | 0.000 |
| HSA04721\_SYNAPTIC\_VESICLE\_CYCLE | 0.944 | 0.126 | \-0.002 | 0.000 | 0.7122 | 0.8821 | 0.000 |
| HSA04725\_CHOLINERGIC\_SYNAPSE | 0.940 | 0.091 | \-0.005 | 0.000 | 0.7718 | 0.8821 | 0.000 |
| HSA04216\_FERROPTOSIS | 0.906 | 0.128 | \-0.040 | 0.000 | 0.7652 | 0.8821 | 0.000 |
| HSA04080\_NEUROACTIVE\_LIGAND\_RECEPTOR\_INTERACTION | 0.850 | 0.050 | \-0.095 | 0.000 | 0.9984 | 0.9984 | 0.000 |
| HSA04514\_CELL\_ADHESION\_MOLECULES\_CAMS | 0.842 | 0.091 | \-0.104 | 0.000 | 0.9832 | 0.9984 | 0.000 |

The more informative pattern appeared in Stage 5\. All 16 Polycomb pathways had higher median absolute Z in the European stratum than in the average of the African and East Asian strata. The largest European median absolute-Z advantages were seen for renin–angiotensin system, serotonergic synapse, GABAergic synapse, glutamatergic synapse, cell adhesion molecules, and axon guidance. The numerical European advantage was strongest for HSA04614\_RENIN\_ANGIOTENSIN\_SYSTEM, but this pathway did not meet the strict European-dominant dNES criterion and had a very small leading edge in the European post-hoc run. The GABAergic synapse pathway was therefore the clearest ancestry-structured synaptic signal. The Stage 5 European versus non-European absolute-Z differential results are summarized in Table 2\.

**Table 2\. Stage 5 ancestry-specific absolute-Z differential: European versus mean non-European**

| Set | EUR | AFR | EAS | Mean non-EUR | EUR advantage | Kruskal p |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| HSA04614\_RENIN\_ANGIOTENSIN\_SYSTEM | 7.82 | 1.36 | 3.48 | 2.42 | 5.40 | 0.0662 |
| HSA04726\_SEROTONERGIC\_SYNAPSE | 4.72 | 1.87 | 1.39 | 1.63 | 3.09 | 0.0000 |
| HSA04727\_GABAERGIC\_SYNAPSE | 4.19 | 1.49 | 2.02 | 1.75 | 2.43 | 0.0000 |
| HSA04724\_GLUTAMATERGIC\_SYNAPSE | 3.71 | 1.45 | 2.16 | 1.81 | 1.91 | 0.0000 |
| HSA04514\_CELL\_ADHESION\_MOLECULES\_CAMS | 3.13 | 1.50 | 1.99 | 1.75 | 1.38 | 0.0000 |
| HSA04360\_AXON\_GUIDANCE | 3.13 | 1.89 | 1.70 | 1.80 | 1.34 | 0.0000 |
| HSA04725\_CHOLINERGIC\_SYNAPSE | 3.29 | 2.61 | 1.45 | 2.03 | 1.26 | 0.0000 |
| HSA04520\_ADHERENS\_JUNCTION | 3.65 | 1.64 | 3.23 | 2.43 | 1.22 | 0.0000 |
| HSA04720\_LONG\_TERM\_POTENTIATION | 3.23 | 1.84 | 2.23 | 2.03 | 1.20 | 0.0008 |
| HSA04142\_LYSOSOME | 3.36 | 2.05 | 2.27 | 2.16 | 1.20 | 0.0000 |
| HSA03020\_RNA\_POLYMERASE | 2.59 | 1.50 | 1.40 | 1.45 | 1.13 | 0.0285 |
| HSA04810\_REGULATION\_OF\_ACTIN\_CYTOSKELETON | 2.61 | 1.81 | 1.47 | 1.64 | 0.97 | 0.0000 |
| HSA04216\_FERROPTOSIS | 2.64 | 1.59 | 1.76 | 1.68 | 0.96 | 0.0236 |
| HSA04721\_SYNAPTIC\_VESICLE\_CYCLE | 2.55 | 1.28 | 1.94 | 1.61 | 0.94 | 0.0001 |
| HSA04080\_NEUROACTIVE\_LIGAND\_RECEPTOR\_INTERACTION | 2.37 | 1.38 | 1.64 | 1.51 | 0.86 | 0.0000 |
| HSA03040\_SPLICEOSOME | 2.99 | 2.33 | 2.06 | 2.20 | 0.80 | 0.0000 |

In the head-to-head European analysis, HSA04727\_GABAERGIC\_SYNAPSE had NES 1.3334, p \= 0.010495, compared with antipsychotic comparator NES 1.0498, p \= 0.272864, yielding dNES 0.2836 and a “set1\_beats\_set2” verdict. In Stage 5, it was the only pathway meeting the prespecified European-dominant rule: dNES\_eur 0.284, non-European mean dNES 0.117, European dNES advantage 0.166, and European p \= 0.0105. By comparison, adherens junction also performed strongly in the European stratum, with NES 1.3283 and p \= 0.006497, but its non-European dNES mean was also high, so it did not meet the same divergence criterion.

The GABAergic synapse result was not explained simply by overlap with antipsychotic leading-edge genes. In African and East Asian strata, GABAergic synapse had no leading-edge overlap with the antipsychotic comparator. In the European stratum, overlap was limited to GNB3 and SRC. After removal of antipsychotic comparator genes, the European GABAergic synapse pathway remained significant, with clean NES 1.331 and p \= 0.010495, still exceeding the comparator NES of 1.0545. This supports a signal that is related to bipolar synaptic biology rather than merely reflecting known antipsychotic targets.

The same pattern was weaker outside the European stratum. In African ancestry data, GABAergic synapse had NES 0.9537, p \= 0.613693, and dNES 0.0615. In East Asian ancestry data, it had NES 1.0680, p \= 0.342829, and dNES 0.1729. Thus, the direction of effect was not absent in East Asian data, but the signal did not meet enrichment significance or comparator dominance. This distinction is important. The finding should not be read as proof of European-specific biology. It may reflect greater European statistical power, better TWAS model fit, ancestry-specific architecture, or some combination of these.

### **Sixty-nine core genes shared across ancestries and five universal hubs**

The second major finding was cross-ancestry convergence at the gene level. Across all Polycomb leading edges, Stage 4 identified 815 unique leading-edge genes. Of these, 69 were present in all three ancestries, and 284 were shared by exactly two ancestries. Stage 5 identified 462 ancestry-unique leading-edge genes: 127 African-only, 133 East Asian-only, and 202 European-only. The larger number of European-only genes is consistent with the stronger European signal, but it also raises the possibility of power-driven discovery bias. The shared and ancestry-specific leading-edge structure is summarized in Table 3\.

**Table 3\. Stage 4 shared and ancestry-specific leading-edge gene structure**

| Category | Count | Genes or summary |
| ----- | ----- | ----- |
| Total unique Polycomb leading-edge genes | 815 | All Polycomb leading-edge genes across AFR, EAS, and EUR |
| Core genes present in all three ancestries | 69 | ACP5; ACSL6; AGA; AP2A2; ARPC2; ARPC5L; ATP6V1G2; BDKRB2; CACNA1B; CALCB; CDC40; CGA; CHRNA10; CHRNA4; CHRND; CLTCL1; CPLX2; CPLX3; CREB3L4; CTNND1; CWC25; DRD2; EPHB6; F2RL1; GAA; GABRA6; GABRB2; GLRA3; GNRH1; GNRH2; GNRHR; GRID1; GRIK2; GRM3; ITGA1; ITGA3; ITGA5; KISS1; LIMK1; MAP1LC3B2; MYH10; MYH14; MYL12A; NMB; NTN4; OSBPL7; P2RX2; P2RX4; P2RY11; PAQR6; PDGFRB; PLCB3; POLR2C; POLR2H; PRLHR; RHOA; RRAS2; RXFP1; SLC1A7; SLC38A3; SNAI1; SUMF1; TAC3; TLR9; TTI1; VPS29; VPS39; WASF1; WBP11 |
| Genes shared in exactly two ancestries | 284 | First 30 reported: ABAT; ABCB9; ABLIM1; ACE; ACP1; ACSL1; ACSL5; ACTB; ACTN4; ADCY4; ADCY6; ADCY7; ADORA2A; ADORA3; ADRA2A; ADRA2B; AGT; AKT1; AP1B1; AP1M1; AP1M2; AP3B2; AP3S2; AP4M1; AP5B1; APLNR; AQR; ARHGEF12; ARHGEF7; ARPC5 |
| Tracked hubs among core genes | 5 | CACNA1B; DRD2; GABRA6; GABRB2; LIMK1 |

The 69 core genes were ACP5, ACSL6, AGA, AP2A2, ARPC2, ARPC5L, ATP6V1G2, BDKRB2, CACNA1B, CALCB, CDC40, CGA, CHRNA10, CHRNA4, CHRND, CLTCL1, CPLX2, CPLX3, CREB3L4, CTNND1, CWC25, DRD2, EPHB6, F2RL1, GAA, GABRA6, GABRB2, GLRA3, GNRH1, GNRH2, GNRHR, GRID1, GRIK2, GRM3, ITGA1, ITGA3, ITGA5, KISS1, LIMK1, MAP1LC3B2, MYH10, MYH14, MYL12A, NMB, NTN4, OSBPL7, P2RX2, P2RX4, P2RY11, PAQR6, PDGFRB, PLCB3, POLR2C, POLR2H, PRLHR, RHOA, RRAS2, RXFP1, SLC1A7, SLC38A3, SNAI1, SUMF1, TAC3, TLR9, TTI1, VPS29, VPS39, WASF1, and WBP11.

Five tracked hubs appeared in the leading edge across all three ancestries: CACNA1B, DRD2, GABRA6, GABRB2, and LIMK1. These hubs connect inhibitory signaling, presynaptic calcium entry, dopamine modulation, and cytoskeletal plasticity. GABRA6 had the highest mean maximum absolute Z among universal hubs, with mean max |Z| 5.902 and maximum 9.414. GABRB2 had mean max |Z| 4.530 and maximum 8.198. CACNA1B had mean max |Z| 3.512 and maximum 7.762. LIMK1 had mean max |Z| 3.213 and maximum 5.520. DRD2 had lower mean magnitude, at 2.053, but its recurrence across all ancestries is notable because it links the Polycomb-derived signal to dopaminergic pharmacology. The full tracked hub prioritization results are shown in Table 4\.

**Table 4\. Stage 4 transancestry hub-gene prioritization**

| Gene | Ancestries in LE | Mean max |Z| | Max max |Z| | Mean signed Z |
| ----- | ----- | ----- | ----- | ----- |
| GABRA6 | 3 | 5.902 | 9.414 | \-5.128 |
| GABRB2 | 3 | 4.530 | 8.198 | 4.530 |
| CACNA1B | 3 | 3.512 | 7.762 | 2.669 |
| LIMK1 | 3 | 3.213 | 5.520 | \-3.213 |
| DRD2 | 3 | 2.053 | 2.708 | \-2.053 |
| HTR6 | 2 | 7.225 | 12.129 | 7.225 |
| MAPK3 | 2 | 6.569 | 10.557 | 6.569 |
| CYP2D6 | 2 | 5.838 | 6.977 | \-5.838 |
| RPTOR | 2 | 5.562 | 9.148 | \-3.585 |
| GLS2 | 2 | 3.655 | 5.339 | \-1.684 |
| CTNNB1 | 2 | 3.544 | 5.363 | 1.819 |
| CHRM5 | 2 | 2.071 | 3.126 | \-1.055 |
| SF3B1 | 1 | 9.358 | 9.358 | 9.358 |
| GNB3 | 1 | 7.815 | 7.815 | \-7.815 |
| FYN | 1 | 7.479 | 7.479 | \-7.479 |
| MAPK1 | 1 | 5.357 | 5.357 | 5.357 |
| GSK3B | 1 | 3.111 | 3.111 | 3.111 |
| ANK3 | 0 | NA | NA | NA |

The ancestry-differential hub analysis showed that several hubs were especially high in the European stratum. European-high hubs above |Z| 5 included HTR6, MAPK3, GABRA6, SF3B1, RPTOR, GABRB2, GNB3, CACNA1B, FYN, CYP2D6, LIMK1, CTNNB1, MAPK1, and GLS2. The most cross-ancestry-divergent hubs by absolute-Z range were HTR6, GABRA6, MAPK3, RPTOR, and GABRB2. These results again support a mixture of convergence and ancestry-structured magnitude differences.

### **Compact GABA/glutamatergic/calcium signaling subnetwork**

The third major finding was the extraction of a compact seven-gene subnetwork from the 69-gene core. This subnetwork comprised CACNA1B, GABRA6, GABRB2, GRIK2, GRM3, SLC1A7, and SLC38A3. It is biologically coherent because it spans postsynaptic inhibition, presynaptic release, glutamate and glutamine handling, and modulatory glutamate receptor signaling. The validation-ready GABA/glutamatergic/calcium subnetwork is summarized in Table 5\.

**Table 5\. Stage 5 GABA/glutamatergic/calcium subnetwork for validation**

| Gene | Family | AFR |Z| | EAS |Z| | EUR |Z| | Mean max |Z| |
| ----- | ----- | ----- | ----- | ----- | ----- |
| CACNA1B | Calcium channel | 1.51 | 1.26 | 7.76 | 3.51 |
| GABRA6 | GABAergic | 1.16 | 7.13 | 9.41 | 5.90 |
| GABRB2 | GABAergic | 1.05 | 4.35 | 8.20 | 4.53 |
| SLC38A3 | Glutamatergic | 2.74 | 5.12 | 7.13 | 4.99 |
| GRIK2 | Glutamatergic | 1.44 | 1.54 | 3.71 | 2.23 |
| GRM3 | Glutamatergic | 0.92 | 1.75 | 2.46 | 1.71 |
| SLC1A7 | Glutamatergic | 1.38 | 1.73 | 1.75 | 1.62 |

GABRA6 and GABRB2 encode GABAA receptor subunits and represent the most direct inhibitory signaling component of the subnetwork. GABRA6 showed ancestry-specific maximum absolute Z values of 1.16 in African ancestry, 7.13 in East Asian ancestry, and 9.41 in European ancestry, with mean max |Z| 5.90. GABRB2 showed 1.05, 4.35, and 8.20 across the same ancestries, with mean max |Z| 4.53. These two genes anchor the GABAergic synapse finding and are consistent with broader evidence that GABAA receptor composition and GABAergic signal transduction are relevant to psychiatric illness \[15-17\].

CACNA1B encodes the Cav2.2 N-type voltage-gated calcium channel alpha subunit. It is central to presynaptic calcium entry and neurotransmitter release. In the present analysis, CACNA1B was a universal hub and part of the core subnetwork, with maximum absolute Z values of 1.51, 1.26, and 7.76 in African, East Asian, and European strata. This pattern supports the idea that bipolar TWAS signal may intersect with presynaptic release machinery, not only postsynaptic receptor biology. Cav2 channels are well established regulators of neurotransmitter release and presynaptic plasticity \[18,19\].

SLC38A3 encodes a glutamine transporter involved in nitrogen and glutamine handling. It had maximum absolute Z values of 2.74, 5.12, and 7.13 across African, East Asian, and European strata. Its inclusion is important because the glutamate–glutamine cycle links astrocytic and neuronal metabolism to both glutamate and GABA synthesis \[20,21\]. SLC1A7, GRIK2, and GRM3 add glutamate clearance and modulatory receptor components \[22,23\]. GRIK2 had values of 1.44, 1.54, and 3.71; GRM3 had 0.92, 1.75, and 2.46; SLC1A7 had 1.38, 1.73, and 1.75. These are more modest than GABRA6, GABRB2, CACNA1B, and SLC38A3, but they help complete an excitatory–inhibitory balance model.

### **Secondary findings: directionality and drug overlap**

The signed-Z analyses did not support a strong uniform repression model across ancestries. Stage 4 found no Polycomb pathway with strong repression support, defined as negative signed-Z skew significant in at least two ancestries. RNA polymerase and regulation of actin cytoskeleton showed only moderate repression support. In Stage 5, East Asian ancestry had the highest mean percentage of negative signed Z values across sets, but no significant negative-skew sets. European ancestry showed a specific negative skew for RNA polymerase, with 100% negative leading-edge Z values and mean Z \-3.5305. Overall, the evidence is stronger for magnitude-based proximity than for uniform directional repression.

The drug-repurposing screen recovered many compounds, including expected psychiatric agents. Stage 4 identified 7,510 distinct drugs hitting leading-edge genes in at least one ancestry and 6,648 recurring across all three ancestries. Eight known psychiatric or bipolar-relevant drugs were recovered across ancestries: olanzapine, clozapine, risperidone, valproic acid, lamotrigine, carbamazepine, aripiprazole, and lithium carbonate. This provides face validity for the gene-set approach, but it should not be interpreted as a treatment recommendation. Many top-ranked compounds were oncology or broad-target drugs, such as doxorubicin, cisplatin, sorafenib, dasatinib, and fluorouracil, which likely reflect database connectivity rather than clinical suitability. The top recurrent transancestry drug-repurposing overlaps are shown in Table 6\.

**Table 6\. Stage 4 transancestry drug-repurposing overlap, top recurrent candidates**

| Drug | Ancestries | Total targets | Mean targets | Mean score | Known psych/BD drug |
| ----- | ----- | ----- | ----- | ----- | ----- |
| HALOPERIDOL DECANOATE | 3 | 77 | 25.67 | 0.302 | No |
| OLANZAPINE | 3 | 76 | 25.33 | 0.124 | Yes |
| DOXORUBICIN HYDROCHLORIDE | 3 | 75 | 25.00 | 0.033 | No |
| CISPLATIN | 3 | 66 | 22.00 | 0.038 | No |
| CLOZAPINE | 3 | 65 | 21.67 | 0.040 | Yes |
| SORAFENIB | 3 | 56 | 18.67 | 0.032 | No |
| DASATINIB ANHYDROUS | 3 | 55 | 18.33 | 0.115 | No |
| FLUOROURACIL | 3 | 55 | 18.33 | 0.098 | No |
| CYCLOSPORINE | 3 | 49 | 16.33 | 0.159 | No |
| QUERCETIN | 3 | 49 | 16.33 | 0.088 | No |
| RISPERIDONE | 3 | 49 | 16.33 | 0.085 | Yes |
| CELECOXIB | 3 | 45 | 15.00 | 0.038 | No |
| ILORASERTIB | 3 | 45 | 15.00 | 0.011 | No |
| ASPIRIN | 3 | 42 | 14.00 | 0.050 | No |
| DEHYDRATED ALCOHOL | 3 | 42 | 14.00 | 0.177 | No |
| VANDETANIB | 3 | 42 | 14.00 | 0.102 | No |
| CHLORPROMAZINE | 3 | 40 | 13.33 | 0.066 | No |
| DACTOLISIB | 3 | 40 | 13.33 | 0.062 | No |
| CYCLOPHOSPHAMIDE ANHYDROUS | 3 | 39 | 13.00 | 0.113 | No |
| GOSSYPOL | 3 | 39 | 13.00 | 0.040 | No |

## **Discussion**

### **Principal findings in clinical context**

This analysis does not support a simple claim that Polycomb-derived neuronal aging modules outperform antipsychotic-related genes across all ancestries in bipolar disorder. The Stage 4 results were clear: no pathway won in every ancestry, and no pathway passed combined FDR. That negative result is important because it protects against overinterpretation. Bipolar disorder is genetically and clinically heterogeneous, and a model that claims a single pathway dominates across ancestries would not fit the data.

The stronger finding is more nuanced. Bipolar TWAS signal showed ancestry-structured convergence on Polycomb-vulnerable synaptic maintenance pathways, with the most interpretable signal in the European stratum and centered on the GABAergic synapse pathway. The same analysis also identified a cross-ancestry core of 69 leading-edge genes and five universal hubs. These results suggest that ancestry-specific magnitude differences and transancestry gene-level recurrence can coexist.

Clinically, this is relevant because bipolar disorder is not only a disorder of episodic mood change. It often involves persistent cognitive, motivational, and functional impairment. Synaptic maintenance failure, altered inhibitory control, and disrupted calcium-dependent neurotransmission provide a plausible bridge between molecular liability and clinical heterogeneity. The findings also align with the broader genomic observation that bipolar disorder risk is enriched in GABAergic interneurons and medium spiny neurons \[3\].

### **Mechanistic integration: Polycomb vulnerability and synaptic maintenance**

The Polycomb model used here comes from the idea that aging neurons may undergo focal redistribution of H3K27me3 rather than a simple global loss of repression. Cheung \[14\] described dominant H3K27me3 gain at neuronal identity, cell adhesion, synaptic scaffold, and neurotransmission genes, with smaller H3K27me3 loss at stress and homeostasis genes. In the present bipolar TWAS analysis, the most clinically relevant overlap was not the full Polycomb space but a specific synaptic segment of it.

The GABAergic synapse pathway is the best example. GABRA6 and GABRB2 were both core genes and universal cross-ancestry hubs. These genes encode GABAA receptor subunits, and GABAA receptor subunit composition affects inhibitory signaling, receptor localization, and pharmacological sensitivity \[16,17,26\]. If genetic liability and epigenetic vulnerability converge on these genes, the result may be reduced stability of inhibitory signaling rather than a simple increase or decrease in one neurotransmitter.

CACNA1B adds a presynaptic layer. Cav2.2 channels regulate calcium entry at nerve terminals and thereby influence neurotransmitter release probability. In a circuit-level model, altered CACNA1B function could impair GABA release from interneurons, glutamate release from excitatory neurons, or both, depending on cell type and synaptic context. The convergence of CACNA1B with GABAA receptor subunits suggests that the signal is not limited to receptor expression. It may involve the full chain from presynaptic release to postsynaptic inhibition.

The glutamatergic members of the subnetwork add another layer. SLC38A3 supports glutamine transport and therefore the metabolic supply line for glutamate and GABA synthesis. SLC1A7 relates to glutamate transport. GRIK2 and GRM3 represent ionotropic and metabotropic glutamate receptor systems. Together, these genes describe an excitatory–inhibitory balance module rather than a purely GABAergic module.

LIMK1 provides a structural plasticity connection. LIMK1 regulates actin dynamics through cofilin phosphorylation and is relevant to dendritic spine remodeling and synaptic plasticity \[24,25\]. Its recurrence across all three ancestries links the synaptic signaling findings to structural maintenance of synapses. DRD2, meanwhile, connects the core gene set to dopaminergic modulation and antipsychotic pharmacology. This is not surprising, but it is useful: the analysis does not separate disease biology and pharmacology into unrelated categories. Instead, it shows that some genes sit at their intersection.

### **Relation to existing bipolar biology**

The findings fit several strands of bipolar disorder biology. First, they are consistent with genomic studies implicating GABAergic interneurons, medium spiny neurons, and synaptic biology \[3,5\]. Second, they align with postmortem and neurochemical studies suggesting GABAergic and glutamatergic abnormalities in mood disorders \[6,7,9\]. Third, they are compatible with imaging-transcriptomic studies showing that bipolar disorder brain network abnormalities can map onto synaptic and neurodevelopmental gene expression programs \[10,11\].

The present analysis adds a specific interpretation: inherited bipolar transcriptomic risk may intersect with genes that are vulnerable to age-associated Polycomb remodeling. This does not mean that bipolar disorder is a disease of aging, nor does it imply that all patients share the same mechanism. It suggests that synaptic maintenance genes may be a shared vulnerability point, where genetic liability, chromatin regulation, and circuit function meet.

### **Addressing treatment heterogeneity and ancestry gaps**

One of the practical difficulties in bipolar disorder is that treatment selection is still largely empirical. The recovery of known bipolar and psychiatric drugs in the drug-overlap analysis gives some confidence that the pipeline is capturing clinically relevant biology. However, the drug results should be treated as a prioritization tool rather than a prescribing guide. Broad-target oncology compounds ranked highly because they hit many genes in databases, not because they are plausible bipolar treatments.

The more useful translational output is the core gene and subnetwork structure. A biomarker panel based on CACNA1B, GABRA6, GABRB2, DRD2, LIMK1, and the seven-gene inhibitory/glutamatergic/calcium subnetwork could be tested in future studies as a stratification tool. Such a panel would not diagnose bipolar disorder by itself. Rather, it could help identify a subgroup in which inhibitory signaling, presynaptic calcium dynamics, and glutamate–GABA cycling are especially relevant.

The ancestry findings are also clinically important. The European-dominant signal should be interpreted cautiously because European cohorts often have greater discovery power and better-matched transcriptomic prediction models. The East Asian GABAergic signal was present but weaker, and the African ancestry signal was weaker still. This could reflect true biological differences, but it could also reflect sample size, reference-panel mismatch, TWAS model portability, or differences in imputation and tissue prediction accuracy. The Korean GWAS findings reinforce the need for ancestry-matched genomic resources and multi-ancestry modeling rather than direct transfer of European-derived findings \[4\].

### **Translational roadmap**

The most immediate next step is not clinical implementation but validation. The 69 core genes should be overlapped with credible genes from the O’Connell et al. bipolar GWAS and with cell-type-specific expression resources. The seven-gene subnetwork should be tested in iPSC-derived neurons, especially GABAergic interneuron-like cells, glutamatergic neurons, and cortico-striatal models. CRISPR interference, CRISPR activation, or epigenome editing could test whether changing Polycomb regulation at these loci alters receptor expression, calcium transients, synaptic vesicle release, or excitatory–inhibitory balance.

Postmortem validation would also be valuable. If the model is correct, one might expect altered expression or chromatin marks at GABRA6, GABRB2, CACNA1B, SLC38A3, and related genes in bipolar disorder brain regions involved in mood regulation, cognition, and reward. Such work should be ancestry-aware wherever possible, because the current analysis suggests that magnitude and pathway ranking differ by ancestry.

For clinical trials, these genes could inform stratification rather than direct treatment selection. Patients with higher burden or stronger transcriptomic signal in the inhibitory/calcium subnetwork might be studied separately in trials targeting synaptic plasticity, inhibitory tone, glutamatergic modulation, or presynaptic calcium-dependent signaling. Neuromodulation studies could also incorporate these gene sets, because cortical excitability and inhibition measures may provide a functional readout of excitatory–inhibitory balance. TMS studies in mood disorders already support the usefulness of probing cortical reactivity and inhibition as translational physiology \[27\].

The same framework may help refine adjunctive treatment development. Network meta-analytic work has examined adjunctive anti-inflammatory agents in bipolar disorder, and oxidative stress and inflammation remain relevant to bipolar treatment research \[28\]. The present findings do not show that any adjunctive strategy should be used for a genetically defined subgroup. They do suggest that future adjunctive trials may benefit from measuring synaptic, inflammatory, and metabolic biomarkers together rather than treating them as separate domains.

### **Limitations**

Several limitations are central. First, the strongest signal was European-dominant. This may reflect biology, but it may also reflect statistical power and TWAS model portability. Larger African and East Asian bipolar TWAS datasets are needed before ancestry-specific conclusions can be made confidently.

Second, TWAS does not prove causal gene expression effects. A TWAS signal may reflect linkage disequilibrium, shared eQTL architecture, correlated expression, or model features rather than direct causal expression changes. Locus-level colocalization and fine mapping are needed before individual genes can be treated as causal targets.

Third, the Polycomb modules were derived from mouse neuronal aging data and mapped onto human KEGG pathways. This is a strength for hypothesis generation but also a limitation. Human validation is needed, ideally using single-cell or cell-type-specific chromatin and expression data from relevant brain regions.

Fourth, the primary signal was based on absolute Z ranking. This was appropriate for detecting magnitude-based proximity, but it does not establish whether genes are upregulated or downregulated. The signed-Z analysis did not show strong uniform repression across ancestries. Therefore, the most defensible interpretation is convergence on Polycomb-vulnerable genes, not proof of directional Polycomb repression in bipolar disorder.

Fifth, the antipsychotic comparator is broad and biologically heterogeneous. Some overlap with Polycomb pathways is expected because psychiatric drug targets include neurotransmitter receptors, kinases, transporters, and signaling proteins. The comparator is clinically useful, but it is not a perfect control.

### **Future directions**

Future work should prioritize four directions. First, larger non-European bipolar TWAS studies are needed, with ancestry-matched expression weights and harmonized phenotype definitions. Second, the 69 core genes and seven-gene subnetwork should be tested against credible bipolar GWAS loci, rare variant findings, and single-cell enrichment maps. Third, functional experiments should examine whether Polycomb perturbation at these loci changes inhibitory signaling, calcium-dependent release, or glutamate–GABA cycling. Fourth, clinical studies should test whether synaptic subnetwork burden relates to cognition, treatment response, cortical inhibition, or longitudinal functional outcomes.

## **Conclusion**

This transancestral TWAS gene-set analysis found no uniform pan-ancestry superiority of Polycomb-derived neuronal aging modules over antipsychotic-related genes in bipolar disorder. Its main contribution is more specific: bipolar TWAS signal showed ancestry-structured convergence on Polycomb-vulnerable synaptic maintenance pathways, with the GABAergic synapse pathway emerging as the clearest European-dominant module. Across ancestries, 69 core leading-edge genes were shared, anchored by CACNA1B, DRD2, GABRA6, GABRB2, and LIMK1. Within this core, CACNA1B, GABRA6, GABRB2, GRIK2, GRM3, SLC1A7, and SLC38A3 formed a compact GABA/glutamatergic/calcium signaling subnetwork.

The findings support a model in which bipolar genetic liability intersects with synaptic maintenance nodes vulnerable to epigenetic aging processes. This model is not ready for clinical use, but it offers a focused path for validation. The most important next steps are ancestry-aware replication, locus-level causal inference, single-cell functional studies, and translational work linking the core subnetwork to inhibitory physiology, cognitive impairment, and treatment heterogeneity.

## **References**

1. Cheng CM, Chang WH, Lin YT, et al; TSBPN Bipolar Taskforce. Taiwan consensus on biological treatment of bipolar disorder during the acute, maintenance, and mixed phases: the 2022 update. *Asian J Psychiatry*. 2023;82:103480. doi:10.1016/j.ajp.2023.103480

2. Lin C, Lin YP, Park SC, et al. Long-acting injectable antipsychotic use in patients with bipolar disorder: findings from the REAP-BD study. *Asian J Psychiatry*. 2025;103:104338. doi:10.1016/j.ajp.2024.104338

3. O’Connell KS, Koromina M, van der Veen T, et al; Bipolar Disorder Working Group of the Psychiatric Genomics Consortium. Genomics yields biological and phenotypic insights into bipolar disorder. *Nature*. 2025;639(8056):968-975. doi:10.1038/s41586-024-08468-9

4. Choi MJ, Kim Y, Lee HJ, et al. Genome-wide association study and polygenic risk score analysis for bipolar disorder in the Korean population. *Asian J Psychiatry*. 2026;122:105034. doi:10.1016/j.ajp.2026.105034

5. Owen MJ, Bray NJ, Walters JTR, O’Donovan MC. Genomics of schizophrenia, bipolar disorder and major depressive disorder. *Nat Rev Genet*. 2025;26:862-877. doi:10.1038/s41576-025-00843-0

6. Guidotti A, Auta J, Davis JM, et al. GABAergic dysfunction in schizophrenia: new treatment strategies on the horizon. *Psychopharmacology (Berl)*. 2005;180(2):191-205. doi:10.1007/s00213-005-2212-8

7. Luscher B, Shen Q, Sahir N. The GABAergic deficit hypothesis of major depressive disorder. *Mol Psychiatry*. 2011;16(4):383-406. doi:10.1038/mp.2010.120

8. Beneyto M, Meador-Woodruff JH, Lewis DA. Glutamate receptor expression in the prefrontal cortex of schizophrenic and bipolar subjects. *Neuropsychopharmacology*. 2007;32(9):1888-1902. doi:10.1038/sj.npp.1301313

9. Yüksel C, Öngür D. Magnetic resonance spectroscopy studies of glutamate-related abnormalities in mood disorders. *Biol Psychiatry*. 2010;68(9):785-794. doi:10.1016/j.biopsych.2010.06.016

10. Zhang C, Zhang L, Liang J, et al. Treatment-related changes in functional connectivity of anterior cingulate cortex subregions and their genetic associations in bipolar disorder. *Asian J Psychiatry*. 2026;120:105002. doi:10.1016/j.ajp.2026.105002

11. Zhang C, Zhang L, Liang J, et al. Dynamic ALFF and dynamic ReHo in bipolar disorder: genetic links and predictive value for diagnosis and therapy. *Asian J Psychiatry*. 2025;114:104764. doi:10.1016/j.ajp.2025.104764

12. Margueron R, Reinberg D. The Polycomb complex PRC2 and its mark in life. *Nature*. 2011;469(7330):343-349. doi:10.1038/nature09784

13. Schuettengruber B, Bourbon HM, Di Croce L, Cavalli G. Genome regulation by Polycomb and Trithorax: 70 years and counting. *Cell*. 2017;171(1):34-57. doi:10.1016/j.cell.2017.08.002

14. Cheung N. Focal Polycomb-mediated repression of neuronal identity and synaptic maintenance genes in aging neurons. *Cureus*. 2026;18(6):e111824. doi:10.7759/cureus.111824

15. Craddock N, Jones L, Jones IR, et al. Strong genetic evidence for a selective influence of GABAA receptors on a component of the bipolar disorder phenotype. *Mol Psychiatry*. 2010;15(2):146-153. doi:10.1038/mp.2008.66

16. Olsen RW, Sieghart W. International Union of Pharmacology. LXX. Subtypes of gamma-aminobutyric acid(A) receptors: classification on the basis of subunit composition, pharmacology, and function. Update. *Pharmacol Rev*. 2008;60(3):243-260. doi:10.1124/pr.108.00505

17. Möhler H. GABAA receptor diversity and pharmacology. *Cell Tissue Res*. 2006;326(2):505-516. doi:10.1007/s00441-006-0284-3

18. Catterall WA, Few AP. Calcium channel regulation and presynaptic plasticity. *Neuron*. 2008;59(6):882-901. doi:10.1016/j.neuron.2008.09.005

19. Dolphin AC, Lee A. Presynaptic calcium channels: specialized control of synaptic neurotransmitter release. *Nat Rev Neurosci*. 2020;21(4):213-229. doi:10.1038/s41583-020-0278-2

20. Bak LK, Schousboe A, Waagepetersen HS. The glutamate/GABA-glutamine cycle: aspects of transport, neurotransmitter homeostasis and ammonia transfer. *J Neurochem*. 2006;98(3):641-653. doi:10.1111/j.1471-4159.2006.03913.x

21. Rubio-Aliaga I, Wagner CA. Regulation and function of the SLC38A3/SNAT3 glutamine transporter. *Channels (Austin)*. 2016;10(6):440-452. doi:10.1080/19336950.2016.1207024

22. Danbolt NC. Glutamate uptake. *Prog Neurobiol*. 2001;65(1):1-105. doi:10.1016/S0301-0082(00)00067-8

23. Tzingounis AV, Wadiche JI. Glutamate transporters: confining runaway excitation by shaping synaptic transmission. *Nat Rev Neurosci*. 2007;8(12):935-947. doi:10.1038/nrn2274

24. Bosch M, Castro J, Saneyoshi T, Matsuno H, Sur M, Hayashi Y. Structural and molecular remodeling of dendritic spine substructures during long-term potentiation. *Neuron*. 2014;82(2):444-459. doi:10.1016/j.neuron.2014.03.021

25. Ben Zablah Y, Zhang H, Gugustea R, Jia Z. LIM-kinases in synaptic plasticity, memory, and brain diseases. *Cells*. 2021;10(8):2079. doi:10.3390/cells10082079

26. Rudolph U, Knoflach F. Beyond classical benzodiazepines: novel therapeutic potential of GABAA receptor subtypes. *Nat Rev Drug Discov*. 2011;10(9):685-697. doi:10.1038/nrd3502

27. Reddy PV, Basavaraju R, Sanjay TN, et al. Investigational applications of transcranial magnetic stimulation in mood disorders: studies from a tertiary care center in India. *Asian J Psychiatry*. 2024;97:104054. doi:10.1016/j.ajp.2024.104054

28. Xu H, Du Y, Wang Q, et al. Comparative efficacy, acceptability, and tolerability of adjunctive anti-inflammatory agents on bipolar disorder: a systematic review and network meta-analysis. *Asian J Psychiatry*. 2023;80:103394. doi:10.1016/j.ajp.2022.103394

