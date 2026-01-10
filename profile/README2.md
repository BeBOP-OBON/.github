# Better Biomolecular Ocean Practices (BeBOP)

## 🌊 Overview

The **Better Biomolecular Ocean Practices (BeBOP)** initiative provides a standardized, machine-readable framework for sharing and archiving scientific protocols. Originally arising from international collaboration within the **Ocean Biomolecular Observing Network (OBON)**, BeBOP aims to make biomolecular and omics methods FAIR (Findable, Accessible, Interoperable, and Reusable) through version control and structured metadata.

## 🛠 Core Components

The initiative bridges the gap between traditional narrative protocols and modern data science needs through three core pillars:

1.  **Markdown-Based Authoring**: Protocols are written in human-readable and machine-readable Markdown, allowing for easy version tracking via Git.
2.  **Structured Metadata**: Every protocol includes a YAML header containing terms from the **Minimum Information about an Omics Protocol (MIOP)** and domain-specific checklists like **FAIR eDNA (FAIRe)**. Values for each term specific for the protocol are added by the user, enabling machine-based tracking of protocol data.
3.  **Permanent Archiving**: Protocols are hosted on **GitHub** and archived on **Zenodo**, which assigns a Digital Object Identifier (DOI) to ensure long-term accessibility and precise citation. High-level versioning is managed via GitHub Releases, which mints version-specific DOIs for each release in addition to the original concept DOI for the repository.

## 🚀 How to Create a BeBOP Protocol

### 1. Repository Setup

Each unique protocol should ideally have its own GitHub repository. This allows for individual DOI assignment, clear versioning, and focused issue tracking.
* **Template:** Fork or use the [0_protocol_collection_template](https://github.com/BeBOP-OBON/0_protocol_collection_template).

### 2. Fill in the YAML Front Matter

The top of your `README.md` must contain structured metadata. This is critical for machine readability and "AI-ready" science. Key fields include:
* `methodology_category`: (e.g., DNA Extraction, Bioinformatic Pipeline)
* `project`: The overarching initiative or lab name.
* `maturity_level`: (e.g., Pilot, Mature, Superseded).
* `external_standard`: References to MIOP or FAIRe terms.

### 3. Document the SOP

Follow the standardized sections provided in the template:

| Section | Purpose |
| :--- | :--- |
| **Protocol Information** | Includes authors, related protocols, a revision record, and a glossary of terms. |
| **Background** | Provides a summary, method description, and spatial/environmental relevance. |
| **Personnel & Safety** | Details the required staff, safety hazards, training, and execution time. |
| **Equipment & Reagents** | A full description of equipment and consumables, including product models and manufacturers. |
| **Procedure** | Step-by-step instructions for preparation, execution, and quality control. |
| **Troubleshooting** | A guide for known issues or common failures and a full list of cited literature with DOIs. |

### 4. Release & Archive

To make your protocol citeable:

1.  Create a **GitHub Release** (e.g., `v1.0.0`).
2.  Connect your repository to **Zenodo**.
3.  Generate a **DOI** to include in your manuscript.

### 5. Use & Maintainenance

* **Version DOI vs. Concept DOI:** Always use the unique version DOI when citing protocols in publications to ensure long-term reproducibility of the exact method used.
* **Protocol Lists:** Organizations are encouraged to maintain a parent repository or README file that links to your different protocol documents. This allows new users to see the collection of protocols in use by your group, and easily navigate across the different repositories.
* **GitHub Topic:** We recommend using the GitHub topic "obon-bebop" to make them findable across GitHub.

## 🔬 Why Use BeBOP?

* **Machine-readability**: The YAML terms and Markdown format facilitate the use of programmatic digestion of protocols usign **R** and **Python** and large-scale data synthesis using **Artificial Intelligence**.
* **Version Control:** Unlike PDFs, BeBOP protocols on GitHub are "living documents". Using the **Version DOI** ensures researchers cite the exact iteration of the method used in their study.
* **Reproducibility:** By tracking protocol details in a machine-readable and version-controlled fashion, BeBOP allows others to precisely reproduce your methods, reducing "methodological drift" across different laboratories.
* **Interoperability:** Metadata fields are designed to "cross-walk" with major data standards like **NCBI (MIxS)** and **GBIF (Darwin Core)**.
Findability: Standardized metadata allows protocols to be easily queried by purpose, target gene, or environmental context.

## 🤝 Community & Support

We encourage the community to provide feedback, suggest metadata improvements, or report issues:

* **Organization:** For general feedback, please submit an issue on the main organization page: [BeBOP-OBON on GitHub](https://github.com/BeBOP-OBON).
* **Repositories:** For technical questions or template suggestions relevant to individual protocol templates, please open an issue in the relevant repository.
