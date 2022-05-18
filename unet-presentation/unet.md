---
marp: false
theme: gaia
---

# Segmentation Task

How do we get to this?
![](segmentation.png)

---

# Problem Description

Similar to image classification.

Instead of classifying the class of the image - classfiy every pixel.

Image | Mask 
:-:|:-:
![left](image.png)|![right](label.png)

---

# General Idea

Encoder - Decoder architecture

Compress image to dense representation [Encoder]

Decode image from dense representation [Decoder]

![](encoder-decoder.png)

Why? Receptive Fields in the dense representation is (nearly) global.

---

# Spatial information

![bg right](sad-dog.png)

We loose spatial (positional) information

If I tell you there is a dog in a image, can you tell me where it is?

No.

--- 

![bg width:1050px](unet-architecture.png)

---


# Huh..

https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html
