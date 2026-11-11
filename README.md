# OpenCat — Open-Source Quadruped Robot Framework

> **On current-gen hardware (Bittle X, Nybble Q) or starting fresh?** This repo covers the legacy NyBoard platform. Head to [OpenCatESP32](https://github.com/PetoiCamp/OpenCatEsp32-Quadruped-Robot) for current hardware and active development.

🚀 **[Quaddle](https://www.kickstarter.com/projects/petoi/quaddle-open-source-desktop-robot-kit/?ref=8t25yj&utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-hero-banner) — Petoi's newest OpenCat-lineage quadruped — funded on Kickstarter in October 2026.** [Late pledge →](https://www.kickstarter.com/projects/petoi/quaddle-open-source-desktop-robot-kit/?ref=8t25yj&utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-hero-banner) (details below)

OpenCat is an open-source Arduino and Raspberry Pi-based framework for building and programming quadruped robots. Developed by [Petoi](https://www.petoi.com?utm_source=github&utm_medium=code&utm_campaign=github-opencat), the maker of futuristic programmable robotic pets, it's the framework behind two mini robot kits: the Bittle robot dog and the Nybble robot cat.

The framework handles the hard parts — gait coordination, servo control, IMU integration — so you can focus on what you're actually building on top of it.

![](https://github.com/PetoiCamp/NonCodeFiles/blob/master/gif/walk.gif?raw=true)

![](https://github.com/PetoiCamp/NonCodeFiles/blob/master/gif/run.gif?raw=true)


---

## Quaddle mini robot dog — funded on Kickstarter, October 2026
![](https://github.com/PetoiCamp/NonCodeFiles/blob/master/gif/quaddleCover.gif?raw=true)

[Quaddle](https://www.kickstarter.com/projects/petoi/quaddle-open-source-desktop-robot-kit/?ref=8t25yj&utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-quaddle-section) is Petoi's newest quadruped, **funded on Kickstarter on October 8, 2026 by 534 backers** — a mini desk robot built on the same OpenCat lineage as Bittle and Nybble.

- Full quadruped running on just **4 servos** instead of the usual 8–12, which forces genuinely different gait-design and leg-coordination solutions to still get all four legs walking, running, and balancing
- Position-feedback servos — readable, not just drivable — which is what makes **Puppet Mode** possible: hand-guide the legs and record a motion directly, no code required
- 3D-printable shells and mounts for customization
- Same open platform this repo already supports for gait research, reinforcement learning (RL), and sim2real work — a hands-on physical AI platform, not a toy version of the idea
- Try it in the [online simulator](https://www.petoi.com/pages/quaddle-robot-dog-simulator?utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-quaddle-simulator) before it ships

**Source code is not yet public.** It's an upgraded version of the OpenCat project. The ESP32-S3 code structure is similar to this repo and closer to [OpenCatESP32](https://github.com/PetoiCamp/OpenCatEsp32-Quadruped-Robot), which already powers thousands of Bittle X and Nybble Q robots in the field. We plan to open source it before Quaddle delivery.

- Watch this repo and [r/petoi](https://www.reddit.com/r/Petoi/) for the open-source announcement
- [Late pledge on Kickstarter](https://www.kickstarter.com/projects/petoi/quaddle-open-source-desktop-robot-kit/?ref=8t25yj&utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-notify-link) while rewards are available
- Check out the [Quaddle Hugging Face page](https://huggingface.co/petoi/quaddle)

---

## About the Project

Inspired by Boston Dynamics' Spot, [Dr. Rongzhong Li](https://www.linkedin.com/in/rongzhongli/) started OpenCat in his dorm at Wake Forest University in 2016. The goal was straightforward: make agile quadruped robots affordable and hackable enough for researchers, educators, and makers — not just well-funded labs.

Since then:
- **30,000+ robots shipped**, cumulative across all channels
- **60+ countries**
- **$1M+ raised** across two prior Kickstarter and Indiegogo campaigns
- **14 academic papers** cite the platform — see [Research Spotlight](https://www.petoi.com/pages/robotics-research-and-academic-applications?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- One of the most-starred open-source quadruped robot projects on GitHub

OpenCat is now deployed across two robot platforms and used in K-12 schools, university research labs, maker spaces, and independent projects worldwide.

### Current Hardware

- 🐶 [Bittle X — mini robot dog & AI robotics kit with voice control](https://www.petoi.com/products/petoi-robot-dog-bittle-x-voice-controlled?utm_source=github&utm_medium=code&utm_campaign=github-opencat) — current generation, BiBoard/ESP32
  - [Also available on Amazon](https://www.amazon.com/dp/B0FNT6TSVT?utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-amazon-buy-link)
  - [Try the simulator](https://www.petoi.com/pages/bittle-x-robot-dog-simulator?utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-bittle-x-simulator)
- 🐱 [Nybble Q — mini robot cat & AI robotics kit](https://www.petoi.com/products/petoi-nybble-q-robot-cat?utm_source=github&utm_medium=code&utm_campaign=github-opencat) — current generation

The original [Bittle](https://www.petoi.com/collections/robots/products/petoi-bittle-robot-dog?utm_source=github&utm_medium=code&utm_campaign=github-opencat) and [Nybble](https://www.petoi.com/collections/robots/products/petoi-nybble-robot-cat?utm_source=github&utm_medium=code&utm_campaign=github-opencat) mini robots (NyBoard/ATmega328P) are discontinued but still fully supported by this codebase. This repo is the right place for NyBoard users; for ESP32/BiBoard see [OpenCatESP32](https://github.com/PetoiCamp/OpenCatEsp32-Quadruped-Robot).

![](https://github.com/PetoiCamp/NonCodeFiles/blob/master/gif/slope.gif?raw=true)

---

## What the Framework Gives You

- **Multi-language:** C/C++, Python, block-based coding
- **Open hardware + software:** fork, modify, extend — no vendor lock-in
- **Arduino + Raspberry Pi native:** works with the tools you already use
- **Sensor integration:** cameras, touch, IMUs, ultrasonic, etc. — clip and go
- **Sim-to-real:** experiment reinforcement learning models on an affordable robot
- **ROS compatible:** SLAM, navigation, and perception pipelines documented by the community

Whether you're teaching **robotics programming** for the first time, building a weekend **hackathon** project, or running a graduate-level **embodied robotics** experiment, the platform scales.

---

## What the Community Has Built

Users have shipped real **robotics projects** across AI, Raspberry Pi, and research — a few highlights:

- [Autonomous movement & object detection](https://www.petoi.com/blogs/blog/reid-graves-robotics-ai-applications-with-bittle-robot-dog-raspberry-pi?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [Raspberry Pi robotics projects](https://www.petoi.com/blogs/blog/tagged/raspberry-pi?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [AI and computer vision applications](https://www.petoi.com/blogs/blog/tagged/showcase+ai?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [NVIDIA Isaac simulations and reinforcement learning](https://www.youtube.com/playlist?list=PLHMFXft_rV6MWNGyofDzRhpatxZuUZMdg)
- [Visual and LiDAR-based SLAM with ROS](https://www.youtube.com/watch?v=uXpQUIF_Jyk&list=PLHMFXft_rV6MWNGyofDzRhpatxZuUZMdg&index=6)
- [Imitation learning with Tiny ML models](https://www.learnwitharobot.com/p/imitation-learning-with-petoi-bittle)
- [IoT robot fleet management with AWS](https://www.petoi.com/blogs/blog/aws-iot-robot-fleet-demo-with-petoi-bittle?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [3D-printed accessories and custom builds](https://www.petoi.com/blogs/blog/petoi-bittle-bittle-x-robots-3d-printed-robot-accessories?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [DIY 3D-printed robot pets on OpenCat](https://www.petoi.com/pages/3d-printed-robot-dog-robot-cat?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [Research Spotlight](https://www.petoi.com/pages/robotics-research-and-academic-applications?utm_source=github&utm_medium=code&utm_campaign=github-opencat) — academic and research use cases

![](https://github.com/PetoiCamp/NonCodeFiles/blob/master/gif/stand.gif?raw=true)

![](https://github.com/PetoiCamp/NonCodeFiles/blob/master/gif/NybbleBalance.gif?raw=true)

---

## Hardware

This repo targets the **NyBoard** — a customized Arduino board based on ATmega328P. It coordinates up to 12 [high-performance servos](https://www.petoi.com/products/quadruped-robot-dog-bittle-servo-set?utm_source=github&utm_medium=code&utm_campaign=github-opencat) for walking, running, jumping, and backflipping.

Extend with:
- [Sensor pack](https://www.petoi.com/products/petoi-sensor-pack?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [Intelligent camera module](https://www.petoi.com/products/intelligent-camera-module?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- Raspberry Pi, Nvidia Jetson Nano, or other AI co-processors via wired/wireless connections

For ESP32/BiBoard (current-gen hardware), see [OpenCatESP32](https://github.com/PetoiCamp/OpenCatEsp32-Quadruped-Robot).

---

## Setup

Full documentation: [Petoi Doc Center](https://docs.petoi.com)
The following steps give you a brief walk-through, but may miss detailed tips and illustrative pictures. 

**1. Clone the repo**

Remove the `-main` (or branch name) suffix from the folder after downloading.

**2. Open `OpenCat.ino` — select your robot and board**

```cpp
#define BITTLE    // Petoi 9 DOF robot dog: 1x on head + 8x on leg
//#define NYBBLE  // Petoi 11 DOF robot cat: 2x on head + 1x on tail + 8x on leg

//#define NyBoard_V0_1
//#define NyBoard_V0_2
#define NyBoard_V1_0
//#define NyBoard_V1_1
```

**3. Enter configuration mode**

Comment out `#define MAIN_SKETCH`, upload, follow serial prompts.

```cpp
// #define MAIN_SKETCH
```

**4. (Optional) Auto-init**

`#define AUTO_INIT` skips prompts and auto-calibrates IMU — handy for repeated flashing.

**5. Upload**

Plug USB uploader into NyBoard, install driver if needed, hit upload (→) in Arduino IDE.

**6. Serial Monitor**

Set to **no line ending** and **115200 baud rate**.

**7. Reset joint offsets**

```
Reset joint offsets? (Y/n)
Y
```

**8. IMU calibration**

```
Calibrate the IMU? (Y/n):
Y
```

Place the robot flat on a table. 6 long beeps → reads sensor data → saves offsets → beeps when done. Close Serial Monitor when `Ready!` appears.

**9. Switch to main sketch**

```cpp
#define MAIN_SKETCH
```

Uncomment and re-upload.

**10. Joint calibration**

Boot with one side up to enter calibration mode, or calibrate directly via Serial Monitor.

**11. Optional: Petoi app**

Plug in Bluetooth dongle for a friendlier calibration UI:
- iOS: [App Store](https://apps.apple.com/us/app/petoi/id1581548095)
- Android: [Google Play](https://play.google.com/store/apps/details?id=com.petoi.petoiapp)

See the [calibration guide](https://bittle.petoi.com/6-calibration) and [app guide](https://docs.petoi.com/app-guide).

**12. Start building**

Infrared remote, Petoi app, Python, or Serial Monitor. [Full play guide →](https://bittle.petoi.com/7-play-with-bittle)

---

## Education

OpenCat shows up in **AI robotics education** across K-12 programs, community colleges, university labs, and maker spaces — hands-on **physical AI** teaching that goes beyond screen-based coding exercises:

- [Robotics education showcases](https://www.petoi.com/blogs/blog/tagged/showcase+education?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [STEM & robotics curriculum resources](https://www.petoi.com/pages/resources-curriculum-stem-coding-robot?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [Robotics competitions](https://www.petoi.com/blogs/blog/robot-competitions-with-petoi?utm_source=github&utm_medium=code&utm_campaign=github-opencat)

---

## Community & Discussion

- [r/OpenCat](https://www.reddit.com/r/OpenCat/) — firmware code, framework hacking, extending and porting OpenCat
- [r/Petoi](https://www.reddit.com/r/Petoi/) — hardware Q&A, builds, quadruped coding, RL experiments, curriculum, 3D-printed parts, general discussion
- [Facebook Group](https://www.facebook.com/groups/385050523510952) — community discussion and builds

---

## Resources

- [Advanced tutorials by the community](https://www.youtube.com/playlist?list=PLHMFXft_rV6MWNGyofDzRhpatxZuUZMdg)
- [GitLab embedded DevOps workshop with Bittle X](https://www.petoi.com/blogs/blog/gitlab-embedded-devops-workshop-bootcamp-with-bittle-x?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [Talking Petoi robot dog with Azure AI Model Inference API integration](https://www.petoi.com/blogs/blog/petoi-robot-dog-and-azure-ai-model-inference-api-integration?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [Talk to Bittle robot dog with ChatGPT](https://www.petoi.com/blogs/blog/talk-to-bittle-robot-dog-with-chatgpt?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [Research spotlight](https://www.petoi.com/pages/robotics-research-and-academic-applications?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [Robot gallery](https://www.petoi.com/pages/robot-pet-gallery?utm_source=github&utm_medium=code&utm_campaign=github-opencat)
- [FAQ](https://www.petoi.com/pages/faq?utm_source=github&utm_medium=code&utm_campaign=github-opencat)

Follow the project:

- [YouTube](https://www.youtube.com/@petoicamp?utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-youtube-follow)
- [Twitter](https://twitter.com/petoicamp?utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-twitter-follow)
- [Instagram](https://www.instagram.com/petoicamp/?utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-instagram-follow)
- [Facebook](https://www.facebook.com/PetoiCamp/?utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-facebook-follow)
- [LinkedIn](https://www.linkedin.com/company/petoi/?utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-linkedin-follow)
- [TikTok](https://www.tiktok.com/@petoicamp/?utm_source=github&utm_medium=code&utm_campaign=github-opencat&utm_content=readme-tiktok-follow)

![](https://github.com/PetoiCamp/NonCodeFiles/blob/master/gif/backflip.gif?raw=true)

---

*The [legacy OpenCat repository](https://github.com/PetoiCamp/OpenCat-Old) is archived and no longer maintained.*
