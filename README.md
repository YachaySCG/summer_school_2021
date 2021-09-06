# SC Summer School 2021 Materials

## Tutorial Notebooks

| Title             | Date                       | Link |
|-------------------|----------------------------|------|
| Transfer Learning | Day 1 - September 20, 2021 | <a href="https://colab.research.google.com/github/YachaySCG/summer_school_2021/blob/master/template_pytorch_sc_2021.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>     |
|                   | Day 2 - September 21, 2021 |  <a href="https://colab.research.google.com/github/YachaySCG/summer_school_2021/blob/master/template_pytorch_sc_2021.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>    |
|                   | Day 3 - September 22, 2021 |  <a href="https://colab.research.google.com/github/YachaySCG/summer_school_2021/blob/master/template_pytorch_sc_2021.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>    |
|                   | Day 4 - September 23, 2021 | <a href="https://colab.research.google.com/github/YachaySCG/summer_school_2021/blob/master/template_pytorch_sc_2021.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>     |
|                   | Day 5 - September 24, 2021 |  <a href="https://colab.research.google.com/github/YachaySCG/summer_school_2021/blob/master/template_pytorch_sc_2021.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>    |

## Challenge Resources

| Source              | Link |
|---------------------|------|
| Pytorch Template    | <a href="https://colab.research.google.com/github/YachaySCG/summer_school_2021/blob/master/template_pytorch_sc_2021.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>     |
| Tensorflow Template | <a href="https://colab.research.google.com/github/YachaySCG/summer_school_2021/blob/master/template_tensorflow_sc_2021.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>     |
| Modified Dataset    | <a href="https://drive.google.com/file/d/1pFWcrh9Qdn8irqognubPTjfaY1uDecFM/view?usp=sharing" target="_parent"><img src="https://cdn.icon-icons.com/icons2/2642/PNG/512/google_drive_logo_icon_159334.png" width="32" height="32" alt="Download Dataset"/></a>     |

## Challenge Guideline

In this competition, you are challenged to build a deep learning model that identifies different types of natural scenes in a dataset of images, where the images have been noisy (between 15-25% of the image was randomly covered by a black rectangle).

The dataset counts with 6 natural scene categories: `buildings`, `forest`, `glacier`, `mountain` , `sea` , `street`.

The dataset was dividided in train: 9300 images, val: 3000 images, test: 4734

### Rules

- This is an individual competition, only for SC 2021 participants.
- You will work with the dataset available at:

    [dataset_sc_2021.zip](https://drive.google.com/file/d/1pFWcrh9Qdn8irqognubPTjfaY1uDecFM/view?usp=sharing)

- Your task is to propose a model to obtain best classification results using the provided `test` subset (a part of the data_scg_2021.zip).
- The participants of this challenge will be required to send the code of the created solution (in a ZIP file) for further check.
- The results will be evaluated by the organizers and three best entries will be awarded.
- The winners of the competition will be asked to send a short video (1-5 minutes) or PDF slides with a presentation of their solution. The film or slides will be placed on the SCG 2021 website, therefore matters relating to the privacy of submitters must be properly considered when preparing the video).

### Evaluation

Submissions will be evaluated on a weighted F1 score using a scikit-learn function. The submission website will be announced on Slack.

[F1 score function](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html)

parameters: 

- average='weighted'
- other parameters - default.

For each id in the `test` set, you must predict a type of natural scene (or label). The file should contain a header and have the following format:

```bash
id,label
22010,B
22006,F
22013,G
24025,M
8046,S
803,ST
```

where 

- B indicates `buildings`
- F indicates `forest`
- G indicates `glacier`
- M indicates `mountain`
- S indicates `sea`
- ST indicate `street`

The submission file should be named: 

`sample_submission_first_n.csv`

, where 'first' is the participant's first name and 'n' is the first letter of the participant's last name.

### Schedule 

| Activity                         | Date               |
|----------------------------------|--------------------|
| Start of the competition         | September 10, 2021 |
| Proposal Presentation            | September 24, 2021 |
| End of time for sending results  | October 1, 2021    |
| Announcement of results-> Awards | October 4, 2021    |


### Information about data set

The dataset used in this challenge is the "Intel Image Classification" dataset provided by Puneet Bansal.

Source: [https://www.kaggle.com/techsash/waste-classification-data](https://www.kaggle.com/puneet6060/intel-image-classification)

Licence: CC BY-SA 4.0

The dataset has been processed for the needs of this challenge