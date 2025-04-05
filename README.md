# NEODATASET

NEODATASET is a dataset containing projects with title and description in natural language of User Stories and their Story Points extracted from GitLab.

## Description

This dataset encompasses data from 34 software development projects, with 40.014 User Stories taken from GitLab repositories, totaling 163.897 Story Points. It is made available on GitHub, huggging face and mendeley data, so that the entire interested community can contribute, similarly to what happens with other datasets.

This dataset was mined during January 2023 and April 2023. The mining process targeted GitLab’s top open-source projects. The selected projects employ agile software development methodologies and had the size of their tasks recorded in Story Points. To mine information from GitLab, we created an extraction tool implemented in Python that connects to GitLab via API. Only Tasks with the State attribute equal to Closed and that have the weight attribute filled in were collected. The weight field is used in GitLab to record the effort in Story Points. More information about the projects included in the dataset is also available directly from GitLab. 

The projects in the dataset have different characteristics and cover different programming languages, different business domains, and different geographic locations of the team. The main entity of the dataset is the User Story (or Issue), which contains the main information. The CSV format is easier to use and contains only the attributes: issue key, created, title, description, and story points, making it more user-friendly. 

The expected contribution is that this data set can assist education and research on agile software development. Although our dataset was initially designed for Story Points and User Story estimation training and research, it also includes information relevant to other software engineering aspects. In addition to providing a possibility to reproduce findings from other studies.

## Dataset columns

```mermaid
classDiagram
   class Issue {
     - issuekey
     - created
     - title 
     - description 
     - storypoints
    }
```

- issuekey: User Story ID
- created: Date of the created of the User Story
- title: Title of User Story
- description: Description of User Story
- storypoints: Count of the user story informed by the team

## Info
You can also access this dataset in [HuggingFace](https://huggingface.co/datasets/giseldo/neodataset) or in [Mendeley Data](https://data.mendeley.com/datasets/skk2wn9j86/1).

This dataset is used in [User Story Tutor Software](https://github.com/giseldo/userstory) and was presented in [this article](https://www.scitepress.org/PublicationsDetail.aspx?ID=PpuYOsDviJ4=&t=1), a version of the [article is also available at arxiv](https://arxiv.org/abs/2406.16259).

Another use of this NEODATASET is [this another article at arxiv](https://arxiv.org/abs/2503.13279) from another researchers.

## How to cite

Neo, G. S., Moura, J., Almeida, H., Neo, A. and Freitas Júnior, O. (2024). User Story Tutor (UST) to Support Agile Software Developers. In Proceedings of the 16th International Conference on Computer Supported Education - Volume 2: CSEDU; ISBN 978-989-758-697-2; ISSN 2184-5026, SciTePress, pages 51-62. DOI: 10.5220/0012619200003693

`
@conference{csedu24,
author={Giseldo S. {Neo} and José Moura and Hyggo Almeida and Alana Neo and Olival {Freitas Júnior}},
title={User Story Tutor (UST) to Support Agile Software Developers},
booktitle={Proceedings of the 16th International Conference on Computer Supported Education - Volume 2: CSEDU},
year={2024},
pages={51-62},
publisher={SciTePress},
organization={INSTICC},
doi={10.5220/0012619200003693},
isbn={978-989-758-697-2},
issn={2184-5026},
}

## Contact Autor

Giseldo da Silva Neo at giseldo@gmail.com. More about-me in [ResearchGate](https://www.researchgate.net/profile/Giseldo-Neo) or in my [personal site](http://giseldo.github.io).
