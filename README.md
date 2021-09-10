# Detecting Illegal Fishing

### Project Description
By ingesting [fishing vessel tracking data](https://globalfishingwatch.org/data-download/datasets/public-training-data-v1), I will train a neural network to classify vessels and detect a variety of fishing events. The network will be fed [AIS](https://spire.com/wiki/ais-tracking-data-your-ultimate-guide/) (Automatic Identification System) data, which is a required tracking system that uses GPS sensors on ships, and potentially VMS (Vessel Monitoring System) data as well. 

<figure>
 
 <figcaption align="center">Fig 1. AIS data from a troller ship</figcaption>
 <img width="795" alt="Screen Shot 2021-09-09 at 10 08 56 PM" src="https://user-images.githubusercontent.com/58823003/132802815-50380b9b-2feb-476a-940a-ed98fe6fb18c.png">
</figure>

[Source](https://globalfishingwatch.org/data-download/datasets/public-training-data-v1)

<figure>
 
 <figcaption align="center">Fig 2. Mapped data points for long liner and reefer fishing activities</figcaption>
<img width="540" alt="Screen Shot 2021-09-09 at 10 14 30 PM" src="https://user-images.githubusercontent.com/58823003/132803200-79b13c7f-e8fc-4f8e-9dca-6bfb59308848.png">
 
</figure>

[Source](https://link-springer-com.ccl.idm.oclc.org/article/10.1007/s11277-020-07200-w)
 
Combining this identification method with other datasets from [Global Fishing Watch](https://globalfishingwatch.org/data-download/), the vessel's activities can be categorized as either legal or illegal, depending on parameters such as country of origin and local maritime laws.

Since overfishing and destructive fishing methods impart a tremendous burden on Earth's oceanic ecosystem, the identification of fishing patterns is key to catching and halting illegal fishing methods as soon as possible. 


### Project Goals
1. Use Global Fishing Watch's dataset to train a model that can identify different types of fishing behavior.
2. Apply the model to Global Fishing Watch's testing dataset to categorize fishing behaviors.
3. (Longer Term) Can we predict the fishing behaviors with less data? That is, in real time?

### Unknowns
- How do 'dark spots' (periods in which the ship is not transmitting/receiving AIS data, either on purpose or due to techincal difficulty) impact the classification?
- This dataset contains already identified segments of trips. Can we take a much larger set of a ship's data and identify which aspects of it were attributed to the actual fishing method, rather than simply traveling or halting in the ocean?

### Inspiration
- [Catching industrial fishing incursions into inshore waters of Africa from space](https://onlinelibrary-wiley-com.ccl.idm.oclc.org/doi/full/10.1111/faf.12436)
- [Fishing Vessels Behavior Identification for Combating IUU Fishing: Enable Traceability at Sea](https://link-springer-com.ccl.idm.oclc.org/article/10.1007/s11277-020-07200-w)
- [An Automatic Identification System (AIS) Database for
Maritime Trajectory Prediction and Data Mining](https://arxiv.org/pdf/1607.03306.pdf)
- [A Deep Learning Approach for Fishing Vessel Classification from VMS Trajectories Using Recurrent Neural Networks](https://link-springer-com.ccl.idm.oclc.org/chapter/10.1007/978-3-030-44267-5_20)

<!-- ### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/hfmandell/NN-Project/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
 -->
