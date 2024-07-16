---
layout: page
title: Automatically Assessing Children's Oral Narrative Language Abilities
description: Work with Speech Processing and Auditory Perception Lab at UCLA
img: 
importance: 3
category: lab
---

This work proposes a novel framework for automatically scoring children’s oral narrative language abilities. We use audio recordings from 3rd-8th graders of the Atlanta, Georgia area as they take a portion of the Test of Narrative Language. We design a system which extracts linguistic features and fine-tuned BERT-based self-supervised learning representation from state of-the-art ASR transcripts. We predict manual test scores from the extracted features. This framework significantly outperforms a deterministic method based on the assessment’s scoring rubric. Last, we evaluate the system performance across student’s reading level, dialect, and diagnosed learning/language disabilities to establish fairness across diverse demographics of students. Using this system, we achieve approximately 98% classification accuracy of student scores. We are also able to identify key areas of improvement for this type of system across demographic areas and reading ability.


This work was presented at Interspeech 2023, and can be accessed <a href="https://www.isca-speech.org/archive/interspeech_2023/johnson23_interspeech.html"> here</a>


An extenion to this work focused on automatically scoring children’s oral assessments while they perform a picture description task. Approximately 200 children aged 9-13 participated in this task in which they tell a story about an image presented to them. We use a BERT-based system to predict assessment scores from input ASR transcripts of the student responses. Finally, we propose next design steps to make the system more applicable to an educational setting.


This extension was presented at SLaTE 2023, and can be accessed <a href="https://www.isca-speech.org/archive/slate_2023/veeramani23_slate.html"> here</a>


We also evaluate the performance of widely-used open-source automatic speech recognition systems in transcribing primarily African American English-speaking children’s speech for educational applications. We investigate the performance of the Whisper, HuBERT, and Wav2Vec2 ASR systems as well as the capability of the transformer-based language model, BERT, for automatically grading the student’s oral responses to assessment prompts through use of the generated ASR transcripts. We achieve a 95% oral response scoring accuracy through the methods described. We also show a thorough analysis of ASR system performance over a diverse set of metrics going beyond the standard word error rate.


This work was published in The Journal of Black Excellence in Engineering, Science, & Technology, and can be accessed <a href="https://nsbejournal.scholasticahq.com/article/92286.pdf"> here</a>


An extension to this work presents a novel framework for the automated prediction of item difficulty and response time within educational assessments. Utilizing data from the BEA 2024 Shared Task, we integrate Named Entity Recognition, Semantic Role Labeling, and linguistic features to prompt a Large Language Model (LLM). Our best approach achieves an RMSE of 0.308 for item difficulty and 27.474 for response time prediction, improving on the provided baseline. The framework’s adaptability is demonstrated on audio recordings of 3rd-8th graders from the Atlanta, Georgia area responding to the Test of Narrative Language. These results highlight the framework’s potential to enhance test development efficiency.


This extension was presented at the Nineteenth Workshop on Innovative Use of NLP for Building Educational Applications as part of NAACL 2024, and can be accessed <a href="https://aclanthology.org/2024.bea-1.49/"> here</a>

