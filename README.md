# Primer3-dependent-assay-design-pipeline
Primer3 dependent assay design such as PCR. Change your settings based on your own needs.

# Assay Design Pipeline

**General requirements:**
- Amplicons 100 bp in length
- Primers and probes between 17-35 bp, optimal size 25 bp in length
- Annealing temp: 60 C

**Reaction constants:**
- Expected input DNA concentration: 200 nM
- Monovalent Cations: 50 mM
- Divalent Cations: 4.7 mM
- dNTP: 0.95 uM

**Quality control:**
- Avoid user-specified recognition sites of restriction enzymes ‘CviAII’, ‘FatI’, ‘Hpy188III’, ‘NlaIII’ ‘CviQI’, ‘RsaI’
- Filter the primers and probes have G/C clamps
- Filter any oligos with more than 3 consecutive repeated bases
- Remove any primers and probes that will create heterodimers in the range of 50-75 C

**Result ranking:**
- Results should be ranked by primers and probes of the optimal size, followed by the Tm of the primers and probes - closest to the user specified annealing temperature.

**What to return:**
- Forward primer sequence and Tm
- Reverse primer sequence and Tm
- Probe sequence and Tm
- Tm at which these primers and probes will have homodimers
- Amplicon sequence
