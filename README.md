# DNN-Personification project 

![Training StyleGAN](https://github.com/Shivani29sheth/DNN-Personification/blob/master/GAN%20Local%20Editing%20Reproduce/ezgif.com-gif-maker%20(15).gif)

This above GIF representing the training ouputs that were produced when StyleGAN model was trained on the celebrity HQ dataset on GoogleCOLAB. The training time was nearly 3 days with possible interruptions and reloading of the saved models. The snapshot of evaluated model has been included below. This training was done on GoogleCOLAB Pro version, by using Tesla P100-PCIE-16GB GPU, with 25.51 GB of usable RAM and 147.15 GB of usable Memory.
![GPU](https://github.com/Shivani29sheth/DNN-Personification/blob/master/GAN%20Local%20Editing%20Reproduce/gpu.png)
\
The specifications of the resource used are above.
\
\
The training of the StyleGAN model was done in batches where 6 batches of roughly 12 hrs training was divided and the training was resumed from the point the previous batch left. This led in using the StyleGAN model for our Local GAN editing project. The snapshot of the training example is attached below.
![Training PIC](https://github.com/Shivani29sheth/DNN-Personification/blob/master/GAN%20Local%20Editing%20Reproduce/1122.png)

# GAN Local Editing Reproduce

Using the knowledge from the paper, some part of the author's code, we are able to generate the following results for our project:

![Reproduce](https://github.com/Shivani29sheth/DNN-Personification/blob/master/GAN%20Local%20Editing%20Reproduce/GAN1.png)

Here we see how the specific features of the face can be swapped and local editing is possible, as claimed bby the paper.

# GAN Local Editing Extend Goal

Using the knowledge of Local Editing, we apply that to all features in order to obtain a full facial feature transfer. Applying this to all local features on face one by one gives us the following result :

![Extended Paper1](https://github.com/Shivani29sheth/DNN-Personification/blob/master/GAN%20Local%20Editing%20Reproduce/GAN2.png)

We can see above, how the entire facial features are transferred at the end of ths image. The face of the female at the end has the entire facial features derived from the male face and similar with the female face. This is the goal we wanted to extend in our project.

Now let us look on the second paper imeplementation ad the extension of the paper

# StarGAN v2

StarGAN v2 is the type of Adverserial Network that generates high quality images for faces and animla datasets. This enables feature transformation of faces from source to the target. The model was trained from scratch and generated checkpoints were saved and loaded to get the results. The training took 3 days and using Google Colab PRO, we were able to generate this. As and when the training got interrupted, we saved the model and the loaded in the new notebook session. We had to do so about 6-7 times as notebook got disconnected nearly after 12 hours of training. The generated output is listed below:

![StarGAN_v2_Output](https://github.com/Shivani29sheth/DNN-Personification/blob/master/StarGAN%20v2%20Reproduce/metrics/generated%20image.jpg)

We used our teammates faces and swapped them with famous celebs like : Angelina Jolie, Gal Gadot and Jason Momoa and got the above tremendous results.

The generation of the images can be seen by looking at the transformations our faces went through.

![Generation_StarGAN_v2](https://github.com/Shivani29sheth/DNN-Personification/blob/master/StarGAN%20v2%20Reproduce/metrics/ref_vid.gif)

# StarGAN v2 Extended Goal

We extended this paper implementation to videos and we get the following output.

![Video StarGAN V2](https://github.com/Shivani29sheth/DNN-Personification/blob/master/StarGAN%20v2%20Reproduce/metrics/TonyStark.gif)

This is pretty amazing and unexpectedely stunning result we got.
We converted video to GIF, extracted frames from GIF, used them as images, then applied StarGAN v2, combined them into frames for GIF, made GIF, adjusted speed, converted GIF to video and got amazing results. The results with sound can be seen in the YouTube link.

The implementation and presentation can be seen on YouTube. 
https://www.youtube.com/watch?v=1-WYZ4UKD1Q&t=54s

