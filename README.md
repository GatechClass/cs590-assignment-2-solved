# cs590-assignment-2-solved
**TO GET THIS SOLUTION VISIT:** [CS590 Assignment 2 Solved](https://mantutor.com/product/cs590-assignment-2-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;115160&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS590 Assignment 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Please read the instructions carefully.

Program-1 [25 points]

Use the alexnet program and modify it to the conditions given below. Use the database MNIST already present in the pytorch. Instead of FashionMNIST it will be MNIST. Number of Classes in this dataset is 10. MNIST is a dataset to identify numbers, so the number of classes is 10. Make the batch size 16 and epoch should be 1 or 2.

Layer1:

1. Input will be 1 channel i.e grayscale images

2. Apply 96 kernels, of kernel size 11, stride of 4 and padding of 0

3. Apply activation function ReLU Layer2:

1. Apply 96 kernels, kernel size 1

2. Apply activation function ReLU Layer3:

1. Apply 96 kernel, kernel size 1

2. Apply activation function ReLU

3. Do a maxpool2d, kernel size of 3 and stride2

4. Dropout of 0.5 Layer4:

1. Apply 256 kernel (hint the input to this conv2d layer is still 96) of size 11, stride 4 and padding 2

2. Apply activation function ReLU Layer5:

1. Apply 256 kernels, kernel size of 1

2. Apply activation function ReLU Layer5:

1. Apply 256 kernels, kernel size of 1

2. Apply activation function ReLU

3. Maxpool2d, kernel size of 3 and stride of 2.

4. Dropout of 0.5 Layer6:

1. Apply 384 kernels of size 3, stride of 1 and padding of 1

2. Apply activation function ReLU Layer7:

1. Apply 384 kernels of size 1

2. Apply activation function ReLU Layer 8:

1. Apply 384 kernels of size 1

2. Apply activation function ReLU

3. Dropout of 0.5

Layer 9

1. Apply 10 kernel (hint the input to this layer is 384) of kernel size 3, stride of 1 and padding of 1

2. Apply activation function ReLU Layer 10:

1. Apply 10 kernels of kernel size 1

2. Apply activation function ReLU Layer 11:

1. Apply 10 kernels of kernel size 1

2. Apply activation function ReLU

3. Finally apply nn.AdaptiveAvgPool2d((1, 1)) to the final output.

There is no fully connected layer in this network; it is in the alexnet code that I have given. Modify the alexnet code appropriately.

Program-2: [25 points]

Use the database MNIST already present in the pytorch. Instead of FashionMNIST it will be MNIST. Number of Classes in this dataset is 10. MNIST is a dataset to identify numbers, so the number of classes is 10. Make the batch size 16 and epoch should be 1 or 2.

Use the program you created for program-1 and layers-1 to layer-8 will be the same. Delete the layers-9 to 11. Instead plug in a fully connected (fc) layer (i.e. nn.Linear()).

Remember now you are using the fc layer so please go back and understand the fc layer of alexnet. You have to flatten the data. Look carefully at the transform function, it is transforming the images into 224×224 images. MNIST data are usually 28×28. The transformation is scaling the data. So the input data will be 224×224 and grayscale (i.e. one input channel)

The conditions are:

A. In case of alexnet the input was 5*5*256, in this case the input will be X * Y * 384. Look at the output channel size of the last layer (i.e. previous to this layer). Calculate X and Y yourself. Remember the input image is of size 224×224 in the layer-1 because of transformation. Take help from the alexnet code and slide-8 of

“introduction to Neural Network-II”. Important: In pytorch for output size determination they use the floor function.

Layer-9:

1. Input channel to fc (or nn.Linear) will be X * Y * 384 and output will be 4096

2. Apply activation function ReLU

3. Dropout of 0.5 Layer-10:

1. Input channel to fc (or nn.Linear) will be 4096 and output will be 4096

2. Apply activation function ReLU

3. Dropout of 0.5

Layer-11:(actually this is not a layer but anyways)

1. Input channel to fc (or nn.Linear) will be 4096 and output will be Classes (number of classes)

BONUS QUESTION: [15 Points]

If you are able to draw the diagram of the network given in either program-1 or program-2 in the manner shown in slide number 8 of “introduction to Neural Network-II” slide deck. Upload the image into github.

ZIP THE NOTEBOOK FILES AND SUBMIT IT TO MOODLE TOO FOR RECORD

IF YOU HAVE ANY QUESTION ASK ME AFTER THE CLASS OR DURING THE CLASS, I AM HAPPY TO EXPLAIN.
