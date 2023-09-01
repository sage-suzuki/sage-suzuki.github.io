---
layout: project
type: project
image: img/keyboard/keyboard-pfp.jpeg
title: "Keyboard Assembling"
date: 2020-2022
published: true
labels:
  - Soldering
  - Circuits
  - Sales
summary: "Assembled and sold customized mechanical keyboards and parts."
---


During the spike of covid, I explored my entrepreneurial endeavor, I embarked on a captivating project centered around crafting and selling personalized keyboards tailored to the unique preferences of tech enthusiasts and keyboard aficionados. 

<div class="text-center p-4">
  <img width="440px" src="../img/keyboard/keyboard.png" class="img-thumbnail" >
</div>

### Processs
This venture involved an intricate process that spanned from conception to distribution. Sourcing top-tier components, I ensured the highest quality switches, keycaps, and cases to offer an unparalleled typing experience. The assemblage phase demanded precision soldering and meticulous attention to detail as each keyboard was meticulously brought to life.

### Reflection
My commitment to excellence extended to packaging and distribution, where careful handling guaranteed the keyboards reached their new owners in pristine condition. Through a harmonious fusion of technical expertise and creative customization, this project not only provided customers with a means of expression but also enabled me to immerse myself in the captivating realm of DIY electronics and entrepreneurship.

Here is some code that illustrates how we read values from the line sensors:

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
