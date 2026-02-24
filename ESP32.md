# ESP32 Notes (Easy Version)

## 1. What is ESP32?

ESP32 is a small electronic board (microcontroller) used to build smart devices.

It works like a small computer.
It can:
- Take input
- Process data
- Control devices
- Connect to WiFi and Bluetooth

It is commonly used in IoT (Internet of Things) projects.

---

## 2. Why ESP32 is Popular?

- It has built-in WiFi
- It has built-in Bluetooth
- It is low cost
- It is fast
- It is small in size
- It uses less power

Because of these features, it is widely used in student projects.

---

## 3. Main Parts of ESP32

- GPIO Pins → Used to connect buttons, LEDs, sensors, etc.
- 3V3 Pin → Gives 3.3V power output
- GND → Ground connection
- VIN → Power input
- TX/RX → Used for communication
- EN → Reset button

---

## 4. Basic Specifications

- 32-bit processor
- Speed up to 240 MHz
- Built-in WiFi
- Built-in Bluetooth
- Works at 3.3V

---

## 5. What Can ESP32 Do?

- Control LEDs
- Read button input
- Connect to WiFi
- Send data to server
- Make simple web server
- Control motors
- Read sensor values

---

## 6. How to Program ESP32

ESP32 is usually programmed using:

- Arduino IDE

### Basic Steps:
1. Install Arduino IDE
2. Add ESP32 board in settings
3. Connect ESP32 using USB cable
4. Write code
5. Click Upload

---

## 7. Simple Example (Blink LED)

```cpp
void setup() {
  pinMode(2, OUTPUT);
}

void loop() {
  digitalWrite(2, HIGH);
  delay(1000);
  digitalWrite(2, LOW);
  delay(1000);
}
```

This code makes an LED blink every 1 second.

---

## 8. Applications of ESP32

- Smart home systems
- Digital classroom devices
- IoT projects
- Weather systems
- Automation systems
- Student engineering projects

---

## 9. Advantages

- Cheap
- Fast
- Built-in WiFi
- Easy to use
- Good for IoT

---

## 10. Limitations

- Works only on 3.3V
- Needs basic programming knowledge