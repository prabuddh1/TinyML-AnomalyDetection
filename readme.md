# TinyML (Tiny Machine Learning) Keyword Spotting Application

This TinyML Model uses Speech Commands dataset to train & detect keywords: ON, OFF, STOP, GO.
Also, classifies as 'silence' or 'unknown' on the basis of the data being 'inaudible' or 'unknown keywords other than ON, OFF, STOP, GO' respectively.

### Training & Inference

> Model is trained using Tensorflow, and then Optimized & Converted into Quantized TFLite (Tensorflow Lite) model to run on mobile devices.