Transformers
=======================================================================================================================

State-of-the-art Natural Language Processing for Pytorch and TensorFlow 2.0.

🤗 Transformers (formerly known as `pytorch-transformers` and `pytorch-pretrained-bert`) provides general-purpose
architectures (BERT, GPT-2, RoBERTa, XLM, DistilBert, XLNet...) for Natural Language Understanding (NLU) and Natural
Language Generation (NLG) with over 32+ pretrained models in 100+ languages and deep interoperability between
TensorFlow 2.0 and PyTorch.

This is the documentation of our repository `transformers <https://github.com/huggingface/transformers>`_.

Features
-----------------------------------------------------------------------------------------------------------------------

- High performance on NLU and NLG tasks
- Low barrier to entry for educators and practitioners

State-of-the-art NLP for everyone:

- Deep learning researchers
- Hands-on practitioners
- AI/ML/NLP teachers and educators

Lower compute costs, smaller carbon footprint:

- Researchers can share trained models instead of always retraining
- Practitioners can reduce compute time and production costs
- 8 architectures with over 30 pretrained models, some in more than 100 languages

Choose the right framework for every part of a model's lifetime:

- Train state-of-the-art models in 3 lines of code
- Deep interoperability between TensorFlow 2.0 and PyTorch models
- Move a single model between TF2.0/PyTorch frameworks at will
- Seamlessly pick the right framework for training, evaluation, production

Contents
-----------------------------------------------------------------------------------------------------------------------

The documentation is organized in five parts:

- **GET STARTED** contains a quick tour, the installation instructions and some useful information about our philosophy
  and a glossary.
- **USING 🤗 TRANSFORMERS** contains general tutorials on how to use the library.
- **ADVANCED GUIDES** contains more advanced guides that are more specific to a given script or part of the library.
- **RESEARCH** focuses on tutorials that have less to do with how to use the library but more about general resarch in
  transformers model
- The three last section contain the documentation of each public class and function, grouped in:
    - **MAIN CLASSES** for the main classes exposing the important APIs of the library.
    - **MODELS** for the classes and functions related to each model implemented in the library.
    - **INTERNAL HELPERS** for the classes and functions we use internally.

The library currently contains PyTorch and Tensorflow implementations, pre-trained model weights, usage scripts and
conversion utilities for the following models:

1. `BERT <https://github.com/google-research/bert>`_ (from Google) released with the paper `BERT: Pre-training of Deep
   Bidirectional Transformers for Language Understanding <https://arxiv.org/abs/1810.04805>`_ by Jacob Devlin, Ming-Wei
   Chang, Kenton Lee, and Kristina Toutanova.
2. `GPT <https://github.com/openai/finetune-transformer-lm>`_ (from OpenAI) released with the paper `Improving Language
   Understanding by Generative Pre-Training <https://blog.openai.com/language-unsupervised>`_ by Alec Radford, Karthik
   Narasimhan, Tim Salimans, and Ilya Sutskever.
3. `GPT-2 <https://blog.openai.com/better-language-models>`_ (from OpenAI) released with the paper `Language Models are
   Unsupervised Multitask Learners <https://blog.openai.com/better-language-models>`_ by Alec Radford, Jeffrey Wu,
   Rewon Child, David Luan, Dario Amodei, and Ilya Sutskever.
4. `Transformer-XL <https://github.com/kimiyoung/transformer-xl>`_ (from Google/CMU) released with the paper
   `Transformer-XL: Attentive Language Models Beyond a Fixed-Length Context <https://arxiv.org/abs/1901.02860>`_ by
   Zihang Dai, Zhilin Yang, Yiming Yang, Jaime Carbonell, Quoc V. Le, and Ruslan Salakhutdinov.
5. `XLNet <https://github.com/zihangdai/xlnet>`_ (from Google/CMU) released with the paper `​XLNet: Generalized
   Autoregressive Pretraining for Language Understanding <https://arxiv.org/abs/1906.08237>`_ by Zhilin Yang, Zihang
   Dai, Yiming Yang, Jaime Carbonell, Ruslan Salakhutdinov, and Quoc V. Le.
6. `XLM <https://github.com/facebookresearch/XLM>`_ (from Facebook) released together with the paper `Cross-lingual
   Language Model Pretraining <https://arxiv.org/abs/1901.07291>`_ by Guillaume Lample and Alexis Conneau.
7. `RoBERTa <https://github.com/pytorch/fairseq/tree/master/examples/roberta>`_ (from Facebook), released together with
   the paper a `Robustly Optimized BERT Pretraining Approach <https://arxiv.org/abs/1907.11692>`_ by Yinhan Liu, Myle
   Ott, Naman Goyal, Jingfei Du, Mandar Joshi, Danqi Chen, Omer Levy, Mike Lewis, Luke Zettlemoyer, and Veselin
   Stoyanov.
8. `DistilBERT <https://huggingface.co/transformers/model_doc/distilbert.html>`_ (from HuggingFace) released together
   with the paper `DistilBERT, a distilled version of BERT: smaller, faster, cheaper and lighter
   <https://arxiv.org/abs/1910.01108>`_ by Victor Sanh, Lysandre Debut, and Thomas Wolf. The same method has been
   applied to compress GPT2 into
   `DistilGPT2 <https://github.com/huggingface/transformers/tree/master/examples/distillation>`_.
9. `CTRL <https://github.com/pytorch/fairseq/tree/master/examples/ctrl>`_ (from Salesforce), released together with the
   paper `CTRL: A Conditional Transformer Language Model for Controllable Generation
   <https://www.github.com/salesforce/ctrl>`_ by Nitish Shirish Keskar, Bryan McCann, Lav R. Varshney, Caiming Xiong,
   and Richard Socher.
10. `CamemBERT <https://huggingface.co/transformers/model_doc/camembert.html>`_ (from FAIR, Inria, Sorbonne Université)
    released together with the paper `CamemBERT: a Tasty French Language Model <https://arxiv.org/abs/1911.03894>`_ by
    Louis Martin, Benjamin Muller, Pedro Javier Ortiz Suarez, Yoann Dupont, Laurent Romary, Eric Villemonte de la
    Clergerie, Djame Seddah, and Benoît Sagot.
11. `ALBERT <https://github.com/google-research/ALBERT>`_ (from Google Research), released together with the paper
    `ALBERT: A Lite BERT for Self-supervised Learning of Language Representations <https://arxiv.org/abs/1909.11942>`_
    by Zhenzhong Lan, Mingda Chen, Sebastian Goodman, Kevin Gimpel, Piyush Sharma, and Radu Soricut.
12. `T5 <https://github.com/google-research/text-to-text-transfer-transformer>`_ (from Google) released with the paper
    `Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer
    <https://arxiv.org/abs/1910.10683>`_ by Colin Raffel, Noam Shazeer, Adam Roberts, Katherine Lee, Sharan Narang,
    Michael Matena, Yanqi Zhou, Wei Li, and Peter J. Liu.
13. `XLM-RoBERTa <https://github.com/pytorch/fairseq/tree/master/examples/xlmr>`_ (from Facebook AI), released together
    with the paper `Unsupervised Cross-lingual Representation Learning at Scale <https://arxiv.org/abs/1911.02116>`_ by
    Alexis Conneau, Kartikay Khandelwal, Naman Goyal, Vishrav Chaudhary, Guillaume Wenzek, Francisco Guzmán, Edouard
    Grave, Myle Ott, Luke Zettlemoyer, and Veselin Stoyanov.
14. `MMBT <https://github.com/facebookresearch/mmbt/>`_ (from Facebook), released together with the paper a `Supervised
    Multimodal Bitransformers for Classifying Images and Text <https://arxiv.org/pdf/1909.02950.pdf>`_ by Douwe Kiela,
    Suvrat Bhooshan, Hamed Firooz, and Davide Testuggine.
15. `FlauBERT <https://github.com/getalp/Flaubert>`_ (from CNRS) released with the paper `FlauBERT: Unsupervised
    Language Model Pre-training for French <https://arxiv.org/abs/1912.05372>`_ by Hang Le, Loïc Vial, Jibril Frej,
    Vincent Segonne, Maximin Coavoux, Benjamin Lecouteux, Alexandre Allauzen, Benoît Crabbé, Laurent Besacier, and
    Didier Schwab.
16. `BART <https://github.com/pytorch/fairseq/tree/master/examples/bart>`_ (from Facebook) released with the paper
    `BART: Denoising Sequence-to-Sequence Pre-training for Natural Language Generation, Translation, and Comprehension
    <https://arxiv.org/pdf/1910.13461.pdf>`_ by Mike Lewis, Yinhan Liu, Naman Goyal, Marjan Ghazvininejad, Abdelrahman
    Mohamed, Omer Levy, Ves Stoyanov, and Luke Zettlemoyer.
17. `ELECTRA <https://github.com/google-research/electra>`_ (from Google Research/Stanford University) released with
    the paper `ELECTRA: Pre-training text encoders as discriminators rather than generators
    <https://arxiv.org/abs/2003.10555>`_ by Kevin Clark, Minh-Thang Luong, Quoc V. Le, and Christopher D. Manning.
18. `DialoGPT <https://github.com/microsoft/DialoGPT>`_ (from Microsoft Research) released with the paper `DialoGPT:
    Large-Scale Generative Pre-training for Conversational Response Generation <https://arxiv.org/abs/1911.00536>`_ by
    Yizhe Zhang, Siqi Sun, Michel Galley, Yen-Chun Chen, Chris Brockett, Xiang Gao, Jianfeng Gao, Jingjing Liu,
    and Bill Dolan.
19. `Reformer <https://github.com/google/trax/tree/master/trax/models/reformer>`_ (from Google Research) released with
    the paper `Reformer: The Efficient Transformer <https://arxiv.org/abs/2001.04451>`_ by Nikita Kitaev, Łukasz
    Kaiser, and Anselm Levskaya.
20. `MarianMT <https://marian-nmt.github.io/>`_ (developed by the Microsoft Translator Team) machine translation models
    trained using `OPUS <http://opus.nlpl.eu/>`_ pretrained_models data by Jörg Tiedemann.
21. `Longformer <https://github.com/allenai/longformer>`_ (from AllenAI) released with the paper `Longformer: The
    Long-Document Transformer <https://arxiv.org/abs/2004.05150>`_ by Iz Beltagy, Matthew E. Peters, and Arman Cohan.
22. `DPR <https://github.com/facebookresearch/DPR>`_ (from Facebook) released with the paper `Dense Passage Retrieval
    for Open-Domain Question Answering <https://arxiv.org/abs/2004.04906>`_ by Vladimir Karpukhin, Barlas Oğuz, Sewon
    Min, Patrick Lewis, Ledell Wu, Sergey Edunov, Danqi Chen, and Wen-tau Yih.
23. `Pegasus <https://github.com/google-research/pegasus>`_ (from Google) released with the paper `PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization
    <https://arxiv.org/abs/1912.08777>`_ by Jingqing Zhang, Yao Zhao, Mohammad Saleh and Peter J. Liu.
24. `MBart <https://github.com/pytorch/fairseq/tree/master/examples/mbart>`_ (from Facebook) released with the paper  `Multilingual Denoising Pre-training for Neural Machine Translation <https://arxiv.org/abs/2001.08210>`_ by Yinhan Liu, Jiatao Gu, Naman Goyal, Xian Li, Sergey Edunov,
    Marjan Ghazvininejad, Mike Lewis, Luke Zettlemoyer.
25. `LXMERT <https://github.com/airsplay/lxmert>`_ (from UNC Chapel Hill) released with the paper `LXMERT: Learning
    Cross-Modality Encoder Representations from Transformers for Open-Domain Question
    Answering <https://arxiv.org/abs/1908.07490>`_ by Hao Tan and Mohit Bansal.
26. `Funnel Transformer <https://github.com/laiguokun/Funnel-Transformer>`_ (from CMU/Google Brain) released with the paper
    `Funnel-Transformer: Filtering out Sequential Redundancy for Efficient Language Processing
    <https://arxiv.org/abs/2006.03236>`_ by Zihang Dai, Guokun Lai, Yiming Yang, Quoc V. Le.
27. `Bert For Sequence Generation <https://tfhub.dev/s?module-type=text-generation&subtype=module,placeholder>`_ (from Google) released with the paper
    `Leveraging Pre-trained Checkpoints for Sequence Generation Tasks
    <https://arxiv.org/abs/1907.12461>`_ by Sascha Rothe, Shashi Narayan, Aliaksei Severyn.
28. `LayoutLM <https://github.com/microsoft/unilm/tree/master/layoutlm>`_ (from Microsoft Research Asia) released with the paper
    `LayoutLM: Pre-training of Text and Layout for Document Image Understanding
    <https://arxiv.org/abs/1912.13318>`_ by Yiheng Xu, Minghao Li, Lei Cui, Shaohan Huang, Furu Wei, Ming Zhou.
29. `Other community models <https://huggingface.co/models>`_, contributed by the `community
    <https://huggingface.co/users>`_.

.. toctree::
    :maxdepth: 2
    :caption: Get started

    quicktour
    installation
    philosophy
    glossary

.. toctree::
    :maxdepth: 2
    :caption: Using 🤗 Transformers

    task_summary
    model_summary
    preprocessing
    training
    model_sharing
    tokenizer_summary
    multilingual

.. toctree::
    :maxdepth: 2
    :caption: Advanced guides

    pretrained_models
    examples
    custom_datasets
    notebooks
    converting_tensorflow_models
    migration
    contributing
    testing
    serialization

.. toctree::
    :maxdepth: 2
    :caption: Research

    bertology
    perplexity
    benchmarks

.. toctree::
    :maxdepth: 2
    :caption: Main Classes

    main_classes/configuration
    main_classes/logging
    main_classes/model
    main_classes/optimizer_schedules
    main_classes/output
    main_classes/pipelines
    main_classes/processors
    main_classes/tokenizer
    main_classes/trainer

.. toctree::
    :maxdepth: 2
    :caption: Models

    model_doc/albert
    model_doc/auto
    model_doc/bart
    model_doc/bert
    model_doc/bertgeneration
    model_doc/camembert
    model_doc/ctrl
    model_doc/deberta
    model_doc/dialogpt
    model_doc/distilbert
    model_doc/dpr
    model_doc/electra
    model_doc/encoderdecoder
    model_doc/flaubert
    model_doc/fsmt
    model_doc/funnel
    model_doc/layoutlm
    model_doc/longformer
    model_doc/lxmert
    model_doc/marian
    model_doc/mbart
    model_doc/mobilebert
    model_doc/gpt
    model_doc/gpt2
    model_doc/pegasus
    model_doc/rag
    model_doc/reformer
    model_doc/retribert
    model_doc/roberta
    model_doc/t5
    model_doc/transformerxl
    model_doc/xlm
    model_doc/xlmroberta
    model_doc/xlnet

.. toctree::
    :maxdepth: 2
    :caption: Internal Helpers

    internal/modeling_utils
    internal/pipelines_utils
    internal/tokenization_utils
