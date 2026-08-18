# Gestir: Reading and Writing Maya's Binary Scene Format Without Maya

This is the paper. [PDF](gestir_whitepaper.pdf), or [markdown](gestir_whitepaper.md) if you prefer. The markdown is the canonical copy, the PDF renders from it.

Gestir is a C++ reader and writer for Maya's `.mb` files that doesn't use the Maya SDK and doesn't need Maya installed. Autodesk doesn't publish the format, so I worked it out by diffing controlled saves and letting Maya judge whether my written files were valid. The paper is the container layout as I observed it, how I derived it, the mistakes that cost me the most time, and the writer design that makes it reasonably safe to edit a file whose format you only partly understand.

Corrections get appended to the paper's errata section with dates rather than silently edited in.

v1.0, August 2026. fact@rigelisawesome.com
