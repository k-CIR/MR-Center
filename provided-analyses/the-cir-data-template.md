# The CIR data template

The **main directory** of the **CIR data template** contains all **important directories** and **singularity containers** for running the programs necessary for transfer, conversion to BIDS and preprocessing of data.

<figure><img src="../.gitbook/assets/Screenshot 2024-09-10 at 15.19.10.png" alt=""><figcaption></figcaption></figure>

### Scripts&#x20;

* **`run_dicomtransfer.sh`**: handles file transfers. The script assumes data has been organized according to the MRC standard.
* **`create_heuristic_heudiconv.sh`**: extracts the metadata from DICOM files located in the `/dicom` directory. It generates a `.tsv` file for each DICOM file, storing the results in the `/dicom` directory.
* **`run_heudiconv.sh`**: creates a basic BIDS structure from DICOM files and stores the output in the `/bids` folder.
* **`run_fmriprep.sh`**: BIDS-formatted data located in the **`/bids`** folder using _fmriprep_. The preprocessed output is stored in the **`/bids/derivatives/fmriprep`** directory.
