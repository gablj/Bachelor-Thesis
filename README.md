# Bachelor-Thesis
A repostirory for my Bachelor Thesis: "Deep Learning Based End-to-End Text-Independent Speaker Verification"

# Abstract
Speech processing is one of the most active areas of research and development in Deep Learning.
However, compared to other more common domains, the progress in speech processing has
been relatively less pronounced. This is primarily due to the inherent challenge that imposes
the extraction of meaningful statistical and discriminative features from speech signals. Previous
advancements in speech processing often relied on manual feature modeling, requiring
significant effort from developers and researchers.
Recent experimentation with neural networks architectures has shown promising results in
obtaining low-dimensional vector representations of speech signals, while requiring minimal
preprocessing and simplifying the feature extraction process. Embeddings obtained from these
experiments have reported to be comparable, and sometimes even superior, to traditional feature
modeling methods. This has impulsed the development of models that effectively address
challenging speech processing tasks, such as speaker verification.
Speaker verification is the task of accepting or rejecting a speakers identity claim through the
analysis of their speech signals. In this work we focus on text-independent speaker verification,
which is the most challenging subset of speaker verification tasks. For this task the verification
process is not dependent from a specific phrase, meaning that the user can claim their identity by
speaking any phrase, and the model must verify this claim based on the characteristics extracted
from this arbitrary speech signal.
In traditional speaker verification systems the pipeline consists of three distinct steps: development,
enrollment and verification. For which the development and enrollment steps are
trained separately from the verification model. In this work, we present an end-to-end approach
based on the Generalized End-to-End (GE2E) method proposed by Google researchers. Our
approach employs a single network architecture that directly maps utterances’ log-Mel filterbank
energy vectors to discriminative speaker embeddings. The architecture emulates the three
steps of the traditional speaker verification pipeline while optimizing a unified loss function that
encourages close proximity of utterance embeddings from the same speaker while increasing
the distance from embeddings coming from different speakers in the embedding space. Our
implementation is designed to be trained on small scale datasets, including fewer than 1, 500
speakers. Despite this limitation, it has yielded favorable results, demonstrating the effectiveness
of our architecture for speaker modeling and verification, which further emphasizes the potential
of deep learning in advancing the field of speech processing.
