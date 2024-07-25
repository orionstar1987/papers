## What is Synthetic Data Generation (SDG)?
SDG involves generating artificial data and labels, aiming to emulate authentic samples closely. This process is automated by utilizing generative models that estimate the __probability distribution__ of their training data.
- Different from data augmentation, which manipulates existing data. SDG generates new data by samping from learned distributions.
-  Synthetic data proves highly valuable when real data is insufficient, costly to label, or exhibits biased distributions.

## Model Evolving
Shift from simpler probabilistic models like Markov chains and Bayesian Networks (BNs) to more sophisticated neural network-based approaches, such as GANs, RNN, autoencoders, Transformers, RL.

## Guideline for SDG
- For image generation and related purposes, diffusion models and GANs are the best options quality-wise. GANs are better for situations where less training data is available. Autoencoders are a less powerful but also a less resource-demanding alternative.
- Generation of sequential data like symbolic music, time series, most graph/molecule representations, and text is a suitable task for transformers and RNNs. Markov chains are a less powerful but simple and efficient alternative that humans can inspect.
- Autoencoders, especially VAEs, are good unsupervised feature learners that can disentangle and recombine features from training data to produce new data with desired properties.
- CNNs are a common building block of models to make them suitable to process high-dimensional data like large-resolution images and audio waveforms, whose sizes otherwise significantly slow down the training process or increase model size beyond a processable point.

## Distillation
- One model teaches another
- Supervised
- Close to human-created data

### Methods
- Self-instruct (easiest)
- Evol-instruct (challenging)
    - Separate the timing of generating prompt and answers
    - Add a process to slightly increase of the difficulty of the prompt
- LAB - Large-scale Alignment of Bots (more diverse data)
- Task-specific (Open math)
- Knowledge-specific (QA)

## Self-improvement
- Model improves itself


## Related Papers
<table>
  <thead>
    <tr>
      <th>Date</th>
      <th>Category</th>
      <th>Paper Name</th>
      <th>Description</th>
      <th>Citation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>2024.6</td>
      <td>SDG</td>
      <td><a href="https://developer.nvidia.com/blog/leverage-our-latest-open-models-for-synthetic-data-generation-with-nvidia-nemotron-4-340b/">NVIDIA Nemotron-4 340B</a></td>
      <td>
        <ul>
          <li>NVIDIA's new suite of models specifically built for SDG, including a state-of-the-art Reward Model, and a Instruct model to aid in SDG</li>
        </ul>
      </td>
   <td>
      </td>
    </tr>
    <tr>
      <td>2024.2</td>
      <td>SDG</td>
      <td><a href="https://arxiv.org/pdf/2401.02524">Comprehensive Exploration of Synthetic Data Generation: A Survey</a></td>
      <td>
      </td>
      <td><a href="https://www.semanticscholar.org/paper/Sequential-Recommender-Systems%3A-Challenges%2C-and-Wang-Hu/d837642802ffc85e193694f94f7499276864648e"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F4ec981ed24911e9f5cf1162930eb19321bcdafcb%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td>2023.10</td>
      <td>SDG</td>
      <td><a href="https://arxiv.org/pdf/2310.07849">Synthetic Data Generation with Large Language Models for Text Classification: Potential and Limitationsn</a></td>
      <td>
      </td>
      <td><a href="https://www.semanticscholar.org/paper/Sequential-Recommender-Systems%3A-Challenges%2C-and-Wang-Hu/d837642802ffc85e193694f94f7499276864648e"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F29f07e73b7aaa7e9e950c59710472c62316be74a%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>