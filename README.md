# Disease-Extraction
Problem Statement
Clinical studies often require detailed patients’ information documented in clinical narratives. Named Entity Recognition (NER) is a fundamental Natural Language Processing (NLP) task to extract entities of interest (e.g., disease names, medication names and lab tests) from clinical narratives, thus to support clinical and translational research. Clinical notes have been analyzed in greater detail to harness important information for clinical research and other healthcare operations, as they depict rich, detailed medical information.

In this problem, we have to extract all disease names from a given set of 20000 paragraphs/documents in the test set provided the labelled entities (diseases) for 30000 documents in the train set.

For example, here is a sentence from a clinical report: We compared the inter-day reproducibility of post-occlusive reactive hyperemia (PORH) assessed by single-point laser Doppler flowmetry (LDF) and laser speckle contrast analysis (LSCI).

In the sentence given, reactive hyperemia (in bold) is the named entity with the type disease/indication

Data Description
The train file has the following structure:

Variable Definition

id Unique ID for a token/word

Doc_ID Unique ID for a Document/Paragraph

Sent_ID Unique ID for a Sentence

Word Exact word/token

tag(Target) Named Entity Tag

The target 'tag' follows the Inside-outside-beginning (IOB) tagging format. The IOB format (short for inside, outside, beginning) is a common tagging format for tagging tokens in named-entity recognition.

• The B-indications (beginning) tag indicates that the token is the beginning of a disease entity (disease name in this case)

• An I-indications (inside) tag indicates that the token is inside an entity

• An O (outside) tag indicates that a token is outside a disease entity

DataSet:
1.train.csv
2.test.csv
