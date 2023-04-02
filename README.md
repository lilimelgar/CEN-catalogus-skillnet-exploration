[![Binder: launch this notebook on the web](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lilimelgar/CEN-catalogus-exploration/HEAD?labpath=%2Fsrc%2FCEN_SKILLNETslice_overview.ipynb)

[![DOI for this Github repository](https://zenodo.org/badge/DOI/10.5281/zenodo.7309978.svg)](https://doi.org/10.5281/zenodo.7309978)

[![DOI for the dataset](<https://img.shields.io/badge/Dataverse DOI-10.34894/G8XQI0-orange>)](https://dataverse.nl/dataset.xhtml?persistentId=doi:10.34894/G8XQI0)


# Exploring the Catalogus Epistolarum Neerlandicarum (CEN): curated slice by SKILLNET (1200-1820)

Note: The SKILLNET project finished at the end of 2022. The CEN dataset described below and the jupyter notebook developed to explore the dataset are not being longer cleaned or developed. If you find any issues or have any questions, please email the repository owner.

--

# Introduction

This jupyter notebook was created in the context of the SKILLNET project (skillnet.nl/). 

The SKILLNET project (https://skillnet.nl/) is a European Research Council (ERC)-funded project led by Dirk van Miert (https://orcid.org/0000-0002-5460-4075) at Utrecht University. This project investigates the ideals of sharing knowledge as a legacy of a bottom-up social network of scholars and scientists from the Early Modern period.

One of the most important datasets curated during this project is the Catalogus Epistolarum Neerlandicarum (CEN). The CEN is the Dutch national letter catalog, which aggregates letter metadata from different universities in the Netherlands and from the National Library of the Netherlands (KB), among others, since the years 1980's to the present. The curated version of a slice of the entire data (approx. 10% of the entire CEN) is offered in this dataset. It includes the letters between 1270 and 1820 plus some undated letters, which is of interest for the study of Early Modern correspondence.

The complete description and the dataset is available in Dataverse (https://dataverse.nl/dataverse/skillnet). The specific dataset that is used by this notebook can be cited with this DOI (add always version number to the citation): https://doi.org/10.34894/G8XQI0.

# Introduction to the jupyter notebook

This repository includes the jupyter notebook that was created for exploring the CEN curated dataset by SKILLNET. 

Jupyter notebooks (https://jupyter.org/) are web environments where code can be written and executed, and it is not only code, but it also allows the integration of narrative text.

This notebook provides access to the latest version of the CEN catalog slice (a exact copy is deposited in Dataverse, link above), and offers basic functionalities to query and visualize the data. As a researcher interested in the letters metadata of this period you can use this notebook for:

- Getting an overview of how many letters are in the dataset, in total and per year
- Getting an overview of the correspondents (persons) in the dataset, and the amount of letters they exchanged
- Generating a first-degree network for a person of interest
- Generating a second-degree network for a person of interest
- Downloading the "nodes" and "edges" files necessary for network analysis in other tools (e.g., Gephi (https://gephi.org/))
- Understanding the challenges and solutions we used to clean the original dataset

The data overview facilitated by the notebook is offered to researchers as a basic way to see "what's in the data", but for more complex analyses it is recommended to download the latest version of the entire dataset from Dataverse and perform their own analyzes.

This jupyter notebook is part of a Github repository which is deposited in Zenodo and can be cited with this DOI: https://doi.org/10.5281/zenodo.7309977 (using the specific version number DOI). The original repository is here: https://github.com/lilimelgar/CEN-catalogus-skillnet-exploration.


# How to use this notebook

**If you are newbie to jupyter notebooks or simply want to use this notebook to explore the data, just click here: https://edu.nl/bn93d**.

Jupyter notebooks can also be ran in your own computer by installing them (for example, using the Anaconda distribution (https://www.anaconda.com/products/distribution) and then cloning the github repository. If you prefer that method:
- install Anaconda on your system
- clone the git repository to your machine, or simply download and extract the zip file-
- create a new Anaconda environment that contains everything necessary to run the notebook (see the 'requirements.txt' file) 

However, to facilitate its use by people who are not interested in installing the programs, or to avoid conflicting versioning of these programs, we have used "My binder" (https://mybinder.readthedocs.io/en/latest/#) to pack the repository, which is ready to be used online in the link provided above (https://edu.nl/bn93d) (1).

More specific instructions about how to use the notebook are provided within the notebook itself.

# Data

An exact copy of the data (letters and persons files of the CEN cleaned slice by Skillnet) is also deposited in Dataverse, where there is more complete documentation about the cleaning process.

# Contributing

You can also add comments to this notebook (for example: suggestions to add new functions, questions, requests for more explanation, etc.). For doing this, we recommend to create an "issue" in Github: https://github.com/lilimelgar/CEN-catalogus-exploration/issues.

# Versioning and citing

The CEN curated dataset has different versions, it is recommended to always use the latest one deposited from the Dataverse repository: https://doi.org/10.34894/G8XQI0.

The jupyter notebook also has versions. Likewise, it is recommended to always use the latest one deposited in Zenodo: https://doi.org/10.5281/zenodo.7309977 (this DOI provides access to all the versions, if you need to cite a specific version, including the latest one, copy the DOI of the version provided in Zenodo)

# Credits and acknowledgements

- The right holders of the original CEN database and its content are OCLC and the National Library of The Netherlands (KB), who granted access to a data dump of the CEN dataset in 2019 to Ingeborg van Vugt.
- The dataset has been obtained and cleaned to an important extent by Ingeborg van Vugt.
- Datamanager Liliana Melgar-Estrada has contributed with semi-automatic methods, and also manual curation, to the cleaning of the dataset since 2020.
- Rosalie Versmissen, student assistant, has also contributed to the curation of the dataset since August 2022.
- Project leader Dirk van Miert has provided the means to perform this work, and has also been curator and researcher of this dataset.
- This project has received funding from the European Research Council (ERC) under the European Union's Horizon 2020 research and innovation programme (grant agreement n° ERC-2016-COG).
- The SKILLNET project thanks other project members (Koen Scholten, Robin Buning, intern students) and external collaborators for their contributions.



---
- (1) The URL above is shortened for dissemination purposes. This is the long original URL provided by my Binder: https://mybinder.org/v2/gh/lilimelgar/CEN-catalogus-exploration/HEAD?labpath=%2Fsrc%2FCEN_SKILLNETslice_overview.ipynb