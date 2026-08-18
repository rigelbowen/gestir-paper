[![DOI](https://zenodo.org/badge/1338772660.svg)](https://doi.org/10.5281/zenodo.22002250)

# Gestir: Reading and Writing Maya's Binary Scene Format Without Maya

A white paper on gestir, my dependency-free C++ reader and writer for Maya's
binary `.mb` scene format. No Maya SDK, no Autodesk libraries, no license seat,
no running DCC. Everything in it was derived by differential analysis of files
Maya wrote, with Maya itself as the final say on whether a written file is valid.

- **[Read the paper (PDF)](gestir_whitepaper.pdf)**
- [Markdown source](gestir_whitepaper.md) (canonical; the PDF renders from it)

Covers: the `.mb` container as observed (64-bit IFF, big-endian, 4-byte aligned,
and the alignment mistake that costs the most time), the reverse-engineering
method, a catalog of real failures and what each one taught, and the writer
architecture ("verbatim unless dirty") that makes it safe to modify a file
whose format you only partly understand.

Version 1.0, August 2026. Contact: fact@rigelisawesome.com
