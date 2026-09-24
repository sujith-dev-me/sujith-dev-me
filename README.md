<h1 align="center">Sujith Ravikumar</h1>

<p align="center">
  <b>Cloud Engineer · IoT Cloud · Backend Systems</b><br/>
  I build the cloud and backend systems that connect physical devices to software.
</p>

<p align="center">
  <a href="https://linkedin.com/in/sujith-ravikumar"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:sujithravikumar0306@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://instagram.com/sujith_ravikumar_"><img src="https://img.shields.io/badge/Instagram-E4405F?style=flat&logo=instagram&logoColor=white" alt="Instagram"/></a>
</p>

---

## About

I'm a **Cloud Engineer at L&T Semiconductor Technologies**, an Indian fabless semiconductor company. I work on cloud platforms and connected-device systems: secure, scalable infrastructure that links embedded devices to cloud services and backend applications.

My work sits where four layers meet:

```
  Embedded Systems  ──►  Connectivity  ──►  Cloud  ──►  Backend
  MCU · firmware         LTE · Wi-Fi         AWS IoT      REST · GraphQL
  QCM2290 · QCX216       BLE · GNSS          Core · MQTT  PostgreSQL
  A/B OTA · DFOTA        TLS                 Lambda · S3  IAM · OAuth2
```

Day to day, that means AWS IoT Core, MQTT, device provisioning and lifecycle, telemetry, remote AT command execution, GNSS/TPS positioning, OTA/FOTA workflows and the backend APIs behind them, mostly for connected mobility and smart-device platforms.

I'm also doing an **M.Tech in Embedded Systems at BITS Pilani**, so I can work on both the device side and the cloud side.

---

## Selected work

| Project | What it is | Highlights |
|---|---|---|
| **SIPS**: Secure Identity & Provisioning Server | Identity and provisioning platform for users, organizations, factories, firmware releases, product catalog, TAC management and IMEI provisioning | Node.js · GraphQL · Prisma · PostgreSQL · Keycloak · OAuth2/JWT · Docker · AWS |
| **TPS / AT Command Server** | Runs AT commands on remote devices over MQTT, using per-device topics, request-UUID correlation, timeouts and response validation | Python · MQTT · AWS IoT Core · TLS · REST · EC2 |
| **QCM2290 A/B OTA** | A/B-partition OTA workflow for automotive and connected devices, with slot switching, boot validation and rollback | **99% fewer boot failures** |
| **DFOTA / QCX216** | Fault-tolerant firmware-over-the-air updates for connected embedded platforms: delivery, verification, slot activation | **60% faster OTA** |
| **Internal Dashboard Server** | Backend and dashboard for operational visibility and connected-device workflows | **Provisioning in under 2 seconds** |

<details>
<summary><b>How the AT Command Server works</b></summary>

```mermaid
sequenceDiagram
    participant C as API client
    participant B as Backend
    participant M as AWS IoT Core (MQTT)
    participant D as Device
    C->>B: POST AT command
    B->>B: Generate request UUID
    B->>M: Publish to device command topic
    M->>D: Deliver command
    D->>M: Response + same UUID
    M->>B: Response topic
    B->>B: Correlate, validate, handle timeout
    B-->>C: Result
```

</details>

---

## Experience

**Cloud Engineer**, L&T Semiconductor Technologies · *Mar 2025 – Present*
IoT cloud, device provisioning and lifecycle, telemetry, OTA/FOTA, backend APIs for connected mobility and smart devices.

**Software Engineer**, Buyerstage · *Jan 2024 – Jan 2025*
Backend and platform engineering: API development, database-backed services, faster delivery of backend workflows.

---

## Tech stack

**Languages**<br/>
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Embedded C](https://img.shields.io/badge/Embedded_C-A8B9CC?style=flat-square&logo=c&logoColor=black)

**Backend**<br/>
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

**Cloud & IoT**<br/>
![AWS IoT Core](https://img.shields.io/badge/AWS_IoT_Core-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)
![AWS Lambda](https://img.shields.io/badge/Lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white)
![EC2](https://img.shields.io/badge/EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white)
![S3](https://img.shields.io/badge/S3-569A31?style=flat-square&logo=amazons3&logoColor=white)
![EventBridge](https://img.shields.io/badge/EventBridge-FF4F8B?style=flat-square&logo=amazonwebservices&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white)

**Security & identity**<br/>
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=flat-square&logo=keycloak&logoColor=white)
![OAuth2](https://img.shields.io/badge/OAuth2-3C4043?style=flat-square)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![TLS / X.509](https://img.shields.io/badge/TLS_/_X.509-3C4043?style=flat-square)

**DevOps**<br/>
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Embedded & automotive:** QCM2290 · QCX216 · RH850 · A/B partitioning · DFOTA · secure boot concepts · telematics · 2W connected clusters

---

## Education

- **M.Tech, Embedded Systems**, BITS Pilani · *Nov 2025 – Present*
- **B.Tech, Information Technology**, Dr. Mahalingam College of Engineering and Technology · GPA 9.2

---

<p align="center"><i>Device → Connectivity → Cloud → Backend</i></p>
