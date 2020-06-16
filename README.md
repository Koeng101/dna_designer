# dna_designer [DEPRECIATED]

This is the DNA designer package, made by Keoni Gandall originally to help design DNA for the FreeGenes project. Note: this project is being depreciated, and work is being moved to [Poly](https://github.com/TimothyStiles/poly).

## Usage

To install:
```bash
pip install dna_designer
```

To optimize genes and remove restriction enzyme sites:
```python
from dna_designer import moclo
gene = 'MHELLQWQRLD'
new_gene = optimize_fix(gene)
```

## How it works

Your gene is stochastically optimized against a given codon table. After optimization, it is reviewed for repeats, homopolyers, and GC ranges which may affect DNA synthesis and those are then fixed by stochastically switching codons in the affected region. By default, it uses the [FreqB](https://doi.org/10.1371/journal.pone.0007002) codon table.

## Supporters
Thank you to Anton Jackson-Smith for writing the original gene optimization software, from which this was forked and built out of.
