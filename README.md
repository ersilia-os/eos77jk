# Chemical Checker Signaturizer 3D D1-5

Building on the Chemical Checker bioactivity signatures (available as eos4u6p), the authors use the relation between stereoisomers and bioactivity of over 1M compounds to train stereochemically-aware signaturizers that better describe small molecule bioactivity properties. This model corresponds to the Chemical Checker spaces D1, D2, D3, D4 and D5.

This model was incorporated on 2025-06-25.

## Information
### Identifiers
- **Ersilia Identifier:** `eos77jk`
- **Slug:** `cc-signaturizer-3d-d`

### Domain
- **Task:** `Representation`
- **Subtask:** `Featurization`
- **Biomedical Area:** `Any`
- **Target Organism:** `Not Applicable`
- **Tags:** `Descriptor`, `Bioactivity profile`, `Embedding`

### Input
- **Input:** `Compound`
- **Input Dimension:** `1`

### Output
- **Output Dimension:** `640`
- **Output Consistency:** `Fixed`
- **Interpretation:** Vector representation of a molecule

Below are the **Output Columns** of the model:
| Name | Type | Direction | Description |
|------|------|-----------|-------------|
| d1_000 | float |  | Dimension 0 for Signaturizer3D dataset cells (D) gene expression (D1) |
| d1_001 | float |  | Dimension 1 for Signaturizer3D dataset cells (D) gene expression (D1) |
| d1_002 | float |  | Dimension 2 for Signaturizer3D dataset cells (D) gene expression (D1) |
| d1_003 | float |  | Dimension 3 for Signaturizer3D dataset cells (D) gene expression (D1) |
| d1_004 | float |  | Dimension 4 for Signaturizer3D dataset cells (D) gene expression (D1) |
| d1_005 | float |  | Dimension 5 for Signaturizer3D dataset cells (D) gene expression (D1) |
| d1_006 | float |  | Dimension 6 for Signaturizer3D dataset cells (D) gene expression (D1) |
| d1_007 | float |  | Dimension 7 for Signaturizer3D dataset cells (D) gene expression (D1) |
| d1_008 | float |  | Dimension 8 for Signaturizer3D dataset cells (D) gene expression (D1) |
| d1_009 | float |  | Dimension 9 for Signaturizer3D dataset cells (D) gene expression (D1) |

_10 of 640 columns are shown_
### Source and Deployment
- **Source:** `Local`
- **Source Type:** `External`
- **DockerHub**: [https://hub.docker.com/r/ersiliaos/eos77jk](https://hub.docker.com/r/ersiliaos/eos77jk)
- **Docker Architecture:** `AMD64`, `ARM64`
- **S3 Storage**: [https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos77jk.zip](https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos77jk.zip)

### Resource Consumption
- **Model Size (Mb):** `5456`
- **Environment Size (Mb):** `1309`
- **Image Size (Mb):** `9375.15`

**Computational Performance (seconds):**
- 10 inputs: `39.1`
- 100 inputs: `99.89`
- 10000 inputs: `-1`

### References
- **Source Code**: [https://gitlabsbnb.irbbarcelona.org/packages/signaturizer3d](https://gitlabsbnb.irbbarcelona.org/packages/signaturizer3d)
- **Publication**: [https://jcheminf.biomedcentral.com/articles/10.1186/s13321-024-00867-4](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-024-00867-4)
- **Publication Type:** `Peer reviewed`
- **Publication Year:** `2024`
- **Ersilia Contributor:** [arnaucoma24](https://github.com/arnaucoma24)

### License
This package is licensed under a [GPL-3.0](https://github.com/ersilia-os/ersilia/blob/master/LICENSE) license. The model contained within this package is licensed under a [GPL-3.0-or-later](LICENSE) license.

**Notice**: Ersilia grants access to models _as is_, directly from the original authors, please refer to the original code repository and/or publication if you use the model in your research.


## Use
To use this model locally, you need to have the [Ersilia CLI](https://github.com/ersilia-os/ersilia) installed.
The model can be **fetched** using the following command:
```bash
# fetch model from the Ersilia Model Hub
ersilia fetch eos77jk
```
Then, you can **serve**, **run** and **close** the model as follows:
```bash
# serve the model
ersilia serve eos77jk
# generate an example file
ersilia example -n 3 -f my_input.csv
# run the model
ersilia run -i my_input.csv -o my_output.csv
# close the model
ersilia close
```

## About Ersilia
The [Ersilia Open Source Initiative](https://ersilia.io) is a tech non-profit organization fueling sustainable research in the Global South.
Please [cite](https://github.com/ersilia-os/ersilia/blob/master/CITATION.cff) the Ersilia Model Hub if you've found this model to be useful. Always [let us know](https://github.com/ersilia-os/ersilia/issues) if you experience any issues while trying to run it.
If you want to contribute to our mission, consider [donating](https://www.ersilia.io/donate) to Ersilia!
