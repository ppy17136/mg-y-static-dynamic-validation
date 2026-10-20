# Mg-Y static references and protocol-dependent strain reversal


Data and analysis index for **Static DFT Agreement and Protocol-Dependent Strain-Reversal Response in Mg-Y Interatomic Potentials**.


## Data releases


- Version 4.0.0: [rebuilt-cohort data and analysis code](https://doi.org/10.5281/zenodo.23501142), seventeen modules and a guide in 20 independent ZIPs plus three support files.
- Version 3.0.0: [response and saved-state analysis supplement](https://doi.org/10.5281/zenodo.23438447), nine modules distributed as 62 files, with reassembly and integrity checks.
- Version 2.0.0: [data and output-based analysis code](https://doi.org/10.5281/zenodo.23331296), eight modules, with archive and member checksums.
- Version 1.0.0: [historical reproducibility archive](https://doi.org/10.5281/zenodo.21806152). This remains a separate historical record, not duplicated in version 2.0.0.


Use the version-specific DOI for the data actually analyzed. The releases are complementary: version 4.0.0 does not replace version 3.0.0, the earlier QE/MEAM static-reference modules or the historical archive. Keep the cohorts separate.


## Version 4.0.0 contents

The separate rebuilt cohort contains seventeen data/code modules and an integrated guide: construction and preparation records, sixteen loading recipes and atomic-stress observations, endpoint structural analyses, six selected full first-leg trajectories, and bounded early-frame and material-neighborhood analyses. The sixteen paths use seed 23456 and are not independent seed replicates. The six first-leg trajectories do not provide all raw trajectories of the sixteen complete reversals.

Download all 23 files: Rebuilt_MgY_01_of_20.zip through Rebuilt_MgY_20_of_20.zip, README_TRANSFER.md, TRANSFER_MANIFEST.json and SHA256SUMS.txt. Verify the archive hashes and extract every ZIP into the same new empty directory. These are independent ZIPs, not binary parts: do not concatenate them. The restored layout contains 461 files. From delivery_guide_candidate_v1, run `python -I -B test_verifier.py` and `python -I -B verify_delivery.py --root ..`, then consult README.md and RUN_ORDER.md. Verification and analysis entry points do not launch MD/DFT; loading inputs require separate, deliberate execution. External potential references and exact hashes are provided without the parameter payloads.

Prepared-state acceptance is not proof of thermodynamic equilibrium. The edge_pair label describes construction, not persistent dipole identity. Geometric association and graph breaks do not uniquely establish physical line identity, annihilation or escape. This release does not resolve a direct DFT-to-MD atom mapping or the complete historical/new-baseline difference. Retained candidate labels identify build snapshots, not the published record's status.

## Version 3.0.0 contents


The supplement covers fixed-reference response cohorts, matched preparation/thermostat/rate controls, input provenance, a bounded reversal-velocity intervention, and selected-state structural analyses. The numerical records belong to distinct cohorts and must not be pooled as independent replications.


Download all 62 files from Zenodo and follow TRANSFER_README.md to reassemble the split archives and check their hashes. Then follow README.md and RUN_WORKFLOW.md. The scripts reanalyse retained outputs or postprocess saved states, including PTM/DXA where specified; they do not run fresh MD/DFT simulations. External software dependencies must be obtained separately.


The matched controls and velocity intervention use one seed and do not fully explain the historical/new baseline difference. Two historical final profiles remain unresolved. The Mg-Nd geometry derivative excludes 866 unresolved auxiliary vector records; those fields are not certified. See each module for definitions, exclusions and tolerances.


## Version 2.0.0 contents


The modules cover MD duration/thermostat controls, fast/slow stress comparisons, preparation energy, QE starting-site endpoint energies, finite-cell size checks, pure-CTB low-stress confirmation, vertical MEAM energy reanalysis, and structural-source preservation.


Download the seven complete module ZIPs, five structural-archive parts, reassemble_structures.py, and accompanying README, RUN_WORKFLOW, FILE_INDEX and SHA256SUMS from Zenodo. Run `python -I -B reassemble_structures.py` to reconstruct and verify the original structural ZIP, then extract all eight modules as sibling directories and follow RUN_WORKFLOW.md. Seven numerical reanalysis entry points and one structural-integrity entry point passed local checks. These checks use retained outputs; they do not launch fresh simulations or reproduce upstream PTM/DXA extraction.


## Scientific scope


Static reference agreement and protocol-dependent dynamic response are separate checks, not an experimental ranking of dynamic fidelity. Matched cohorts must not be pooled as independent replications. Finite-cell checks do not establish an infinite-dilution limit or a uniquely resolved equilibrium site. Selected structures do not establish persistent defect identity or DFT-to-MD atom mapping.


Sites 08/10 retain a preoptimized starting route followed by QE relaxation and final SCF. Upstream software is not identified or reproduced in the distribution; original detailed provenance is retained separately. The route is not a native QE-only optimization history. See the module documentation for scope and source-reference versus derivative hashes.


Versions 2.0.0 and 3.0.0 contain no manuscript, paper artwork, complete figure captions, peer-review correspondence, internal working notes, wavefunctions, binary checkpoints or potential payloads.


## Rights


No blanket license overrides existing third-party terms. See THIRD_PARTY_NOTICES.md and file-level notices. The archive grants no rights to external simulation software or potential files.


Corresponding author: Bai Lin Lü, Liaoning Petrochemical University.
