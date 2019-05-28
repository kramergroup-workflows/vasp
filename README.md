# VASP Workflows

This repository collects workflows for VASP.

## Workflows

| File                         | Description                                          |
| ---------------------------- | ---------------------------------------------------- |
| `total-energy-from-iscd.yml` | Compute total energy of structure from ICSD database |

### Total energy calculations

#### Total energy from ISCD

File: `total-energy-from-iscd.yml`

Computes the fully relaxed total energy of a structure using materialsproject.org defaults.
The following inputs are valid:

| Name         | Description                                                                     |
| ------------ | ------------------------------------------------------------------------------- |
| `icsdid`     | The ICSD cif file id code (unfortunately, this is rather difficult to obtain)   |
| `functional` | Defined the functional to use (**currently ignored; defaults to PBE or PBE+U**) |

> The CIF file code is unfortnuately not the same as the collection code of the ICSD database. The easiest
> way to obtian the CIF code is to download the cif file and check the download URL (can be done in Firefox)
