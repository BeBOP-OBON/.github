# Welcome to Better Biomolecular Ocean Practices (BeBOP)

Better Biomolecular Ocean Practices ([BeBOP](https://oceandecade.org/actions/better-biomolecular-ocean-practices/)) is a UN Ocean Decade project under the [Ocean Biomolecular Observing Network (OBON)](https://www.obon-ocean.org/) programme. This project developed out of the [Task Team 21-03: Omics/eDNA Protocol Management](https://www.oceanbestpractices.org/about/task-teams/obps-task-team-21-03-omics-edna-protocol-management/) under the Ocean Best Practices System.

## Aim and Scope
Currently, the wealth of ocean biomolecular practices is shared in diverse formats (e.g. text in publications, pdfs, ...). To better compare differences in practices and integrate data generated using biomolecular protocols, we developed markdown templates as well as standardized metadata describing protocols (called Minimum Information about an Omics Protocol or "MIOP"). Our goal is to create machine-readable protocol documents where changes can be tracked, assigned DOIs, and linked to associated datasets. These tools will also allow us to compare protocols at scale and make protocols more findable.

> [!NOTE]
> Our 2021 paper describes our overall vision and organizational principles:
> 
> Samuel, Robyn M., et al. "Toward a global public repository of community protocols to encourage best practices in biomolecular ocean observing and research." Frontiers in Marine Science 8 (2021): 758694. [https://doi.org/10.3389/fmars.2021.758694](https://doi.org/10.3389/fmars.2021.758694)

## How to get started sharing protocols:

> #### Updates 04/15/25
> We have now updated our BeBOP templates to include relevant metadata from the [FAIRe](https://fair-edna.github.io/index.html) standard.
> 
> We've updated our guidance on how to use our templates with GitHub and now recommend users within their own github lab or personal space:
> - create a seperate repository for each protocol allowing:
>   - DOI creation for each protocol through [Zenodo](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content)
>  - Then create a README file which links to each of their protocol documents (markdown files)
>  - Please also add the github topic "[obon-bebop](https://github.com/topics/obon-bebop)" to make them findable
>
> Great examples from NOAA AOML [here](https://github.com/aomlomics/protocols) and NOAA PMEL [here](https://github.com/NOAA-PMEL/Ocean-Molecular-Ecology)
>
> More details below!

### Overview of steps:

1. Gather your internal SOP/protocol information
2. Navigate to our [template repository](https://github.com/BeBOP-OBON/0_protocol_collection_template) and choose an appropriate protocol template
   - download markdown file (e.g. "protocol_template_DNA_extraction.md")
3. Move major content into appropriate template file
   - many markdown editors are available that easily allow you to visualize your markdown files as you edit them
4. Fine-tune details not included in your internal SOP
   - this includes important metadata fields from both [MIOP](https://github.com/BeBOP-OBON/0_protocol_collection_template/blob/main/MIOP_definition.md) and [FAIRe](https://fair-edna.github.io/index.html) terms
   - handy tip: many details like equipment lists may be very similar to another completed protocols and can be copied and edited
5. Create a GitHub repository for your new BeBOP protocol
   - be specific in your repository name, we recommend something similar to "MyInstitution_Lab/Group_DetailedName_Protocol".
6. Generate a DOI using [Zenodo](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content)

### Step 1: Gather Information

You'll need detailed information about the exact protocol followed, usually found in an internal Standard Operating Procedure (SOP). It is easiest if the person following the protocol first creates this document.

### Step 2: Download appropriate template file

Choose from one of our already created template files which currently cover steps from sampling, DNA extraction, PCR, or sequencing in our [template repository](https://github.com/BeBOP-OBON/0_protocol_collection_template). We are continuing to create more templates for different protocol types and if your protocol is not currently covered, then we would  *highly*  appreciate it if you would like to adapt one of our templates to your new purpose and share it. You can suggest changes or pose issues with templates in our [template repository issue tracker](https://github.com/BeBOP-OBON/0_protocol_collection_template/issues).

- [sampling](https://github.com/BeBOP-OBON/0_protocol_collection_template/blob/main/protocol_template_sampling.md)
- [DNA extraction](https://github.com/BeBOP-OBON/0_protocol_collection_template/blob/main/protocol_template_DNA_extraction.md)
- [PCR](https://github.com/BeBOP-OBON/0_protocol_collection_template/blob/main/protocol_template_PCR.md)
- [sequencing](https://github.com/BeBOP-OBON/0_protocol_collection_template/blob/main/protocol_template_sequencing.md)

### Step 3: Move content into markdown file

Here is where the rubber hits the road. Start copying and pasting text from your SOP into the appropriate parts of the template file. We recommend using a markdown editor that will help you immediately preview what your text formating looks like with markdown formating.

> [!TIP]
> If you are unfamiliar with markdown language, please see this list of resources and softwares to support your work:
> 
> Training resources
> - [Markdown Cheatsheet by Adam Pritchard](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
> - [Markdown Crash Course by Traversy Media](https://youtu.be/HUBNt18RFbo) 
> - [Writing on GitHub by GitHub docs](https://docs.github.com/en/get-started/writing-on-github)
> 
> Markdown Editors (not necessary, but may facilitate editing in markdown)
> - [Visiual Studio Code](https://code.visualstudio.com/Docs/languages/markdown)
> - [MacDown](https://macdown.uranusjr.com), open source Markdown editor for macOS

### Step 4: Enter details missing from internal SOPs

Some needed information will likely be missing from your internal SOP. We decided to include details like equipment lists to enable anyone to easily reproduce your protocol (and see exactly what it requires). We also added metadata from both MIOP and FAIRe standards which describe important details about your protocol. This will both allow us to make protocol documents easier to find, sort, and discover as well as allow tools to be built that can pull important metadata (based on the protocols you used) and allow easier submission of datasets to standard biodiversity repositories like OBIS or GBIF. The metadata section at the beginning of the template enhances the machine-readability of our templates, allowing these tools to be built.

### Step 5: Create GitHub repository

Now that you have your edited markdown file, you can create a new GitHub repository for just that protocol. If you are part of an organization or lab you may want to create all your protocol repositories within that organization. Please be specific in your repository name; we recommend something similar to "MyInstitution_Lab/Group_DetailedName_Protocol".

### Step 6: Generate DOI

Through Zenodo, GitHub has an easy path to create a DOI for any repository. This allows you to have a "release" of your protocol that you can then cite, and will be perpetually available (even if you later edit your protocol document on GitHub). One big advantage is as you may make changes to protocols, you can release new versions with seperate DOIs.

GitHub has good documentation [here](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content) on how to proceed with Zenodo

### Bonus: create README file overview of all your protocols

For the superorganized, we highly recommend creating a README file through GitHub which links to your different protocol documents. This allows new users to see the collection of protocols in use by your group, and easily navigate across the different repositories. We also recommend using the GitHub topic "[obon-bebop](https://github.com/topics/obon-bebop)" to make them findable across GitHub.

There are great examples from NOAA AOML [here](https://github.com/aomlomics/protocols) and NOAA PMEL [here](https://github.com/NOAA-PMEL/Ocean-Molecular-Ecology).

## Contribute!

If you have any feedback or suggestions about our templates please post an issue on the [template repository](https://github.com/BeBOP-OBON/0_protocol_collection_template/issues) or about MIOP fields in our [miop repository](https://github.com/BeBOP-OBON/miop/issues). We also welcome contributions of new types of templates to our collection. Our goal is to cover protocols ranging from study initiation to data sharing, across an entire omics [workflow](https://www.frontiersin.org/files/Articles/758694/fmars-08-758694-HTML-r1/image_m/fmars-08-758694-g001.jpg).
