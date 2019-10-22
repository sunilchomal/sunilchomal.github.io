# **Repositories**

## 1. pixel-cnn++ (enhanced)

repo: [pixel-cnn++ (enhanced)](https://sunilchomal.github.io/pixel-cnn/)

The changes added to the PixelCNN++ model are inspired by understanding the image, its properties & the field of computer vision in general. For example, adding a Non-Local NN block in the network, is like pre-processing the image using the a classical filtering *non-local means* algorithms, capturing long range dependences in images. Convolution gives *translation invariance", but at a cost. It losses *positional context*. Adding the "Coordinates Channels" to the image, before using it as the input to a network, gives the network the ability to learn the *translation dependence* in an image. This is similar to *optical flow* or dynamic image analysis in conventional techniques.

So literally, we are enabling our networks to see the *bigger picture* by enabling it to see long range dependencies & translation dependencies.

These techniques are applicable beyond generative models, and can be used to improve performances of image processing networks. These are like "low/mid level vision" tasks that supplement the semantic/high level vision tasks done by existing networks.

*tech: tensorflow, generative models, CoordConv, Non-Local Neural Networks, Focal Loss, google cloud, gpu*

## 2. Language Model (LM) for Grammar Error Correction (GEC), without the use of annotated data

repo: [GECwBERT](https://sunilchomal.github.io/GECwBERT/)

Grammatical errors are of many different types, including articles or determiners, prepositions, noun form, verb form, subject-verb agreement, pronouns, word choice, sentence structure, punctuation, capitalization, etc. Of all the error types, determiners and prepositions are among the most frequent errors made by learners of English. The focus of this project is to correct errors in spellings, determiners, prepositions & action verbs using BERT as a language representation model.

Bidirectional Encoder Representations from Transformers (BERT) is designed to pretrain deep bidirectional representations from unlabelled text by jointly conditioning on both left and right context in all layers. As a result, the pre-trained BERT model can be finetuned with just one additional output layer to create state-of-the-art models for a wide range of tasks, such as question answering and language inference, without substantial task specific architecture modifications.

We plan to use BERT for 2 tasks 

• Grammar Error Detection (GED) and 
• Grammar Error Correction (GEC)

Specifically, for task related to GEC, we plan to do it without the use of any annotated training, and just rely on the language knowledge captured by the BERT Masked Language Model (MLM).

*tech: python, pytorch, BERT, transformers, pytorch-transformers, language models, google colab, gpu*

## 3. Automatic Sensor Deployment tool for Surveillance Systems

repo: [Automatic Sensor Deployment tool for Surveillance Systems](https://sunilchomal.github.io/GISSitePlanner/)

These days, every establishment, may it be an office complex, a museum or a secure facility has a perimeter security system installed. Site Planner is an automated sensor deployment for surveillance systems. Surveillance systems require deployment of multitude of sensors across perimeters spanning 10's of kilometers. Each perimeter has its own unique geometry that would need unique sensor placement decisions. Sensor could be day camera, thermal or IR camera, Lidar, Radar or one of the many other options available these days. Each sensor would have its own coverage analysis methods & parameters. Visible sensors require Line of Sight calculations, and RF based sensors require Radio Line of Sight calculations. Site Planner tools allows surveillance system designers to automate the process of optimal sensor placement to give gap free coverage using GIS maps and algorithms.

*tech: python, luigi, django, geo-django, docker, pipenv, aws*

## 4. Camera Motion Detection

repo: [Camera Motion Detection](https://sunilchomal.github.io/cam-pan-detect/)

A moving camera creates image change due to its own motion, even if the 3D environ ment is unchanging. This motion has several uses. First, it may create more observations of the environment than available from a single viewpoint - this is the case when a panning camera is used to provide a wider (panoramic) view of the scene. Secondly, it can provide for computation of relative depth of objects since the images of close objects change faster than the images of remote objects. Third, it can provide for perception/measurement of the 3D shape of nearby objects - the multiple viewpoints allow for a triangulating computation similar to binocular stereo. In processing or analyzing video or film content, it is often important to detect points in time when the camera is panned or zoomed: in this case, we may not be interested in the contents of the scene but rather in the manner in which the scene was viewed.

*tech: python, openCV, optical flow*
