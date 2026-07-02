<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,100:8A2BE2&height=200&section=header&text=Hi,%20I'm%20Matthew!&fontSize=45&fontColor=ffffff&animation=fadeIn&fontAlignY=35" width="100%"/>
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=A259FF&center=true&vCenter=true&width=650&lines=Aspiring+Cloud+Engineer+%E2%98%81%EF%B8%8F;BS+Computer+Science+%E2%80%A2+3rd+Year;AWS+%2B+Terraform+%2B+Serverless;Seeking+Cloud+Engineering+Internships" alt="Typing SVG" />
</div>
<br>
<img align="right" width="320" src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.gif">
<br>

<img align="right" width="320" src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.gif">

### 🖤 About Me

- 🎓 3rd Year **BS Computer Science** student — GPA **1.21**
- ☁️ Building production-grade infra on **AWS**, provisioned entirely with **Terraform**
- 🧩 Focused on **serverless architecture**, **CI/CD automation**, and **security-first IAM design**
- 💼 Currently seeking a **Cloud Engineering / Cloud Support** internship
- 📫 **punojustinematthew3@gmail.com**
- 🔗 [Connect on LinkedIn](https://www.linkedin.com/in/justine-matthew-puno-107b3b285/)

<br clear="right"/>

---

## 💜 Tech Stack

**Languages**

<img src="https://skillicons.dev/icons?i=py,ts,js,postgres&theme=dark" />

**Frameworks & Backend**

<img src="https://skillicons.dev/icons?i=nodejs,express,react,prisma&theme=dark" />

**IaC & DevOps**

<img src="https://skillicons.dev/icons?i=terraform,docker,git,githubactions,linux&theme=dark" />

**Cloud — AWS, grouped by function**

| Category | Services |
|---|---|
| 🖥️ Compute & Networking | ![EC2](https://img.shields.io/badge/EC2-000000?style=flat-square) ![ASG](https://img.shields.io/badge/ASG-000000?style=flat-square) ![VPC](https://img.shields.io/badge/VPC-000000?style=flat-square) ![ALB](https://img.shields.io/badge/ALB-000000?style=flat-square) ![Route53](https://img.shields.io/badge/Route_53-000000?style=flat-square) |
| 🗂️ Storage & Delivery | ![S3](https://img.shields.io/badge/S3-000000?style=flat-square) ![CloudFront](https://img.shields.io/badge/CloudFront-000000?style=flat-square) ![MediaConvert](https://img.shields.io/badge/MediaConvert-000000?style=flat-square) |
| 🗄️ Database & Caching | ![DynamoDB](https://img.shields.io/badge/DynamoDB-000000?style=flat-square) ![RDS](https://img.shields.io/badge/RDS-000000?style=flat-square) ![ElastiCache](https://img.shields.io/badge/ElastiCache_(Redis)-000000?style=flat-square) |
| ✉️ Messaging & Notifications | ![SQS](https://img.shields.io/badge/SQS-000000?style=flat-square) ![DLQ](https://img.shields.io/badge/DLQ-000000?style=flat-square) ![SNS](https://img.shields.io/badge/SNS-000000?style=flat-square) ![SES](https://img.shields.io/badge/SES-000000?style=flat-square) |
| 🔐 Security & Ops | ![IAM](https://img.shields.io/badge/IAM-000000?style=flat-square) ![SecretsManager](https://img.shields.io/badge/Secrets_Manager-000000?style=flat-square) ![CloudWatch](https://img.shields.io/badge/CloudWatch-000000?style=flat-square) ![SSM](https://img.shields.io/badge/SSM-000000?style=flat-square) ![ECR](https://img.shields.io/badge/ECR-000000?style=flat-square) ![Lambda](https://img.shields.io/badge/Lambda-000000?style=flat-square) |

---

## 🚀 Featured Projects

### ☁️ Serverless File Processing Pipeline
`AWS · Terraform · Python`

Event-driven, production-grade serverless pipeline, fully provisioned with **Terraform** across 9 modular components (compute, storage, messaging, notifications, observability).

- Multi-Lambda architecture — a **Trigger Lambda** forwards S3 upload events to SQS, a **Worker Lambda** processes files into DynamoDB and fires SNS/SES notifications, and a **URL Generator Lambda** exposes presigned POST URLs via Lambda Function URL (no API Gateway needed)
- Dual dead-letter queues (SQS DLQ + Lambda-level DLQ) for isolating failed messages, plus 30-day CloudWatch log retention across all functions
- Iterative least-privilege **IAM** — deployed with zero permissions, then added only the exact actions required per function, no wildcard ARNs
- Live frontend on Netlify (vanilla HTML/CSS/JS) supporting CSV, JSON, PDF, and image uploads up to 5MB via presigned S3 POST

`AWS S3` `Lambda` `SQS` `DLQ` `DynamoDB` `SNS` `SES` `CloudWatch` `IAM` `Terraform` `Python`

<br>

### 🎬 Ourframe — Cloud-Native Video Sharing Web App *(Ongoing)*
`AWS · Docker · React · TypeScript` — Netflix-inspired media app for couples

Co-developing full infrastructure and backend, with 80%+ of backend API functions complete and containerized builds already live on AWS.

- Secured a custom **VPC** (public/private subnets) — frontend via S3 + CloudFront (OAC/signed cookies), backend traffic through an ALB
- Built a **GitHub Actions** CI/CD pipeline that authenticates to AWS, builds Docker images tagged by commit SHA, and pushes to Amazon **ECR**
- Automated **zero-downtime** EC2 deployments in an Auto Scaling Group using AWS SSM Send-Command — no exposed SSH ports
- Added an **ElastiCache (Redis)** caching layer and isolated production data in PostgreSQL (migrating to RDS)
- Built an automated media pipeline with S3 + **MediaConvert** for HLS transcoding and low-latency playback
- All infrastructure provisioned via **Terraform**, secrets in AWS Secrets Manager, least-privilege IAM throughout

`EC2` `ASG` `S3` `CloudFront` `Route 53` `ALB` `VPC` `RDS` `ElastiCache` `MediaConvert` `Secrets Manager` `ECR` `Docker` `Node.js` `Express` `Prisma` `PostgreSQL` `React` `TypeScript`

---

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Jmpuno&show_icons=true&theme=dark&bg_color=000000&title_color=A259FF&text_color=ffffff&border_color=8A2BE2&icon_color=A259FF&count_private=true" height="165"/>
<img src="https://github-readme-streak-stats.herokuapp.com/?user=Jmpuno&theme=dark&background=000000&border=8A2BE2&stroke=8A2BE2&ring=A259FF&fire=A259FF&currStreakLabel=A259FF" height="165"/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Jmpuno&layout=compact&theme=dark&bg_color=000000&title_color=A259FF&text_color=ffffff&border_color=8A2BE2" height="165"/>

</div>

---

<div align="center">

### 💜 Let's Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-000000?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/justine-matthew-puno-107b3b285/)
[![Gmail](https://img.shields.io/badge/Gmail-000000?style=for-the-badge&logo=gmail&logoColor=white)](mailto:punojustinematthew3@gmail.com)

<img src="https://komarev.com/ghpvc/?username=Jmpuno&color=8A2BE2&style=for-the-badge&label=PROFILE+VIEWS"/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:8A2BE2,100:000000&height=100&section=footer"/>

</div>
