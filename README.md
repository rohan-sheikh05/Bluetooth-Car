# Arduino nano → L298N Motor Driver
# Left motors
Arduino D2  -> L298N IN1
Arduino D4  -> L298N IN2
Arduino D5  -> L298N ENA   # PWM speed control

# Right motors
Arduino D6  -> L298N IN3
Arduino D7  -> L298N IN4
Arduino D10  -> L298N ENB   # PWM speed control

# Power connections
Battery +12V -> L298N VCC (12V input)
Battery GND  -> L298N GND
Arduino GND  -> L298N GND (common ground)
Arduino Vin  -> L298N 5V

# Motors
L298N OUT1 -> Left Motor 1 (+)
L298N OUT2 -> Left Motor 1 (–)
L298N OUT3 -> Right Motor 1 (+)
L298N OUT4 -> Right Motor 1 (–)

# Bluetooth HC-05 Module
Arduino D0 (RX) <- HC-05 TX
Arduino D1 (TX) -> HC-05 RX (via voltage divider to 3.3V)
Arduino 5V      -> HC-05 VCC
Arduino GND     -> HC-05 GND
