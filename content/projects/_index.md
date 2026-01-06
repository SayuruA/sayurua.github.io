---
title: "Projects"
---

<div style="max-width: 760px; margin: 2rem auto; font-size: 1rem;">

**Final Year Project: Training LLMs on privacy-sensitive data in resource-constrained environments (2-mins)**

<div style="display: flex; flex-wrap: wrap; gap: 0.5rem; margin: 1rem 0 1.5rem 0;">
  <span style="display: inline-block; padding: 0.4rem 0.8rem; background-color: rgba(63, 185, 80, 0.15); border: 1px solid rgba(63, 185, 80, 0.4); border-radius: 6px; font-size: 0.85rem; font-weight: 500; color: #3fb950;">Federated Learning (FL)</span>
  <span style="display: inline-block; padding: 0.4rem 0.8rem; background-color: rgba(63, 185, 80, 0.15); border: 1px solid rgba(63, 185, 80, 0.4); border-radius: 6px; font-size: 0.85rem; font-weight: 500; color: #3fb950;">Split-Federated Learning (SFL)</span>
  <span style="display: inline-block; padding: 0.4rem 0.8rem; background-color: rgba(63, 185, 80, 0.15); border: 1px solid rgba(63, 185, 80, 0.4); border-radius: 6px; font-size: 0.85rem; font-weight: 500; color: #3fb950;">Large Language Models (LLMs)</span>
  <span style="display: inline-block; padding: 0.4rem 0.8rem; background-color: rgba(63, 185, 80, 0.15); border: 1px solid rgba(63, 185, 80, 0.4); border-radius: 6px; font-size: 0.85rem; font-weight: 500; color: #3fb950;">Open Radio Access Networks (O-RAN)</span>
</div>

</div>

<div style="max-width: 760px; margin: 2rem auto; font-size: 0.90rem;">

Google can train AI models on our private data without reading a single one. 

They used a training scheme called federated learning, where separate models are hosted and trained in each device and their knowledge is periodically combined to form a global model.

<figure style="
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 2rem auto;
  max-width: 500px;
">
  <img src="/images/FL.png" width="600" style="border-radius: 8px; max-width: 100%;" />
  <figcaption style="font-size: 0.8rem; opacity: 0.75; margin-top: 0.4rem; text-align: center; max-width: 100%;">
    FL - Don't need to collect data, send the model to user!
  </figcaption>
</figure>

But requiring to train the model in each device is not scalable, especially for large (vision) language models (LVLMs). A technique called Split-Federated learning proposes to delegate the large amount of computation to a cloud server while keeping the data from leaving the user's device.

While this sounds quite appealing, it is not without practical challenges when it comes to actual deployment. For one, feasibilty research done in using this approach with LVLMs is still in its infancy. And the massive size of tensors that needs to get passed between the cloud and the devices is one of the biggest reasearch/ engineering challenges yet to be solved.

<figure style="
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 2rem auto;
  max-width: 680px;
">
  <img src="/images/fyp.png" width="800" style="border-radius: 8px; max-width: 100%;" />
  <figcaption style="font-size: 0.8rem; opacity: 0.75; margin-top: 0.4rem; text-align: center; max-width: 100%;">
    Our high level architecture - Keeps a few layers at both the input and the output side of model at user. Testbeds at UoM and UCD are taken as users/ clients.
  </figcaption>
</figure>


In this final year project we strive to explore solutions to these challenges, and build a model that auotmates security related administartive tasks in an Open Radio Access Network (O-RAN).

While we focus on a specific use case in networks (O-RAN), as a drop-in replacement for federated learning, we believe this approach with more advancements in the future is the way to train large models on privacy-sensitive data all the while keeping the end devices from getting bloated-out with model training. We are working with Dr. [Kasun Hemachandra](https://scholar.google.com/citations?user=RT8_dlYAAAAJ&hl=en) and Prof. [Tharaka Samarasinghe](https://tharakas.staff.uom.lk/) from department of Electronic and Telecommunication University of Moratuwa, Sri Lanka and Prof. [Madushanka Liyanage](https://www.madhusanka.com/) from NetsLab University College Dublin, Ireland.

Current Progress:
- Integrate compression mechanisms to existing split federated learning pipeline.
- Practical Deployment on an Open Radio Access Network (O-RAN) testbed.

</div>

<!-- My Team: -->



