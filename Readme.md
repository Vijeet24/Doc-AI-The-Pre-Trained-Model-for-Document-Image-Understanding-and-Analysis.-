<h1><b>LayoutLMV1</b></h1>

Pre-training techniques have been verified successfully in a variety of NLP tasks in recent years. Despite the widespread use of pretraining models for NLP  
applications, they almost exclusively focus on text-level manipulation,while neglecting layout and style information that is vital for document image understanding.
The LayoutLM jointly model interactions between text and layout information across scanned document images, which is beneficial for a great number of realworld 
document image understanding tasks such as information extraction from scanned documents. Furthermore, we also leverage image features to incorporate words’ visual 
information into LayoutLM. LayoutLM makes it possible for model to learn text and layout are jointly in a single framework for document level pre-training. We will 
also try to fine-tune these models on task-specific data, as in Scaling Instruction-Finetuned Language Models, and try to improve their performance even further.




•	In this project, we replicated the results of the LayoutLM, getting the accuracy of 0.92 on the FUNSD dataset.
•	We try to pretrain an RCNN model with a ResNet101 as it's backbone and they uses this backbone to generate feature maps, which are documents' embeddings.
•	This feature map from documents is used in addition to LayoutLM Transformer to classify tokens and extract fields from the document.
•	We can use LayoutLM Version 1 with image embeddings from documents' feature maps to improve performance.         


The project was inspired from the paper https://arxiv.org/abs/1912.13318.
