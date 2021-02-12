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
1. A relevant real-world problem is effectively mandating face masks during the pandemic. Especially in the U.S, we’ve found that it’s been a struggle in properly enforcing mask-wearing behavior––a situation that comes with many repercussions.  I found a dataset on Kaggle (https://www.kaggle.com/andrewmvd/face-mask-detection)  that has three classes of images: people wearing masks, people without masks, and people with masks worn incorrectly. With this dataset, we could develop a model that detects whether someone is taking the proper precautions against COVID-19. This can be particularly useful in public locations, where this mask detection model can spot those who lack the appropriate protection and are potentially riskings others.  
I’m not sure what specific deep learning algorithm to develop a model, but I believe this would fall under supervised learning, since the computer learns to detect mask-wearing through images that already represent the classes we’re trying to isolate. 

