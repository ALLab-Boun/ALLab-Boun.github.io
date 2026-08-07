---
title: Projects
nav:
  order: 3
#  tooltip: Software, datasets, and more
---

# {% include icon.html icon="fa-solid fa-university" %}Projects

{% include section.html %}

## Alzheimer's Disease 

{% capture text %}
Alzheimer's disease (AD) is a neurodegenerative disorder that is one of the primary causes of dementia. Our research focuses on developing methods to improve the understanding of AD prognosis and to support clinical research. 

We proposed a latent-space manipulation-based approach to generate synthetic conversion visits. Using a variational autoencoder's latent space, the changes in the biomarkers of an MCI patient who converts to AD were studied. 

<a href="https://arxiv.org/abs/2111.08794" target="_blank" rel="noopener noreferrer">For more click here</a>

{%
  include button.html
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/advprog.png"
  text=text
%}

{% capture text %}
In ADVPROG, an adversarial progression framework, we aimed to reduce the complexity of the MCI-to-AD prediction by employing adversarial attacks on a shallow multilayer perceptron. The magnitude of the attack was used to infer the patient's proximity to conversion. The ADVPROG framework was used for both conversion prediction and subtyping.

<a href="https://ieeexplore.ieee.org/abstract/document/10476682" target="_blank" rel="noopener noreferrer">For more click here</a>

{%
  include button.html
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/advprog.png"
  text=text
%}
{% capture text %}
FATE-Net was developed as an attention-based architecture for predicting conversion from Mild Cognitive Impairment (MCI) to AD. The proposed architecture treats visit time as a separate modality to capture the correlation between time and feature significance.

<a href="https://link.springer.com/article/10.1007/s10044-025-01447-4" target="_blank" rel="noopener noreferrer">For more click here</a>

{% capture text %}
A local dataset was collected in collaboration with the Department of Neurology at the University of Health Sciences Sultan Abdulhamid Han Research and Training Hospital in İstanbul, Türkiye. We analyzed the MRI regional volumes of 1547 visits of 474 MCI and AD patients. This research was supported by the Scientific and Technological Research Council of Türkiye (TÜBİTAK) under grant number 121E594.

<a href="https://www.mdpi.com/2077-0383/15/6/2250" target="_blank" rel="noopener noreferrer">For more click here</a>

{%
  include button.html
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/chat-gnn.png"
  text=text
%}



{% include section.html %}

## Graph Neural Networks

{% capture text %}

Graph neural networks (GNNs) set the state of the art for a wide variety of applications, including social networks and complex molecules. Most commonly used GNN architectures leverage the message-passing paradigm. On the other hand, the message-passing mechanism suffers from several issues. 

We proposed CHAT-GNN, a channel-attentive GNN architecture, to mitigate over-smoothing that emerges as GNN's depth increases. In CHAT-GNN, by computing the messages via learning how to attend neighboring nodes and their feature channels, we aimed to increase the diversity of the information transferred between nodes. 

<a href="https://ieeexplore.ieee.org/abstract/document/10884168" target="_blank" rel="noopener noreferrer">For more click here</a>

{%
  include button.html
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/chat-mini.png"
  flip=true
  text=text
%}
{% capture text %}
Local virtual nodes (LVN) were developed to address the over-squashing challenge caused by bottlenecks during message passing, which disrupts the modeling of long-range dependencies. The LVN framework aims to improve the connectivity in the regions with likely bottlenecks by adding trainable virtual node embeddings shared across selected central regions. 

<a href="https://arxiv.org/abs/2508.20597" target="_blank" rel="noopener noreferrer">For more click here</a>

{%
  include button.html
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/lvn-mini.png"
  flip=true
  text=text
%}

{% include section.html %}

## Adversarial Robustness

{% capture text %}


Robustness-via-synthesis: Robust training with generative adversarial perturbations
<a href="https://www.sciencedirect.com/science/article/pii/S0925231222013091" target="_blank" rel="noopener noreferrer">For more click here</a>

Perturbation Augmentation for Adversarial Training with Diverse Attacks
<a href="https://dergipark.org.tr/en/pub/gujsa/article/1458880" target="_blank" rel="noopener noreferrer">For more click here</a>


Adversarial Robustness for Deep Metric Learning
<a href="https://ieeexplore.ieee.org/abstract/document/10647877" target="_blank" rel="noopener noreferrer">For more click here</a>

Out-of-Distribution Detection with Prototype Similarity
<a href="https://ieeexplore.ieee.org/abstract/document/10884282" target="_blank" rel="noopener noreferrer">For more click here</a>




{%
  include button.html
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  text=text
%}
