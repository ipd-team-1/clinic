# IPD Engineering Clinic

In this clinic, you'll play with the foundations of programming to do interesting things with our Raspberry Pi.

The following are hints and power-ups you'll be using in building this Raspberry Pi LED component.

### Imports

These are libraries we may need.

```python
import RPi.GPIO as GPIO
import time
```

- `GPIO` stands for general-purpose input out. Basically, there are just pins that gets turned on or off.
- `time` is a standard library that provides time and clock abilities, like sleep!

### Setup

```python
GPIO.setmode(GPIO.BCM)
GPIO.setwarnings(False)
GPIO.setup(18, GPIO.OUT)
```

These are some commands we need to run to set up our GPIOs. I didn't dive deep into knowing what they mean, but I can guess that:

- Warnings are suppressed.
- We are using port 18 to output (power our LED).

### Turning the LED on and off

```python
GPIO.output(18, GPIO.HIGH) # On.
GPIO.output(18, GPIO.LOW)  # Off.
```

### Sleeping

You can use `time`'s `sleep` to delay the code.

```python
time.sleep(1) # Let's sleep for 1 second.
```

### Conditionals

Conditionals allow you to make decisions in code.

```python
if (a == b):
  # Do something.
else:
  # Do something else.
```

### Loops

Loops lets you do things over and over again.

```python
while True:
  # Do something ... forever.

for x in range(5):
  # Do something 5 times.
  print x # You can even use that variable!
```

### Functions

Functions allow you to package chunks of code into small bits, which you can reuse! Less copy-pasting, better testing, and much easier to understand.

```python
def pet(cat):
  print cat + " is petted!"
```
