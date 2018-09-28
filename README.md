# Neural_Relation_Extraction

In this project, we have analysed two of the most prominent neural models, PCNN and Bi-GRU with word attention, that have been shown to be very effective for the of Relation Extraction. In literature, both the models have been separately used the task and combined as an ensemble. A key observation we found during the course of project is that PCNN being a window based method effectively captures representation of each word in a local context whereas Bi-GRU with captures the global representation of the word in the context of the entire sentence. Hence both having complementary properties. While PCNN captures syntax aware word representations from local windows, the global representation from Bi-GRU are more semantic in nature. In this project we have experimented with novel ways to combine these two models in an attempt to explore the effectiveness of the above interpretation. 

#
How to Run the Code Files::
Extract the vec.txt.tar.gz and copy the vec.txt(extracted file obtained ) in the directory where all codes are present.Now any model's .py file can be run independently.
#
PCNN.py is the implementation of the piecewise CNN model which will  output the F1-score on test data with epochs while training.
BiGRU_with_attention.py is the implementation of Bidirectional gated Recurrent unit with word level attention based relation classification.It will also output the F1-Score on test data with epochs.
The rest of the .py files are the novel combinations of both these models and will produce the F1-Score on the test data with epochs while training.
NRE_report.pdf is the report file containing all the work done for this project.
