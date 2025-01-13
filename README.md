# MPCS 57200 1 Generative AI

## Spring 2025



# HW for Lec1

**Yiming Cheng**

**Cnet-id:12450588**

---

[toc]

## File Structure

```
Lec1_HW_YimingCheng_12450588
├── HW1-1
│   ├── gpt2_example.ipynb
│   ├── gpt2_example.pdf
│   ├── hello_gpt4o.ipynb
│   └── hello_gpt4o.ipynb - Colab.pdf
├── HW1-3
│   └── 2096.MP4
├── readme.md
└── readme.pdf
```

## HW1-1

<img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112175531556.png" alt="image-20250112175531556" style="zoom:150%;" />

### `gpt2_example.ipynb`

**Environment：**The environment files is in  `HW1-1/.venv`

**Output**: The answer to the original transformer prediction is 

The answer to the universe is not to be found in the ==**universe**==

![image-20250112182512299](/Users/eamin/Library/Application Support/typora-user-images/image-20250112182512299.png)

**Extra**:

1. On Apple Silicon (mine is M3 pro), PyTorch supports Metal Performance Shaders (MPS) as a device for accelerated computation. I use mps instead of cuda:
<img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112183244687.png" alt="image-20250112183244687" style="zoom:50%;" />

2. To explore the probability distribution provided by the transformer model and examine tokens other than “universe,” I modify the code to print the top-ranked tokens and their probabilities：

<img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112183559230.png" alt="image-20250112183559230" style="zoom:50%;" />

   and the result：

   <img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112183622474.png" alt="image-20250112183622474" style="zoom:50%;" />

   interesting

   3. To generate completions with varying lengths (e.g., 1 token, 5 tokens, 10 tokens, 20 tokens), I modify the code to  generate tokens chains：

   <img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112184447477.png" alt="image-20250112184447477" style="zoom:50%;" />

Result:

<img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112184514458.png" alt="image-20250112184514458" style="zoom:50%;" />

4. various queries and roles：

   <img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112184938924.png" alt="image-20250112184938924" style="zoom:50%;" />

   results：

   <img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112185001411.png" alt="image-20250112185001411" style="zoom:50%;" />

all result can be found in `HW1-1/gpt2_example.pdf`



### `hello_gpt4o.ipynb`

**Environment：**The environment files is in  `google colab`

**Output**: 

<img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112212154287.png" alt="image-20250112212154287" style="zoom:50%;" />

<img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112212216952.png" alt="image-20250112212216952" style="zoom:50%;" />

**Extra**:

I  create a unique story by assigning it the role of a “wildly imaginative storyteller blending mythology with science fiction.” The prompt asked for a tale where a modern scientist meets Zeus. I set the temperature to 0.8 to encourage creative and diverse responses, exploring AI’s storytelling potential.

![image-20250112213149385](/Users/eamin/Library/Application Support/typora-user-images/image-20250112213149385.png)



the complete result is in `HW1-1/hello_gpt4o.ipynb - Colab.pdf`





## HW1-2

<img src="/Users/eamin/Library/Application Support/typora-user-images/image-20250112175613401.png" alt="image-20250112175613401" style="zoom:150%;" />

1. **Generative AI**

ChatGPT uses the Transformer architecture to predict the probability distribution of the next token based on existing tokens (in this case,documents in different languages). It is a type of Generative Artificial Intelligence (Generative AI), making it a form of Generative AI.

2. **Statistics**

Documents in different languages exhibit certain probability distributions or statistical patterns based on compression rates. Encoding common patterns while identifying and compressing  files that compress badly, which are more likely to be non-English documents, is a statistical method.

3. **Machine Learning**

Random forests are used to analyze document  compression rates. By training on labeled datasets of English and non-English documents, they learn the characteristic patterns of English documents. Then, through the integration of multiple decision trees, they classify unlabeled documents and identify anomalies that significantly differ from English characteristics. Therefore, it is a machine learning method.

4.**Deep Learning**

It identifies unusual documents by learning the patterns of English and non-English documents during training. Its ability to find complex features and work with large amounts of data makes it a good choice for this type of anomaly detection, so it is considered deep learning.





## HW1-3

![image-20250112175911777](/Users/eamin/Library/Application Support/typora-user-images/image-20250112175911777.png)

![image-20250112231406989](/Users/eamin/Library/Application Support/typora-user-images/image-20250112231406989.png)

I explored two generative AI models. The first one is CLIP (Contrastive Language-Image Pretraining), a text-to-image model that converts raw images into textual descriptions. The second model is Stable Diffusion, which transforms text into images. For intermediate text states, if the user wants to add additional descriptions—such as transforming Charlie Chaplin into a cartoon character and changing the scene to an igloo—these models can achieve style transformation in the resulting images. The effects of the models are demonstrated in the video `HW1-3/2096.MP4`