# Camila Félix dos Reis

<div align="center">

**Computer Engineering Student | Systems Integration & Architecture • Cyber-Physical Systems • IoT • Embedded**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/camila-felix-dos-reis)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/cawzkf)
[![Lattes](https://img.shields.io/badge/Lattes-0A66A6?style=for-the-badge&logo=academia&logoColor=white)](http://lattes.cnpq.br/4899528348009614)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:camilafelixdosres@gmail.com)
[![Location](https://img.shields.io/badge/Location-Manaus,%20AM-pink?style=for-the-badge&logo=google-maps&logoColor=white)](https://maps.google.com)

![Profile Views](https://komarev.com/ghpvc/?username=cawzkf&color=ff69b4&style=for-the-badge)

</div>

---

## About Me

Computer Engineering student researching **distributed cyber-physical systems (CPS)** — how physical assets, sensors, and cloud services integrate through industrial standards like **OPC UA**, **Asset Administration Shell (AAS)**, and **RAMI 4.0**. My work centers on architectures for physical–digital integration, **digital twins**, and local processing in infrastructure-constrained environments, validated through **vehicular simulation** and **intelligent aquaculture** case studies.

I learn by engineering things end to end — prototypes, drivers, and integrations that connect hardware to software in real environments. I work with **ESP32/ESP8266** and **Raspberry Pi** edge gateways, communication protocols (**MQTT, WebSockets, TCP/IP**), and **AWS** pipelines (Lambda, S3, API Gateway, Rekognition), combining edge and cloud to deliver real-time insight. I also build native **Android** applications in **Kotlin (MVVM)**.

---

## Tech Stack

### Programming Languages
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### Tools & Version Control
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitLab](https://img.shields.io/badge/GitLab-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI%2FCD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![PyCharm](https://img.shields.io/badge/PyCharm-000000?style=for-the-badge&logo=pycharm&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

---

## Cyber-Physical Systems, IoT & Industrial Integration

![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-C51A4A?style=for-the-badge&logo=raspberrypi&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![OPC UA](https://img.shields.io/badge/OPC_UA-004A8F?style=for-the-badge&logo=opc-foundation&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white)

Experience with:

- Distributed cyber-physical architectures and physical–digital integration
- Industrial semantics: **Asset Administration Shell (AAS)**, **OPC UA**, **RAMI 4.0** layering
- **Digital twin** modeling and real-time data synchronization
- Sensor data acquisition and device communication (MQTT, TCP/IP, HTTP, WebSockets)
- ESP32/ESP8266 programming and Raspberry Pi edge gateways
- Drivers that convert raw sensor data into structured information models

---

## Cloud & Backend

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)

- AWS Lambda, S3, API Gateway, Rekognition
- Firebase Auth, Firestore, Realtime Database
- Data processing pipelines and hardware-to-cloud integration

---

## Mobile Development

![Android Studio](https://img.shields.io/badge/Android_Studio-3DDC84?style=for-the-badge&logo=android-studio&logoColor=white)

- Native Android (Kotlin – MVVM)
- REST API integration
- Clean and responsive UI/UX with real-time data visualization

---

## Featured Projects

### **MachForce – Energy Digital Twin (Shell Eco-marathon)**
*2026 – Present | Research project · MachForce team*

Software foundation for the energy **digital twin** of the MachForce electric vehicle. The core is a **simplified longitudinal dynamic model** that estimates instantaneous power, accumulated energy, and battery State of Charge (SoC) — including regenerative braking — and publishes the energy state over **MQTT** for asynchronous consumption by the team's local backend. This model is already in use as the base of the car's software.

Since the physical vehicle isn't instrumented yet, the model is currently fed and validated using the **CARLA** simulator as a stand-in data source. The architecture keeps the physics domain fully decoupled from the data source, so CARLA will be swapped for the **real onboard telemetry / data acquisition** we're building — sensors for voltage, current, temperature, and speed over an RS485 bus — which will feed the digital twin of the actual car.

**Architecture:** RAMI 4.0 layering with separation of concerns (Integration → Functional → Information). AAS (Eclipse BaSyx) and OPC UA layers are mapped on the roadmap and deferred while the embedded hardware is prototyped.

**Tech:** Python, MQTT (Mosquitto), CARLA (current data source), pytest, structlog, pygame (HUD); embedded telemetry hardware in development
**Highlights:** 29 unit tests; analytical verification with 0.00% error; offline synthetic simulation; real-time strategic indicators (specific consumption, estimated range, moving-average power)

---

### **Caiçá – Indigenous Medicinal Plant Identification**
*Feb–May 2025 | Research & Extension Project*

Android application using **AI and computer vision** to identify Amazonian medicinal plants.

**Tech:** Kotlin, AWS Lambda, Rekognition, S3, RDS
**Features:** Image capture, cloud inference, botanical dataset
**Impact:** Supports cultural preservation and scientific accessibility

---

### **Energy Consumption Monitoring System**
*Aug–Nov 2024 | Awarded 2nd place at Engenharia Week*

IoT system for real-time monitoring of electrical consumption using ESP8266 + Firebase + Android.

**Tech:** ESP8266, Firebase, Android
**Highlights:** Real-time graphs, cost estimation, mobile dashboard

---

### **Simple Timer App**
Minimalist Android timer built using Kotlin and real-time UI updates.

---

## Research Output

- **REIS, C. F.** *Arquitetura de Sistema Ciberfísico Offline com Representação AAS Aplicada à Aquicultura.* 2025. (Work presentation / Seminar)

---

## Research & Interests

I focus on connecting the physical and digital worlds through cyber-physical systems, exploring how devices, sensors, cloud services, and industrial standards work together to build smarter, more reliable systems. Current areas of study and experimentation:

- **Cyber-Physical Systems (CPS)** — distributed architectures for real environments
- **Industrial interoperability** — OPC UA, Asset Administration Shell (AAS), RAMI 4.0
- **Digital twins** — modeling, data mapping, and real-time synchronization (vehicular simulation case study)
- **Edge & local processing** — Raspberry Pi gateways and computation under infrastructure constraints
- **Embedded development** — ESP32/ESP8266 and embedded acquisition stacks
- **Cloud pipelines** — AWS (Lambda, API Gateway, S3, Rekognition)
- **AI-based decision support** applied to CPS
- **Prototyping & experimentation** as the primary method for learning complex architectures

---

## GitHub Stats

<div align="center">

![GitHub Stats](https://github-readme-stats-peach-nine-63.vercel.app/api?username=cawzkf&show_icons=true&theme=dracula&hide_border=true&bg_color=0d1117&title_color=ff69b4&icon_color=ff69b4&text_color=ffffff)

![Top Languages](https://github-readme-stats-peach-nine-63.vercel.app/api/top-langs/?username=cawzkf&layout=compact&theme=dracula&hide_border=true&bg_color=0d1117&title_color=ff69b4&text_color=ffffff)

![GitHub Streak](https://streak-stats.demolab.com/?user=cawzkf&theme=dark&hide_border=true&background=0d1117&border=0d1117&stroke=ff69b4&ring=ff69b4&fire=ff69b4&currStreakLabel=ff69b4&sideLabels=ffffff&dates=ffffff&currStreakNum=ffffff&sideNums=ffffff)


</div>

---

## Education

**Bachelor in Computer Engineering** *(in progress, since 2024)*
*Faculdade Matias Machline – Manaus, AM*

---

## Contact

Interested in cyber-physical systems, IoT, embedded development, cloud integration, and emerging technologies.
Feel free to reach out!

- **LinkedIn:** [camila-felix-dos-reis](https://linkedin.com/in/camila-felix-dos-reis)
- **Email:** camilafelixdosres@gmail.com
- **Lattes:** [lattes.cnpq.br/4899528348009614](http://lattes.cnpq.br/4899528348009614)
