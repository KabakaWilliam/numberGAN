# numberGAN
First implementation of a GAN architecture to generate new numbers from the MNIST dataset


<h3> Here's a gif of the numbers created by the GAN </h3>


![numbers-min](https://user-images.githubusercontent.com/73100027/124642171-332e4e00-de98-11eb-9727-6df6ae3aca38.gif)



The numbers are fairly visible at the moment. With more training, I will be able to get more realistic looking numbers generated.


If you want to test the output of the trained GAN call the generator below and it will produce a random number

        noise = tf.random.normal([1, 100])
        generated_image = generator(noise, training=False)
        plt.imshow(generated_image[0, :, :, 0], cmap='gray')
