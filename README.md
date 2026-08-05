# Mg-Y static-dynamic validation under strain reversal

Reproducibility index for the manuscript:

> **Static DFT Agreement and Direction-Dependent Strain-Reversal Response Favor Different Mg-Y Interatomic Potentials: Identical-Start Tests**

## Scope

The study compares two public Mg-Y MEAM parameterizations using controlled identical-start tests. Static finite-cell Quantum ESPRESSO site-energy checks and direction-dependent strain-reversal response favor different parameterizations. This repository is an index for the documented workflow; the immutable full archive is deposited on Zenodo.

## Reproducibility archive

- Zenodo DOI: [10.5281/zenodo.21806152](https://doi.org/10.5281/zenodo.21806152)
- Version: `1.0.0`
- Archive file: `Reproducibility_Package.zip`
- Integrity: byte-counted SHA-256 manifest included in the archive

The Zenodo record was published on August 5, 2026, and the DOI is active.

## Contents

The Zenodo archive contains processed paired metrics, grouped statistics, sensitivity analyses, figure-value tables, representative LAMMPS inputs and outputs, Quantum ESPRESSO inputs and final outputs, pseudopotential checksums, convergence records, and analysis and figure-generation scripts. Large regenerable Quantum ESPRESSO scratch files and nonessential raw molecular-dynamics trajectories are excluded as documented in the archive.

## Verification

After extracting the archive, follow `RUN_WORKFLOW.md`. The fast verification commands are:

```bash
python verify_package.py
python reproduce_core_results.py
python reproduce_transfer_audit.py
```

## Rights and provenance

No blanket license is applied to the mixed archive. Author-created materials and third-party interatomic-potential or pseudopotential files have distinct rights and provenance. Third-party files remain subject to their original terms; see the provenance manifests and included license files in the Zenodo archive.

## Contact

Corresponding author: Bai Lin Lü, Liaoning Petrochemical University.
