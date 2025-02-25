# 🤖 **EDUBOT Robotics Kit**

![Python](https://img.shields.io/badge/python-3.12-blue)
![Raspberry Pi](https://img.shields.io/badge/pi-compatible-red)
![License: MIT](https://img.shields.io/badge/license-MIT-green)

> **Educational robotics platform for classrooms.**

---

### About

EDUBOT is a teaching kit for middle-school robotics using Python.
Simulates wheels, sensors, and actuators on low-cost hardware or browser emulator.

**Website:** [edubotproject.io](https://edubotproject.io)
**Docs:** [docs.edubotproject.io](https://docs.edubotproject.io)

---

###  Concept

Each "bot" is a YAML config + Python behavior:

```yaml
bot:
  name: explorer
  sensors: [ultrasonic, gyro]
  actuators: [motor, servo]
```

```python
def loop(bot):
    if bot.distance() < 10:
        bot.turn(90)
    else:
        bot.forward(1)
```

---

###  Try in browser

```
python3 -m edubot.sim --map=basic
```

then open → `http://localhost:8080`

---

###  Components

* Cross-platform simulator (Pi, Linux, Web)
* Sensor emulation plugins
* Replay with camera overlay
* Curriculum JSON export

---

###  Roadmap

* [x] Web UI
* [ ] Visual programming
* [ ] Cloud sync

MIT License © [edubotproject.io](https://edubotproject.io)
