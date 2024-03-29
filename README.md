
# NEODATASET
### The NEODATASET is a dataset containing projects extracted from gitlab that work with SCRUM
### Autor: Giseldo da Silva Neo

# Introduction

We have made a new dataset (aka NEODATASET) available together with UST. This dataset encompasses data from 34 software development projects, with 40.014 User Stories taken from GitLab repositories, totaling 163.897 Story Points. It is made available on GitHub 6 so that the entire interested community can contribute, similarly to what happens with other datasets.

This dataset was mined during January 2023 and April 2023. The mining process targeted GitLab’s top open-source projects. The selected projects employ agile software development methodologies and had the size of their tasks recorded in Story Points. To mine information from GitLab, we created an ex traction tool implemented in Python that connects to GitLab via API Only Tasks with the State attribute equal to Closed and that have the weight attribute filled in were col- lected. The weight field is used in GitLab to record the effort in Story Points. More information about the projects included in the dataset is also available directly from GitLab. 

The projects in the dataset have different characteristics and cover different programming languages, different business domains, and different geographic locations of the team. The main entity of the dataset is the User Story (or Issue), which contains the main information. The dataset has more than 70 attributes and is stored in JSON and CSV format, given the simplicity of dealing with both formats. 

The dataset presented here includes projects which were not used by previous studies. There are already previous studies that extracted data from the Jira management tool to build predictive models (Tawosi et al., 2022a; Choetkiertikul et al., 2019; Porru et al., 2016; Scott and Pfahl, 2018), but projects extracted from GitLab are rarer. Just as (Tawosi et al., 2022a) did, we are sharing all the data collected. Therefore, the most common thing is to share only the data from the dataset considered in the study itself, as done, for example in (Choetkiertikul et al., 2019), and not all the data collected.

The expected contribution is that this data set can assist education and research on agile software development. Although our dataset was initially designed for Story Points and User Story estimation training and research, it also includes information relevant to other software engineering aspects. In addition to providing a possibility to reproduce findings from other studies.

# Descrição das colunas

- "weight" é a coluna que guarda o SP estimado pelo time
- "description" é a coluna que guarda a descrição da issue

## Todas as colunas do dataset
 
   ```mermaid
   classDiagram
       class Colunas{
        -Title
        -Description
        -Issue ID
        -URL
        -State
        -Author
        -Author Username
        -Assignee
        -Assignee Username
        -Confidential
        -Locked
        -Due Date
        -CrDated At
        -Updated At
        -Closed At
        -Milestone
        -Weight
        -Labels
        -Time Estimate
        -Time Spent
        -Epic ID
        -Epic Title
        }
   ```
 



   

