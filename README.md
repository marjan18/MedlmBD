While Large Language Models (LLMs)
have shown great promise in medical question answer
ing, the majority of medical LLMs primarily cater to
high-resource languages, which hinders their accessi
bility to Bengali speakers. This paper introduces a
translation-augmented medical assistant for managing
medical queries in Bengali, namely MedlmBD. The
system uses the NLLB-200 multilingual translation
model to facilitate seamless interaction with an En
glish medical LLM through a Bengali-English pipeline.
Datacleaning, instruction formatting, tokenization and
shuffling are performed on the ChatDoctor dataset
(subset). The SmolLM3-3B model is fine-tuned using
the parameter-efficient Quantized Low-Rank Adapta
tion (QLoRA). The proposed framework fine-tunes
the lightweight SmolLM3-3B model for the Bengali
medical Q&A task, yielding accuracy, precision, recall,
specificity, and F1 scores of 86.80%, 91.19%, 81.46%,
92.13%, and 86.05% respectively. The cosine similarity
of generated responses is also 0.5033, showing that the
responses retain clinically relevant semantic content
even if they vary in their lexical content. Despite
using only a fraction of the parameters and being fine
tuned only on a subset of the ChatDoctor dataset,
Fine-tuned SmolLM3-3B is competitive with the larger
MedAlpaca-7b model. MedlmBD’s ability to deliver
bilingual information helps make healthcare informa
tion more accessible for Bengali speakers, while the
efficient 4-bit quantization and QLoRA fine-tuning pro
vide an efficient approach to evaluate the performance
of multilingual healthcare AI systems practically and
effectively
