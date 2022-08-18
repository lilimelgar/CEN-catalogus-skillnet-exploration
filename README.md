# CEN-catalogus-exploration

Disclaimer: this repository is public, but the code and the data are still being improved and documented. It is recommended to wait until the final versions are available at the end of 2022.
(note updated on August 18, 2022)

--

This jupyter notebook has been created in the context of the SKILLNET project (skillnet.nl/). The SKILLNET project ("Sharing Knowledge in Learned and Literary Networks") is an European Research Council (ERC)-funded project led by Dirk van Miert (1) at Utrecht University.

One of the most important datasets curated during this project is the Catalogus Epistolarum Neerlandicarum (CEN). This is an aggregated letter dataset of letters' metadata created at different archives and libraries in The Netherlands since the years 1980's which contains more than five hundred thousand records. Since January 2020, one can consult the CEN via Worldcat (https://picarta.on.worldcat.org (last accessed December 29, 2021). 

The CEN dataset was obtained by Ingeborg van Vugt (2) as a data dump in XML format from the Online Computer Library Center (OCLC) and the Royal Dutch Library (KB) in October 2019. The dataset has been sliced (years between 1200 to 1820) and cleaned in two phases: a) manually during Ingeborg's Ph.D. thesis and b) semi-automatically during the SKILLNET project. The second part of the cleaning process has been carried out together by Liliana Melgar Estrada (3) and Ingeborg van Vugt, receiving the input from different collaborators (4). The complete description and the dataset is available in Dataverse (5). 

This repository includes the jupyter notebook that was created for exploring the dataset. This notebook provides access to the CEN catalog slice cleaned during the SKILLNET project (phase b), and offers basic functionalities (using the Python library "Pandas" and other libraries for visualization and network analysis) to query and visualize the data. 

This data overview is offered to researchers as a basic way to see "what's in the data", but for more complex analyses it is recommended to download the latest version of the entire dataset from Dataverse (5) and perform their own analyzes.

---
- (1) Dirk van Miert: SKILLNET project leader. https://orcid.org/0000-0002-5460-4075
- (2) Ingeborg van Vugt: postdoctoral researcher at SKILLNET, data curator of the CEN dataset. https://orcid.org/0000-0002-7703-1791
- (3) Liliana Melgar Estrada: data manager at SKILLNET, data curator of the CEN dataset and author of this jupyter notebook. https://orcid.org/0000-0003-2003-4200
- (4) The SKILLNET project thanks the students and collaborators who gave input to curate this data. They are all listed in the Dataverse page for the dataset.
- (5) All datasets offered by the SKILLNET project are available in this Dataverse: https://dataverse.nl/dataverse/skillnet