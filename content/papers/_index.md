---
title: "Papers"
---

<div style="max-width: 760px; margin: 2rem auto; font-size: 1rem;">

### **Split-Efficient: Transferring the Pre-trained Transformer Language Model’s Knowledge to a more Communication Efficient Design for Split and Federated Learning**

<div style="display: flex; flex-wrap: wrap; gap: 0.5rem; margin: 1rem 0 1.5rem 0;">
  <span style="display: inline-block; padding: 0.4rem 0.8rem; background-color: rgba(63, 185, 80, 0.15); border: 1px solid rgba(63, 185, 80, 0.4); border-radius: 6px; font-size: 0.85rem; font-weight: 500; color: #3fb950;">Split & Federated Learning</span>
  <span style="display: inline-block; padding: 0.4rem 0.8rem; background-color: rgba(63, 185, 80, 0.15); border: 1px solid rgba(63, 185, 80, 0.4); border-radius: 6px; font-size: 0.85rem; font-weight: 500; color: #3fb950;">Knowledge Distillation</span>
  <span style="display: inline-block; padding: 0.4rem 0.8rem; background-color: rgba(63, 185, 80, 0.15); border: 1px solid rgba(63, 185, 80, 0.4); border-radius: 6px; font-size: 0.85rem; font-weight: 500; color: #3fb950;">Large Language Models (LLMs)</span>
  <span style="display: inline-block; padding: 0.4rem 0.8rem; background-color: rgba(63, 185, 80, 0.15); border: 1px solid rgba(63, 185, 80, 0.4); border-radius: 6px; font-size: 0.85rem; font-weight: 500; color: #3fb950;">Communication Efficiency</span>
</div>

</div>

<div style="max-width: 760px; margin: 2rem auto; font-size: 0.90rem;">

#### **Abstract**

<div style="background-color: rgba(255, 255, 255, 0.03); border-left: 4px solid var(--accent); padding: 1.2rem 1.6rem; border-radius: 4px; line-height: 1.7; text-align: justify; color: rgba(255, 255, 255, 0.9);">
Split and Federated learning technique has emerged as a combination of both counterparts as a solution to both privacy preservation by not sharing user data in model training; And to tackle the resource in-efficiency of pure federated learning, which requires all the clients of the federation to train the whole model separately. When adopting the split and federated design to transformer based large language models we face two main obstacles: First, unlike in classification models, the ground-truth/ generated response of a language model may also contain confidential information - requiring us to keep the both the training prompt and response hidden; Secondly, split learning requires the split models to share massive activation tensors back and forth in both training and inference. A simple architectural extension where we split the model in to three parts and host the models containing input and output layers at the client solves the problem of keeping both prompt and response hidden. But having two splits further worsens the communication problem of passing huge activation tensors back and forth for forward and backward propagation. To put this into perspective, we can imagine how every token is represented as a vector of thousands of dimensions in these intermediate hidden states and how that would effectively bloat up the bandwidth and consume a large amount of data in both training and inference in split and federated settings.
<br><br>
To this end, we propose a method — <strong>Split-Efficient</strong> — to pre-train a more communication efficient models with low dimensional hidden states at split locations by transferring the knowledge from an arbitrary pre-trained model. This compresses the communication related to forward and backward propagation upto <strong>95%</strong> and keeps over <strong>90%</strong> of the pre-trained performance of the original model, all the while incurring a tiny fraction of the computation compared to original model's pre-training, enabling us to build efficient models upto 7B parameters on a single moderate-level GPU. We further show our models' capability in post training in split federated settings achieving similar performance to their federated counterparts. We demonstrate this learnability with various datasets and training schemes such as supervised fine tuning and reinforcement learning.
</div>

</div>
