### Transformers using TensorFlow 2

* [GitHub Repo with TensorFlow official Transformer Implementation](https://github.com/tensorflow/models/tree/master/official/nlp/transformer)
* [Paper: Attention Is All You Need](https://arxiv.org/abs/1706.03762)

### Key Transformer Model Components in Python
* [transformer.py](parts-of-a-transformer/transformer.py): Defines a tf.keras.Model: `Transformer`.
* [embedding_layer.py](parts-of-a-transformer/embedding_layer.py): Contains the layer that calculates the embeddings. The embedding weights are also used to calculate the pre-softmax probabilities from the decoder output.
* [attention_layer.py](parts-of-a-transformer/attention_layer.py): Defines the multi-headed and self attention layers that are used in the encoder/decoder stacks.
  * ![Attention in machine translation]((images/attention_sentence.png)) 
  * You can see how the model paid attention correctly when outputing European Economic Area. In French, the order of these words is reversed (européenne économique zone) as compared to English. Every other word in the sentence is in similar order.]
* [ffn_layer.py](parts-of-a-transformer/ffn_layer.py): Defines the feedforward network that is used in the encoder/decoder stacks. The network is composed of 2 fully connected layers.

### Hugging Face Transformer Examples

* [HuggingFace Website](https://huggingface.co/)
* [Write with Transformers](https://transformer.huggingface.co/)
* [Masked word completion with BERT](https://huggingface.co/bert-base-uncased?text=Paris+is+the+%5BMASK%5D+of+France)
* [Text generation with GPT-2](https://huggingface.co/gpt2?text=A+long+time+ago%2C+)
* [Natural Language Inference with RoBERTa](https://huggingface.co/roberta-large-mnli?text=The+dog+was+lost.+Nobody+lost+any+animal)
* [Question answering with DistilBERT](https://huggingface.co/distilbert-base-uncased-distilled-squad?text=Which+name+is+also+used+to+describe+the+Amazon+rainforest+in+English%3F&context=The+Amazon+rainforest+%28Portuguese%3A+Floresta+Amaz%C3%B4nica+or+Amaz%C3%B4nia%3B+Spanish%3A+Selva+Amaz%C3%B3nica%2C+Amazon%C3%ADa+or+usually+Amazonia%3B+French%3A+For%C3%AAt+amazonienne%3B+Dutch%3A+Amazoneregenwoud%29%2C+also+known+in+English+as+Amazonia+or+the+Amazon+Jungle%2C+is+a+moist+broadleaf+forest+that+covers+most+of+the+Amazon+basin+of+South+America.+This+basin+encompasses+7%2C000%2C000+square+kilometres+%282%2C700%2C000+sq+mi%29%2C+of+which+5%2C500%2C000+square+kilometres+%282%2C100%2C000+sq+mi%29+are+covered+by+the+rainforest.+This+region+includes+territory+belonging+to+nine+nations.+The+majority+of+the+forest+is+contained+within+Brazil%2C+with+60%25+of+the+rainforest%2C+followed+by+Peru+with+13%25%2C+Colombia+with+10%25%2C+and+with+minor+amounts+in+Venezuela%2C+Ecuador%2C+Bolivia%2C+Guyana%2C+Suriname+and+French+Guiana.+States+or+departments+in+four+nations+contain+%22Amazonas%22+in+their+names.+The+Amazon+represents+over+half+of+the+planet%27s+remaining+rainforests%2C+and+comprises+the+largest+and+most+biodiverse+tract+of+tropical+rainforest+in+the+world%2C+with+an+estimated+390+billion+individual+trees+divided+into+16%2C000+species)

### Resources
* [Google AI Blog on Transformer Architecture](https://ai.googleblog.com/2017/08/transformer-novel-neural-network.html)
* [Illustrated Self-Attention](https://towardsdatascience.com/illustrated-self-attention-2d627e33b20a)
* [self-attention-mechanisms-in-natural-language-processing](https://www.alibabacloud.com/blog/self-attention-mechanisms-in-natural-language-processing_593968)
* [Transformer Neural Nets - Wolfram Explanation](https://www.wolfram.com/language/12/neural-network-framework/use-transformer-neural-nets.html?product=mathematica)
* [Self Attention in NLP](https://www.geeksforgeeks.org/self-attention-in-nlp/)
* [The Annotated Transformer (in PyTorch)](http://nlp.seas.harvard.edu/2018/04/03/attention.html)
* [What does einsum do?](https://www.tensorflow.org/api_docs/python/tf/einsum)
