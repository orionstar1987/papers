# papers

## NLP

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
      <td></td>
      <td>RNN</td>
      <td></td>
      <td>Vanishing & Exploding Gradients problems</td>
      <td><a href="https://www.semanticscholar.org/paper/Attention-is-All-you-Need-Vaswani-Shazeer/204e3073870fae3d05bcbc2f6a8e263d9b72e776"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F204e3073870fae3d05bcbc2f6a8e263d9b72e776%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td></td>
      <td>LSTM</td>
      <td></td>
      <td>
        <ul>
          <li>2 separate paths (long term memories and short term memories)</li>
          <li>3 gates (forget, input, output)</li>
        </ul>
      </td>
      <td><a href="https://www.semanticscholar.org/paper/Attention-is-All-you-Need-Vaswani-Shazeer/204e3073870fae3d05bcbc2f6a8e263d9b72e776"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F204e3073870fae3d05bcbc2f6a8e263d9b72e776%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td>2014.9</td>
      <td>seq2seq</td>
      <td><a href="https://arxiv.org/abs/1409.3215">Sequence to Sequence Learning with Neural Networks</a></td>
      <td>
        <ul>
          <li>machine translation: can handle variable input and variable output lengths</li>
          <li>decouple Encoder and Decoder </li>
          <li>use Embeddings as input </li>
          <li>stacked LSTM cells and layers for both Encoder and Decoder</li>
          <li>Teacher Forcing: during training, use the known/actual words and stop at the known phrase length, rather than using the predicted tokens</li>
        </ul>
      </td>
      <td><a href="https://www.semanticscholar.org/paper/Sequence-to-Sequence-Learning-with-Neural-Networks-Sutskever-Vinyals/cea967b59209c6be22829699f05b8b1ac4dc092d"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2Fcea967b59209c6be22829699f05b8b1ac4dc092d%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td>2017.6</td>
      <td>Transformer</td>
      <td><a href="https://arxiv.org/abs/1706.03762">Attention is All You Need</a></td>
      <td>
        <ul>
          <li>#4 DL architecture after MLP、CNN、RNN</li>
          <li>LSTM architecture is not needed anymore: for longer phrases, words that are input early on can be forgotten</li>
          <li>Encoding stays the same. Each step of the Decoding has access to the individual Encodings for each input word (similarity score)</li>
        </ul>
      </td>
      <td><a href="https://www.semanticscholar.org/paper/Attention-is-All-you-Need-Vaswani-Shazeer/204e3073870fae3d05bcbc2f6a8e263d9b72e776"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F204e3073870fae3d05bcbc2f6a8e263d9b72e776%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td>2018.6</td>
      <td>GPT</td>
      <td><a href="https://s3-us-west-2.amazonaws.com/openai-assets/research-covers/language-unsupervised/language_understanding_paper.pdf">Improving Language Understanding by Generative Pre-Training</a></td>
      <td>使用 Transformer 解码器来做预训练</td>
      <td><a href="https://www.semanticscholar.org/paper/Improving-Language-Understanding-by-Generative-Radford-Narasimhan/cd18800a0fe0b668a1cc19f2ec95b5003d0a5035"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2Fcd18800a0fe0b668a1cc19f2ec95b5003d0a5035%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td>2018.10</td>
      <td>BERT</td>
      <td><a href="https://arxiv.org/abs/1810.04805">BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding</a></td>
      <td>
        <ul>
          <li>Transformer一统NLP的开始</li>
          <li>BERT = Pretrain Deep Bidirectional Transformer (GPT: transformer but uni-directional; ELMO: bi-directional but RNN-based)</li>
          <li>Masked Language Model (token level): randomly masks some tokens from the input, and the objective is the prediction these masked tokens</li>
          <li>Next Sentence Prediciton (sentence level): learn sentence-level relationship</li>
          <li>Pe-training: unlabled data</li>
          <li>Fine-tuning: initialize with the pre-trained parameters, then use labeled data from downstream tasks to finetune</li>
        </ul>
      </td>
      <td><a href="https://www.semanticscholar.org/paper/BERT%3A-Pre-training-of-Deep-Bidirectional-for-Devlin-Chang/df2b0e26d0599ce3e70df8a9da02e51594e0e992"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2Fdf2b0e26d0599ce3e70df8a9da02e51594e0e992%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td>2019.2</td>
      <td>GPT-2</td>
      <td><a href="https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf">Language Models are Unsupervised Multitask Learners</a></td>
      <td>更大的 GPT 模型，朝着zero-shot learning迈了一大步</td>
      <td><a href="https://www.semanticscholar.org/paper/Language-Models-are-Unsupervised-Multitask-Learners-Radford-Wu/9405cc0d6169988371b2755e573cc28650d14dfe"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F9405cc0d6169988371b2755e573cc28650d14dfe%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td>2019.8</td>
      <td>Sentence BERT</td>
      <td><a href="https://arxiv.org/pdf/1908.10084.pdf">Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks</a></td>
      <td>更大的 GPT 模型，朝着zero-shot learning迈了一大步</td>
      <td><a href="https://www.semanticscholar.org/paper/Language-Models-are-Unsupervised-Multitask-Learners-Radford-Wu/9405cc0d6169988371b2755e573cc28650d14dfe"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F9405cc0d6169988371b2755e573cc28650d14dfe%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td>2020.5</td>
      <td>GPT-3</td>
      <td><a href="https://arxiv.org/abs/2005.14165">Language Models are Few-Shot Learners</a></td>
      <td>100倍更大的 GPT-2，few-shot learning效果显著</td>
      <td><a href="https://www.semanticscholar.org/paper/Language-Models-are-Few-Shot-Learners-Brown-Mann/6b85b63579a916f705a8e10a49bd8d849d91b1fc"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F6b85b63579a916f705a8e10a49bd8d849d91b1fc%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td>2022.4</td>
      <td>LLM Computation</td>
      <td><a href="https://proceedings.neurips.cc/paper_files/paper/2022/file/c1e2faff6f588870935f114ebe04a3e5-Paper-Conference.pdf">Training Compute-Optimal Large Language Models</a></td>
      <td>The model size and the number of training tokens should be scaled equally: for every doubling of model size the number of training tokens should also be doubled</td>
      <td><a href="https://www.semanticscholar.org/paper/An-empirical-analysis-of-compute-optimal-large-Hoffmann-Borgeaud/bb0656031cb17adf6bac5fd0fe8d53dd9c291508"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2Fbb0656031cb17adf6bac5fd0fe8d53dd9c291508%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
    <tr>
      <td>2023.3</td>
      <td>BloombergGPT</td>
      <td><a href="https://arxiv.org/abs/2303.17564">BloombergGPT: A Large Language Model for Finance</a></td>
      <td>
        <ul>
          <li>Combines both financial data (363 billion token) with general-purpose datasets (345 billion token)</li>
          <li>Decoder-only Transformer</li>
          <li>Much better on financial tasks. On par on general NLP tasks</li>
          <li>FinTech use cases: sentiment analysis, named entity recognition, news classification, Q&A</li>
        </ul>
      </td>
      <td><a href="https://www.semanticscholar.org/paper/BloombergGPT%3A-A-Large-Language-Model-for-Finance-Wu-Irsoy/83edcfbb206ddad38a971d605da09390604248ea"><img src="https://img.shields.io/badge/dynamic/json?label=citation&query=citationCount&url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F83edcfbb206ddad38a971d605da09390604248ea%3Ffields%3DcitationCount" alt="citation"></a></td>
    </tr>
  </tbody>
</table>
