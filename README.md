# Primer3-dependent-assay-design-pipeline
Primer3 dependent assay design such as PCR

# Assay Design Pipeline

**General requirements:**
- Amplicons 200 bp in length
- Primers and probes between 18-32 bp, optimal size 24 bp in length
- Annealing temp: 56 C

**Reaction constants:**
- Expected input DNA concentration: 100 nM
- Monovalent Cations: 50 mM
- Divalent Cations: 4.5 mM
- dNTP: 0.8 uM

**Quality control:**
- Avoid user-specified recognition sites of restriction enzymes ‘CviAII’, ‘FatI’, ‘Hpy188III’, ‘NlaIII’ ‘CviQI’, ‘RsaI’
- Filter the primers and probes have G/C clamps
- Filter any oligos with more than 4 consecutive repeated bases
- Remove any primers and probes that will create heterodimers in the range of 55-70 C

**Result ranking:**
- Results should be ranked by primers and probes of the optimal size, followed by the Tm of the primers and probes - closest to the user specified annealing temperature.

**What to return:**
- Forward primer sequence and Tm
- Reverse primer sequence and Tm
- Probe sequence and Tm
- Tm at which these primers and probes will have homodimers
- Amplicon sequence
