---
layout: archive
title: "Projects"
permalink: /projects/project4
author_profile: true
---

**Summary** The Federated Learning framework provides privacy-preserving algorithms to learn a valid machine
learning model without centralizing the data. In the training process, a central server collects model
parameter updates from clients and aggregates the local model updates to update the global model.
Depending on the heterogeneity between clients and the trust level assigned to the clients, robust aggregation rules can be applied in the global model update procedure to protect the central server against
attacks on the client side. 

On the other hand, clients borrow information from their neighbors in a
decentralized Federated Learning framework to protect against the attack on the central server side.
Centralized Federated Learning and Decentralized Federated Learning both incorporate massive clientserver/client-client communication. Applying the quantization procedure to the model updates, increasing the local iterations before each communication round, and one-shot updating with higher-order approximation would save bandwidth in communication and enhance computation efficiency. We glimpse
over some of the common set-ups for Federated Learning, starting at the most basic setup of the Federated Averaging Algorithm and considering extensions to suit various practical concerns, such as model
poisoning due to attacks and heterogeneity between clients.


We also present a simple simulation study
to showcase the application of Federated Learning in logistic regression, demonstrating the behavior of
estimates with respect to the sample size and the model size.


<img src="https://github.com/YSiAllison/YSiAllison.github.io/blob/master/files/Fig1.ga_gmiu.png" alt="projects" width="1000"/>









