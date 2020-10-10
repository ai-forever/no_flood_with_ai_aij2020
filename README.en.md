<p align="center">
  <img src="pics/AIJ_Logo.png" width="100%">
</p>

# NoFloodWithAI: Flash floods on the Amur River

NoFloodWithAI is a special track with a socially important theme prepared jointly with the Ministry of Emergency Situations, Ministry of Natural Resources and Rosgidromet of Russia. 

### Task description

Contestants are invited to develop an algorithm for short-term forecasting of water levels in the Amur River for the following settlements (gauging stations): Dzhalinda, Blagoveshchensk, Innokentievka, Leninskoye, Khabarovsk, Komsomolsk-on-Amur, Nikolaevsk-on-Amur for 10 days in advance in order to prevent emergency situations in Russia’s regions. The results of the contest will be reused to mitigate environmental risks and minimize economic damage wrought on the regions.

The Amur River is a transboundary river, the main part of the basin of which lies within the Russian Federation. The Amur is characterized by low water content in winter period, small floods in spring and repeated sharp rises in water in the second half of summer and early autumn. Low-water periods are followed by years of high water. In the long-term regime of the Amur water flow, the alternation of periods of low and high water content is clearly expressed, each lasting about 12-17 years. Amur, according to the assessment of hydrologists and based on the observation history, entered another period of high water content in the late 2000s. Based on this hydrological regularity of the Amur regime, in the next 5-7 years, a complex flood situation should be expected in the course of the Middle and Lower Amur (the most difficult situation is from the confluence of the Sungari River to the Komsomolsk District, inclusive).

The largest floods occurred in 2013 and 2019. The floods were caused by tropical cyclones, which carried warm humid air, caused frontal sections and heavy precipitation. In 2013, over a large area for 2-3 months the amount of precipitation has exceeded the annual, and in some places even one and a half year norm.

In order to minimize economic damage, it is necessary to create a tool for forecasting flood waves on the Amur and its tributaries.

<p align="center">
  <img src="pics/map.jpg" width="100%">
</p>

The map above shows the Amur River basin and its main tributaries, with gradation based on average water discharge. Blue points - all gauging stations from the dataset, white - gauging stations of interest, pink - weather stations.


### Dataset description

The dataset can be downloaded [тут](https://storage.yandexcloud.net/datasouls-ods/materials/c6be1003/datasets.zip).

A detailed description of this dataset can be found in [```desc/datasets_description.pdf```](https://github.com/sberbank-ai/no_flood_with_ai_aij2020/blob/main/desc/datasets_description_ru.pdf)


### Baseline

Notebook with a baseline task: [```baseline.ipynb```](https://github.com/sberbank-ai/no_flood_with_ai_aij2020/blob/main/baseline.ipynb)

### Solution description

A solution is a repository hosted on [github](https://github.com) consisting of code written in Python only, complete with comments describing the proposed approach in detail and a presentation in pdf format. Priority will be given to innovative and out-of-the-box features and solutions that will help produce the highest-quality forecast. An example of such a repository from the organizers of the hackathon can be found [here](https://github.com/denndimitrov/submission_example_amur).

The solution score will be given by the contest jury (on a scale of 0 to 10, where 10 represents the highest possible score and 0 is the lowest score). The contest jury will assess the description of the proposed approach, with the key focus on innovation, the model’s ability to be extrapolated and replicated for use at other rivers. The jury consists of the organizer’s representatives and guest experts.

Individual contestants or teams earning the highest total score will be declared track winners. 

More details about the assessment criteria can be found in [```desc/solution_requirements_en.md```](https://github.com/sberbank-ai/no_flood_with_ai_aij2020/blob/main/desc/solution_requirements_en.md)

