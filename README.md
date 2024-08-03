# Table of Contents

[Introduction](#introduction)

[How to Run](#howtorun)

<a name="introduction"/>

# Introduction

This repo presents code for Deep Learning based algorithm for
**detecting violence** in indoor or outdoor environments. The algorithm can
detect following scenarios with high accuracy: fight, fire, car crash and even
more.

To detect other scenarios you have to add **descriptive text label** of a
scenario in `settings.yaml` file under `labels` key. At this moment model can
detect 16`+1` scenarios, where one is default `Unknown` label. You can change,
add or remove labels according to your use case. The model is trained on wide
variety of data. The task for the model at training was to predict similar
vectors for image and text that describes well a scene on the image. Thus model
can generalize well on other scenarios too if you provide proper textual
information about a scene of interest.
<a name="howtorun"/>

# How to Run

First install requirements:
`pip install -r requirements.txt`

To test the model you can either run:
`python run.py --image-path ./data/7.jpg`

Or you can test it through web app:
`streamlit run app.py`

