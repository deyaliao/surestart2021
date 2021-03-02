# surestart2021
reflections  
2/8: I'm excited to join surestart to learn more about AI/ML! As these fields are relatively new, I think it's super valuable to understand how to use tech as a means of social change in today's technologically-dependent world. And, as an avid artist, I'm always looking for ways to learn how to creatively achieve my vision.   
2/9: 
1. Supervised vs unsupervised learning: for unsupervised, you let the computer find hidden patterns in a dataset, where new correlations can give you new insight about the data you have. For supervised, you feed data into the computer, which serves as a way to "train" the computer to make its own decisions in the future.   
2. Scikit learn is solely focused on data modeling; it has no involvement with the actual manipulation or visualization of data, so one should use scikit learn along with these other analysis libraries.  

2/10: Today, I read over 2 articles as an introduction to basic ML concepts and model development. I also built my first neural network using tensorflow.   
1. A tensor is a multidimensional array that mathematically depicts a physical entity. We can better understand what a tensor is through its relation to scalars and vectors: scalars is a simple quantity/magnitude, and vectors are scalars with direction. They both are used to represent a physical quantity; likewise, tensors are essentially an array of multiple vectors, allowing mathematically representing data up to N dimensions. In machine learning, data is often multi-dimensional (such as images), and tensors are a data structure that mathematically encodes the data in a way for the computer to understand. This is an integral part to developing neural network models.   
2. I noticed that running the computations returned an array, which was a mathematical representation of the image. As I worked through the tutorial, I understood that one had to study and manipulate the data first (rescale images, convert to greyscale) in order to even start feeding the data into our neural network.  

2/11:
1. A relevant real-world problem is effectively mandating face masks during the pandemic. Especially in the U.S, we’ve found that properly enforcing mask-wearing behavior has been a struggle, unfortunately exacerbating COVID's repercussions in our society.  I found a dataset on Kaggle (https://www.kaggle.com/andrewmvd/face-mask-detection)  that has three classes of images: people wearing masks, people without masks, and people with masks worn incorrectly. With this dataset, we could develop a model that detects whether someone is taking the proper precautions against COVID-19. This can be particularly useful in public locations, where this mask detection model can spot those who lack the appropriate protection and are potentially riskings others.  
I’m not sure what specific deep learning algorithm to develop a model, but I believe this would fall under supervised learning, since the computer learns to detect mask-wearing through images that already represent the classes we’re trying to isolate. 

2/16:
1. This game showed the unconscious bias we display while finding data, which can unintentionally create bias in the model we use. This is problematic becasue in supervised learning, the computer learns to make decisions based off of the pre-existing data. In the game, we saw how the computer perpetuates that bias/stereotype already present in our hiring patterns, which raises ethical concerns regarding if using a model is even reliable and/or fair. 
2. An example of a biased machine learning model is COMPAS (Correctional Offender Management Profiling for Alternative Sactions). I specifically selected this model because of its notoriety and large implications in the real world (it was responsible for many convictions in our justice system), and it serves as a clear reminder for why we should be cognizant + more transparent about the biases in our model before it further exacerbates the prejudice in our world. When creating models, we have to try and adjust for both racial and gender bias. To do this, while choosing to use this data, we should be aware of the factors used to train the model (in this case, risk factors that probably highlight the general societal ills / bias), be more transparent with how exactly this model calculates its data, and potentially expand our sample set to encompass both local/federal cases. 

2/17:
1. Convolutional Neural Network VS Fully Connected Neural Network: a CNN primarly works by taking a main image and reducing that to a smaller dimension through its many layers (convolutional, pooling / downsampling, and the fully connected layer). Specifically, the convolutional layer leverages the fact that each image is composed of pixels which can be further summarized into a feature map through a "convolution" operation. Then, the pooling layer (performing downsampling)  reduces the matrix dimensions of the original image, essentially summarizing the image in a more concise way. Once this process repeats, the data is then flattened into vectors, which means it can be finally be treated as a mathematical input key to the next couple of layers in the model. For a Fully Connected Neural Network, there is no prior data processing (such as downsampling) before the input an be used for backpropagation(?). Each neuron is connected to the neurons in the next layer, with each relationship having its own weight/bias.   

Regarding the differences in applications of these two architectures, a CNN is specialized for image recognition and classification (due to its efficiency in processing images with fewer weights), and a Fully Connected Neural Network is a broader architecture––being "structure agnostic"––that can be used for understanding data and finding patterns. 

2/23:
Using a Rectified Linear activation functions has many benefits. In essence, the function itself is relatively simple, as it's composed of a max() function. And, because it's a max function between 0 and the input, entering in any number will return either 0 or the value itself. This creates a linear output, not only making the model easier to optimize, but decreasing the risks for common issues such as vanishing gradients. Finally, the fact that entering in a negative number will return 0 is also helpful. This is called sparse representation, and it's desired by models as it can simplify the model. RELU is best used for CNN and MLP architectures; we actually used this activation function is some of our last action items (such as the CNN for classifying MNIST digits).  

2/25:
By changing the loss function to a regression based function (adding L2 regularization), the model accuracy went up a bit. Looking at the loss graph, there seems to be less overfitting: unlike before, the training data loss doesn't decrease more than the validation data.  

3/1: 
I attempted to complete Example 4, which was centered around using FastText to detect languages. I could not finish it due to needing to deploy through AWS, which was discussed with my mentors. Some ethical issues with NLP models is that these models are trained on human use of speech; this itself is problematic since humans often use negative, hateful speech. We are inherently flawed, and the model readily adapts to these negative qualities––learning how to replicate semantics and speech that we spew out of our mouths. Synthetic speech can be used for trolling and malicious intent, and this model only exacerbates that risk. 
