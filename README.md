test to see if it updates correctly in Zenodo

# CEN-catalogus-exploration

Disclaimer: We are still actively developing this notebook by improving existing functions and adding new ones. Also the CEN data is constantly being cleaned. This development will go until the end of the SKILLNET project (December 2022). If you use this notebook or the data before that date, please be aware that there may be issues or lack of documentation. It is recommended to use the cleaned data and code from December 2022.
Please submit any issue to this Github repository or email the repository owner.
(note updated on August 18, 2022)

--

# Introduction
This jupyter notebook has been created in the context of the SKILLNET project (skillnet.nl/). The SKILLNET project ("Sharing Knowledge in Learned and Literary Networks") is an European Research Council (ERC)-funded project led by Dirk van Miert (1) at Utrecht University.

One of the most important datasets curated during this project is the Catalogus Epistolarum Neerlandicarum (CEN). This is an aggregated letter dataset of letters' metadata created at different archives and libraries in The Netherlands since the years 1980's which contains more than five hundred thousand records. Since January 2020, one can consult the CEN via Worldcat (https://picarta.on.worldcat.org (last accessed December 29, 2021). 

The CEN dataset was obtained by Ingeborg van Vugt (2) as a data dump in XML format from the Online Computer Library Center (OCLC) and the Royal Dutch Library (KB) in October 2019. The dataset has been sliced (years between 1200 to 1820) and cleaned in two phases: a) manually during Ingeborg's Ph.D. thesis and b) semi-automatically during the SKILLNET project. The second part of the cleaning process has been carried out together by Liliana Melgar Estrada (3) and Ingeborg van Vugt, receiving the input from different collaborators (4). The complete description and the dataset is available in Dataverse (5). 

This repository includes the jupyter notebook that was created for exploring the dataset. This notebook provides access to the CEN catalog slice cleaned during the SKILLNET project (phase b), and offers basic functionalities (using the Python library "Pandas" and other libraries for visualization and network analysis) to query and visualize the data. 

This data overview is offered to researchers as a basic way to see "what's in the data", but for more complex analyses it is recommended to download the latest version of the entire dataset from Dataverse (5) and perform their own analyzes.

# How to use this notebook
(disclaimer: this content was written for an introductory workshop using Google Colab, will be updated soon).

This is a jupyter notebook (6). Jupyter notebooks are web environments where code can be written and executed, and it is not only code, but it also allows the integration of narrative text. Jupyter notebooks can be ran in your own computer by installing them. 
<!-- In this case, we offer the notebook in a cloud service provided by Google, so you don't need to install anything. The service is called "Collab" (7).
 -->
The notebook has cells with python code that can be executed, and other cells with explanatory text written in Markdown (which is a basic text editing language) (8). Below a cell with code there is often a cell with output.

This notebook is meant to work without having to write any code yourself in order to get those outputs. If you click in the main menu above the option "Cell -> Run all", the notebook will produce results and visualizations, which are explained in the explanatory text cells. However, there is also the option to do simple manipulations: for example, instead of getting the first 20 correspondents, you can decide you want to see 50. In that case, you need to change that value in the cell. When this is the case, the cell has a header above named "Your input here".

You can also add comments to this notebook (for example: suggestions to add new functions, questions, requests for more explanation, etc.). For doing this, we recommend to create an "issue" in Github: https://github.com/lilimelgar/CEN-catalogus-exploration/issues. 
<!-- For doing this, you can use the "add comment" functionality in the cell pannel. Another option is to click on "Insert" in the main menu above, and insert a new cell. Change it's type to "Markdown" in the menu below the main menu. Then you can write in simple text all your comments. -->

If you want to read the notebook step by step, you can then:

One option is that you run one cell at the time. However, Section 2 and 3 are mostly preparatory (you don't get any interesting output from them), thus, you can skip those, but you will have to execute them. For that purpose put your cursor in Section 4: CEN Letters overview. Click on the menu "Cell -> Run all above". This is to execute all the cells that download and prepare the data. Then you can go cell by cell reading the explanations and executing the code to get the outputs. When you see a header "Give input here" you can then change the values according to your wishes.
Some cells are meant to facilitate exporting the data. Those cells are "commented". This means that they are not executed unless you decide so. Otherwise, every time that you run the notebook you will get many files downloaded to your computer without you having decided that. The symbol to distinguish a comment is the dash: #. If a cell is commented, all the code inside it has a dash or two dashes. In order to uncomment it, you can select all the content of the cell and press "CTRL" + /.

---
- (1) Dirk van Miert: SKILLNET project leader. https://orcid.org/0000-0002-5460-4075
- (2) Ingeborg van Vugt: postdoctoral researcher at SKILLNET, data curator of the CEN dataset. https://orcid.org/0000-0002-7703-1791
- (3) Liliana Melgar Estrada: data manager at SKILLNET, data curator of the CEN dataset and author of this jupyter notebook. https://orcid.org/0000-0003-2003-4200
- (4) The SKILLNET project thanks the students and collaborators who gave input to curate this data. They are all listed in the Dataverse page for the dataset.
- (5) All datasets offered by the SKILLNET project are available in this Dataverse: https://dataverse.nl/dataverse/skillnet
- (6) https://jupyter.org/
- (7) https://colab.research.google.com/notebooks/basic_features_overview.ipynb
- (8) https://en.wikipedia.org/wiki/Markdown