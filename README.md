# Jukebox_basedon_emotionrecognition

Topic: Interactive jukebox  based on the emotion recognition with facial expression.

Resources are as follows:
1.Python-version 3.0 and above.
2. Scripting language-JavaScript.
3. Framework-Django
4.Dtabase- SQLite
5.Operating System : Windows 10
6. Memory and Ram: 1tb and 8gb respectively
7. Languages Used: Python, HTML, CSS and JavaScript
8. IDE: PyCharm


REGARDING THE DATA SET 
The data consists of 48x48 pixel grayscale images of faces. The faces have been automatically registered so that the face is more or less centered and occupies about the same amount of space in each image. The task is to categorize each face based on the emotion shown in the facial expression into one of seven categories (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral).
Train.csv contains two columns, "emotion" and "pixels". The "emotion" column contains a numeric code ranging from 0 to 6, inclusive, for the emotion that is present in the image. The "pixels" column contains a string surrounded in quotes for each image. The contents of this string are space-separated pixel values in row-major order. Test.csv contains only the "pixels" column and your task is to predict the emotion column.
The training set consists of 28,709 examples. The public test set used for the leaderboard consists of 3,589 examples. The final test set, which was used to determine the winner of the competition, consists of other 3,589 examples.
This dataset was prepared by Pierre-Luc Carrier and Aaron Courville, as part of an ongoing research project. They have graciously provided the workshop organizers with a preliminary version of their dataset to use for this contest.
DATASET: https://www.kaggle.com/jonathanoheix/face-expression-recognition-dataset.

Data Analysis
Data Analysis is the process of analysing the data. Here the data set is of two sets that are train data set and test data set. The training data set is that data set based on which this problem is prepared. Test data is defined as a set of observations utilized for evaluating the performance of the system by the help of some performance metric. The performance metric is essential as it does not include the training set in the test data set.
The trainning of the netwirk is done through the bottle neck problem.The bottleneck is a layer of fewer neurons below or above the neural network. With this layer, the network supports function representations to match better in the space available such that the better loss is obtained during training.Bottleneck layers (for example Google's Promotional Network) are applied to the CNN to reduce the amount of features (such as "channels") on the network. This can be accomplished by means of 1x1 turns and less output channels.Normally, don't measure weights explicitly for bottleneck levels, as with all other weights, the preparation phase is involved. You have to divide and innovate to pick a suitable size for a congestion layer in order to identify the network Architectures that perform well. The goal here is generally to find a network that produces new images and bottleneck capacities by reducing the amount of network parameters while staying profound and representing several maps of features. The below graphs obtained is a histogram graphs. Histogram graph is a tool for accessing the probability distribution quickly.
The logs will be created and this need a virtual envirnoment. The project is implemented using the Django,HTML,CSS,JavaScript in Pycharm.







How to run a project.
1.Install all the libary files from the requirement.txt
2.Go to training folder 
3.python3 train.py \
  --bottleneck_dir=logs/bottlenecks \
  --how_many_training_steps=2000 \
  --model_dir=inception \
  --summaries_dir=logs/training_summaries/basic \
  --output_graph=logs/trained_graph.pb \
  --output_labels=logs/trained_labels.txt \
  --image_dir=./dataset


"dataset" folder has all the images which is been downloaded from the kaggle dataset link.
DATASET: https://www.kaggle.com/jonathanoheix/face-expression-recognition-dataset.

The training summary,inception model will genertaed through the train.py.

4.Training log folder obtained should be copy and pasted in the emotion app folder logs.
That is Copy training\logs(files and folders which are obtained while running the train.py) paste in emotion_recognition_musicplayerusing_Django\emotion_app\emotion_app\logs

5. To Run the foolowing commands 
  1.Tensorboard == >tensorboard --logdir= " "
  2.Run in terminal == > Got to the folder name using django E:\emotion_recognition_musicplayerusing_Django\python manage.py migrate 
                                                             E:\emotion_recognition_musicplayerusing_Django\python manage.py migration 
  3.Run python==> E:\emotion_recognition_musicplayerusing_Django\manage.py
  4.The link obtained with local host,open it in the browser.(http://127.0.0.1:8000/) to start the server.
  
                                                             
                                                             
                                                             
                                                             
                                                             

