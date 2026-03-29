# AIAI Dashboard for 3D Visualization of Customer Clusters

## What's AIAI?

Amazing International Airlines Inc. (AIAI) is facing the challenge of designing personalized services and marketing strategies for its diverse customer base.
Customer loyalty membership data and corresponding flight activity collected over a three-year period was analysed and a data-driven segmentation strategy was developed in order
to distinguish valuable customer segments. This repo includes a cluster visualization dashboard obtained through PCA and UMAP dimensionality reductions.

This repository contains the necessary files to host the interactive cluster visualization dashboard on the render.com website. It allows for:
- **rotation and zoom** capabilities
- **real-time filtering** by demographic/behavioral attributes
- **customer detail pop-ups** with segment characteristics.


## Repo Files:

- DM_AIAI_CustomerDB.csv and DM_AIAI_FlightsDB.csv which include customer data over the 3 year period.
- Procfile and requirements.txt for the host platform (render.com)
- app.py which is the python script with the dashboard implementation
- df_customer_treated.csv: this csv file results from the creation of new features which allowed fot the merging of information from both DM_AIAI_CustomerDB.csv and DM_AIAI_FlightsDB.csv;
it is already treated meaning invalid observations were already excluded;
- df_customer_scaler.csv corresponds to the scaled version of the former; *
- umap_coordinates.csv and umap_coordinates.ipynb: both PCA and UMAP dimensionality reduction were conducted but, for running time purposes, the UMAP coordinates had to be obtained in a
different file from app.py


* both datasets were needed for stakeholder sharing purposes: although the clusters were formed using scaled data, the stakeholders still need meaningful real-life values


<img width="459" height="549" alt="Captura de ecrã 2026-03-29, às 16 11 21" src="https://github.com/user-attachments/assets/fb995526-e8b9-41b4-b4c5-0e9f8dd5da6e" />







