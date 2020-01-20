# Real-time abstract art using a neural net (CPPN) in JavaScript with TensorFlow.js

<p float="left">
    <img src="https://raw.githubusercontent.com/ex-punctis/abstract-art-cppn/master/gif1.gif" hspace="20" >
    <img src="https://raw.githubusercontent.com/ex-punctis/abstract-art-cppn/master/gif2.gif" hspace="20" >
</p>

This is essentially a compositional pattern-producing network (CPPN) except it makes abstract patterns instead of meaningful shapes. Inputs: pixel coordinates, mouse/touch coordinates, cos(time). Output: RGB values. Activations: sin, cos, tanh, linear. Weights: random.

<img src="https://raw.githubusercontent.com/ex-punctis/abstract-art-cppn/master/architecture.png">
(Architecture diagram generated by http://alexlenail.me/NN-SVG/index.html)

[Detailed explanation and live demo in my blog](https://www.expunctis.com/2020/01/19/Abstract-art.html)

## Requirements

TensorFlow.js utilizes WebGL to make calculations faster. It can also use CPU only, but you'll get much better framerates on a GPU-equipped device.  

## Acknowledgements

The following two resources introduced me to abstract art generation with CPPNs. 

https://www.deeplearning.ai/ai-notes/optimization/. 

https://tehnokv.com/posts/visualizing-audio-with-cppns/

I "borrowed" the idea of using cos(time) to generate dynamic patterns, but implemented the CPPN in js from scratch on my own. The idea to use mouse/touch coordinates as additional inputs came from my friend, Igor Guzman. It was my idea to add selection of activation functions and amplitude sliders for additional interactivity.