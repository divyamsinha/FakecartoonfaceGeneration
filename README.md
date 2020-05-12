This project is about learning the faces of cartoons(Google cartoon 10k) and generating similar images from it.
It involves the use of DCGANs technique .
A Generator is used to generate fake images
A Discriminator is used to classify between real and fake images . Both generator and discriminator are trained simultaneously.
Training Discriminator involves feeding both real cartoon face and fake image from generator(initially noise) to discriminator and training it.
Training Generator involves freezing weights of Discriminator and connecting Generator to Discriminator. The output is fixed as real image(more loss can back propagate hence improving the accuracy).
So, after training we can generate fake images from noise .
