# FLARE
A validation of optical priors and a dataset of flares in nighttime road scenes.



## 1. Abstract

Inspired by Dai et al., we found that mobile phone cameras leave reflective flares in the image when capturing strong light. Due to the reflection of internal components in the camera, these flares are usually unavoidable. Flares can affect the quality of images, and the same applies in the field of traffic monitoring. If these flares happen to be in the head position of the motorcycle driver, they will inevitably affect the accuracy of the monitoring task.

We conducted further verification using three brands of mobile phones (iPhone 14 plus, Huawei honor 90 pro, Xiaomi 14 pro), Nikon camera (Nikon Z9), and electric alarm camera (9361-S).

The headlights of motorcycles usually do not affect the detection task of helmets, as the driver's head and headlights usually do not overlap. Most electric police cameras shoot from a top-down perspective, and the reflected flares of the car lights are likely to be right on the driver's head. These flares will seriously affect image quality, thereby affecting the accuracy of detection tasks. For this purpose, we specifically collected some image data of reflection flares in nighttime roads.

## 2. Update logs

**We are gradually opening up.**

1. We uploaded the validation of the optical center prior (April 20, 2024).
2. 

## 3. Optical priors

~~~data
-Optical priors
	--image
		---x.png
		...
	--label
		---x.label
		...
	--Confirmation.png
	--Optical priors.png
~~~

In the `/Optical priors` folder, `/image` stores the images we collected using five different devices, and `/label` stores our annotation information for the light sources and flares in these images.

<img src="/Optical priors/Optical priors.png" alt="Optical priors" style="zoom: 33%;" />

As shown in the above figure, xl and yl represent the coordinates of the light source, while xf and yf represent the coordinates of the flare, which are always symmetrical about the center of the lens.

<img src="/Optical priors/Confirmation.png" alt="Confirmation" style="zoom:50%;" />

As shown in the above figure, we have presented the annotated data in the figure, further verifying the rationality of optical priors. Due to manual annotation, there may be slight errors in some coordinates.

## 4. Flares in nighttime road scenes

Coming...

## 5. Contact

If you have any questions or communication, please contact us:

- Zhiqiang Liu: 2023211273@student.cup.edu.cn

