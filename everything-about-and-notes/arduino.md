---
cover: >-
  https://images.unsplash.com/photo-1603732551658-5fabbafa84eb?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwxfHxhcmR1aW5vfGVufDB8fHx8MTY4ODAwOTgyOHww&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🦾 Arduino

## Introduction

If you are starting **programming** and want to give a try to **electronics**, **Arduino** is the perfect way in to get in. **Arduino is easy to program/learn**. Here will be some things to start with.

## &#x20;What is Arduino?

**Arduino** is an **open-source electronics platform** based on easy-to-use **hardware** and **software**.&#x20;

Arduino boards are able to read inputs - light on a sensor, a finger on a button, or a Twitter message - and turn it into an output - activating a motor, turning on an LED, publishing something online.&#x20;

You can tell your board what to do by sending a set of instructions to the microcontroller on the board. To do so you use the Arduino programming language (based on Wiring), and the Arduino Software (IDE), based on Processing.

### How to start with Arduino?

You will start downloading the **Arduino IDE** and **connecting** your **Arduino microcontroller** with it.

{% embed url="https://www.arduino.cc/en/software" %}

Follow the following steps:

1. Go to Tools >> Boards and select what board you are using.
2. Go to Tools >> Port and select the Arduino port.

Once you did this you have connected your Arduino, and you can start programming.

## Programming

Arduino was made with **c++,** and is a simplified language, if you have been experienced **c++, c or c#** programming you will learn this so much faster.

Here is the documentation:

{% embed url="https://www.arduino.cc/reference/en/" %}

### Your First Program : }

Let's start with the **built in led in the Arduino to demonstrate.**

```arduino
int dot = 1000; // integer variable

void setup(){

  pinMode(LED_BUILTIN, OUTPUT);

}

void loop(){


  digitalWrite(LED_BUILTIN, LOW);
  delay(dot);
  digitalWrite(LED_BUILTIN, HIGH);
  delay(dot);

}
```

#### Variables

* Variables are a defined storage of data that can be an **integer, decimal, characters, Booleans**. Imagine box that you put something like a phone or papers.

#### Functions

* Functions are basically **piece of code design/programmed to do instructions/actions in your program**. In this case the functions in this program are **setup()** and **loop()**.&#x20;
* We assign to the functions specific **parameters** that can be stored on a variable and pass to the function to make the specified actions.&#x20;
* **setup()** - this function is necessary to initialize and tell the Arduino what we are going to use.
* **loop()** - the loop function will repeat consecutively in the microcontroller.

#### digitalWrite()

Is a function of Arduino that lets you **turn on** or **turn off** a specific electronic component. In this case the led of the Arduino.

* **HIGH** - Means Turn **ON**
* **LOW** - Means Turn **OFF**

#### delay()

The **delay() func**, is to tell the microcontroller that we want to stop some time that can be 1, more or minus. In this case we are defining the delay in a **global variable** called **dot.**&#x20;

### Uploading

**Now how you upload this code to the Arduino?** In the IDE there is a checker to check if you have an error in your code before you uploaded. You check your code first, after that click the arrow to upload the code.

#### Input and Output

In this case we are using the led to output information to it, we are sending them instructions.&#x20;

* In case we define Input, we are receiving information threw a component and using that info to further use.

<figure><img src="https://email1akash.files.wordpress.com/2021/05/screenshot-from-2021-05-16-16-11-13.png?w=768" alt=""><figcaption></figcaption></figure>

&#x20;**Great !! Now look at your Arduino board.**

## Projects

Here you will find some of my projects that I do with the Arduino that you can use to build a more difficult circuits or improve your programming knowledge.

{% embed url="https://github.com/j4ckris1337/Arduino_Projects" %}

