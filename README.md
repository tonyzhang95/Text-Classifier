# CNN Text Classifier for Chinese Corpus: News

I trained this CNN text classifier on Chinese news during my internship with Alibaba Cloud, and achieved 99% accuracy on test sets.

The sources news text are collected from internal APIs and are labeled with their corresponding category. The deep learning architecture used in this project is CNN. We also tried RNN with LSTM, but the results are worse and training takes more time. We believe the reason for CNN to work for this task is that the news are inherently focused on one topic, short, and self-contained. The contextual significance is also reasonably constant throughout a single piece of news, unlike chat bots usually use RNN because newer conversations carry more weight than older conversations.

I used TensorFlow for the first implementation, achieved ~95%, and later switched to Keras, which is built on top of TensorFlow, to achieve ~99% accuracy.
