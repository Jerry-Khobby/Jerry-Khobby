<h1 align="center">Hi, I'm Jeremiah Anku Coblah 👋</h1>

<p align="center">
  <b>Data Engineer & Backend Engineer</b> · Accra, Ghana 🇬🇭
</p>

<p align="center">
  I build the systems that move, clean, store and serve data:<br/>
  batch and streaming pipelines, data warehouses, and the APIs and dashboards on top of them.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/jeremiah-coblah-anku-2b3732229"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:jeremiah.anku.coblah@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## 🧭 About me

I'm a software and data engineer from Ghana, and a Computer Science graduate of **Kwame Nkrumah University of Science and Technology (KNUST)**. I have about **2 years of experience in data engineering** and **3 years building backend systems** in Python and Node.js, across healthcare, payments, e-commerce and internal enterprise tools.

My work sits where software engineering and data engineering meet. On the data side, I build ETL/ELT pipelines with Airflow and dbt, stream real-time events through Kafka and Spark, and model data in Snowflake and Redshift so reports run fast and the numbers can be trusted. On the backend side, I design REST APIs, payment flows, authentication and real-time features, and I can build the React or Next.js dashboard that sits on top when a feature needs it.

What I enjoy most is making systems **reliable**. A pipeline that quietly loads wrong data is worse than one that fails loudly, so I build in validation, quality checks and clear error handling from the start. I like finding out *why* something is slow or broken by measuring it, rather than guessing, and I try to leave code documented and tested so the next engineer can work with it easily.


**Right now I'm:**
- 🔧 Building event-driven data pipelines on AWS with Glue, Step Functions, EventBridge and Terraform
- 📊 Going deeper into data modelling: star schemas, incremental loads, idempotent pipelines and data quality testing
- 🤖 Exploring the data layer behind AI systems: feature pipelines, evaluation data and model serving
- 🌍 Interested in fintech and healthcare data in Africa, where accuracy and reliability really matter

---

## 🛠️ What I do

<table>
<tr>
<td width="50%" valign="top">

### 🗄️ Data engineering
- Design and build **ETL/ELT pipelines** with Python, Apache Airflow and dbt, including scheduling, dependencies and failure handling
- Build **real-time streaming pipelines** with Apache Kafka and Spark Structured Streaming
- Model data warehouses in **Snowflake and Amazon Redshift** using star schemas for fast analytics
- Build **lakehouses** with Delta Lake on AWS
- Enforce **data quality**: validation, null checks, deduplication, lineage and rejected-record logging
- Clean and transform data with **Pandas and PySpark**
- Build **web scraping** workflows to automate data collection
- Create reports and dashboards in **Power BI, Grafana and Metabase**

</td>
<td width="50%" valign="top">

### ⚙️ Backend engineering
- Design **REST APIs** with FastAPI, Django REST Framework, NestJS and Express
- Integrate **third-party APIs**: Paystack payments, Cloudinary, SendGrid
- Handle **payment flows** including escrow, failures and refunds
- Build **real-time features** with WebSockets (Socket.IO)
- Implement **authentication and authorization**: JWT, OAuth 2.0 (Google), role-based access control
- Speed up apps with **Redis caching** and query optimization
- Write **tests** with Jest and pytest, and document APIs with Swagger/OpenAPI
- Build **frontends** with React, Next.js and Tailwind, and **mobile apps** with React Native

</td>
</tr>
</table>

---

## 🚀 Featured projects

### 🗄️ Data engineering

**🎵 Music Streaming Data Pipeline**
An event-driven, serverless pipeline on AWS that ingests simulated music-streaming events and turns them into genre-level listening metrics. Events land in S3 and trigger EventBridge, are queued in SQS so bursts don't overwhelm processing, and are processed by Glue jobs (PySpark and Python Shell) orchestrated with Step Functions. CloudWatch logs every run and sends Slack alerts when a job fails, and the whole infrastructure is defined in Terraform so it can be rebuilt from scratch.
`S3` `EventBridge` `SQS` `Step Functions` `Glue` `PySpark` `CloudWatch` `Terraform`

**🛒 Lakehouse for E-commerce Transactions**
A small data lakehouse on AWS that loads e-commerce transaction data from S3 into Delta Lake tables. Before loading, it runs data quality checks (null checks, timestamp validation and deduplication) and logs rejected records for review instead of silently dropping them. The pipeline is automated with Step Functions, with CI/CD for the Glue scripts through GitHub Actions.
`AWS Glue` `PySpark` `Delta Lake` `Step Functions` `GitHub Actions`

**❤️ Real-Time Heartbeat Monitoring System**
A streaming system that simulates patient heart-rate data and processes it in real time. Events flow through Kafka into a Spark Structured Streaming job that validates the incoming JSON and stores clean records in PostgreSQL, where Grafana dashboards show the readings live. The full stack runs locally with Docker Compose.
`Kafka` `Spark Structured Streaming` `PostgreSQL` `Grafana` `Docker Compose`

**🏢 Office Management System** *(work project)*
The data and backend layer of a multi-tenant office management system covering 10+ business domains. I designed the relational schema, built an ETL pipeline that turns raw badge-reader events into daily attendance and punctuality records, and wrote 50+ SQL views providing attendance, occupancy and absenteeism KPIs for employees, managers, HR and Facilities teams.
`PostgreSQL` `SQL Views` `ETL` `REST APIs` `RBAC`

### ⚙️ Backend & full-stack

**🛍️ CampusBid: Campus E-commerce Platform**
A marketplace where students buy and sell safely, with payment held until the buyer confirms delivery. The NestJS backend has 10+ feature modules, an escrow-style Paystack payment flow that handles failures and refunds, real-time buyer-seller chat with Socket.IO, image uploads through Cloudinary, Redis caching and login with JWT or Google. It's covered by **167 unit tests across 14 suites** and documented with Swagger/OpenAPI.
`NestJS` `MongoDB` `Redis` `Socket.IO` `Paystack` `Next.js` `Jest`

**🩺 Sepsis Prediction System**
My final-year project at KNUST: an end-to-end system that predicts sepsis risk in hospital patients from their vital signs and lab results over time. A hybrid CNN-LSTM model spots both sudden changes and gradual decline, a FastAPI backend serves single and batch predictions, and SHAP explanations show which factors drove each risk score so clinicians aren't looking at a black box. A Next.js dashboard supports CSV upload, real-time risk scoring and exportable PDF/CSV reports.
`TensorFlow` `Keras` `SHAP` `FastAPI` `SQLAlchemy` `Next.js`

**🎨 Real-Time Collaborative Whiteboard**
A drawing app where several people work on the same canvas at once and see each other's strokes instantly. Each canvas is its own room, so updates only reach the people on it, and drawing events are throttled to keep the app smooth under load. Drawings are saved in MongoDB so they're still there after a refresh.
`NestJS` `Socket.IO` `MongoDB` `Next.js` `Tailwind CSS`

---

## 💼 Experience

**Data Engineer · AmaliTech** · Nov 2025 – Oct 2026 · Kumasi
- Built ETL/ELT pipelines with Python, Apache Airflow and dbt, cutting pipeline failure rates by an estimated **35%**
- Built and maintained warehouse models in Amazon Redshift and Snowflake, improving query performance by an estimated **45%**
- Built real-time streaming pipelines with Kafka and Spark, reducing data delivery lag by an estimated **40%**
- Enforced data quality and lineage checks across pipelines and warehouse layers
- Built backend services and **50+ REST endpoints** with role-based access for HR and Facilities dashboards

**Backend / Data Engineer · BenchFive** (Internship) · Sep 2024 – Jan 2025 · Remote
- Built web scraping and ingestion workflows that automated previously manual data collection
- Cleaned, transformed and validated datasets with Pandas before storage and analysis
- Developed REST APIs with Django REST Framework, working with a Next.js frontend team

**Agile Developer · Xcelsz** (Contract) · Remote
- Designed RESTful API endpoints for an internal business application within an Agile team

**Backend Developer · Ideation Axis Group** (Internship) · Sep – Nov 2024 · Remote

**Mobile Application Developer · Zap Technology** (Internship) · Oct – Dec 2023
- Built mobile features with React Native, Redux Toolkit and Firebase

**Web Developer · GI-KACE** (Internship) · Sep – Oct 2023 · Accra
- Built full-stack features with FastAPI, PostgreSQL, HTML, CSS and JavaScript

---

## 🧰 Tools & technologies

**Languages**

<img src="https://skillicons.dev/icons?i=python,ts,js,java,cpp,html,css&perline=10" alt="Languages"/>

![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**Backend frameworks**

<img src="https://skillicons.dev/icons?i=fastapi,django,nestjs,nodejs,express&perline=10" alt="Backend"/>

![Django REST Framework](https://img.shields.io/badge/Django_REST_Framework-A30000?style=flat-square&logo=django&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white)
![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=flat-square&logo=mongoose&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![OAuth 2.0](https://img.shields.io/badge/OAuth_2.0-3C4043?style=flat-square)

**Frontend & mobile**

<img src="https://skillicons.dev/icons?i=react,nextjs,redux,tailwind,bootstrap,materialui,firebase&perline=10" alt="Frontend"/>

![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)

**Databases**

<img src="https://skillicons.dev/icons?i=postgres,mysql,mongodb,redis,sqlite&perline=10" alt="Databases"/>

![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=flat-square)

**Data engineering & big data**

<img src="https://skillicons.dev/icons?i=kafka&perline=10" alt="Kafka"/>

![Apache Airflow](https://img.shields.io/badge/Apache_Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![Amazon Redshift](https://img.shields.io/badge/Amazon_Redshift-8C4FFF?style=flat-square)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-003366?style=flat-square)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)

**Cloud & AWS**

<img src="https://skillicons.dev/icons?i=aws&perline=10" alt="AWS"/>

![S3](https://img.shields.io/badge/S3-569A31?style=flat-square)
![Glue](https://img.shields.io/badge/Glue-8C4FFF?style=flat-square)
![Lambda](https://img.shields.io/badge/Lambda-FF9900?style=flat-square)
![Step Functions](https://img.shields.io/badge/Step_Functions-E7157B?style=flat-square)
![EventBridge](https://img.shields.io/badge/EventBridge-E7157B?style=flat-square)
![SQS](https://img.shields.io/badge/SQS-E7157B?style=flat-square)
![CloudWatch](https://img.shields.io/badge/CloudWatch-E7157B?style=flat-square)

**DevOps & tooling**

<img src="https://skillicons.dev/icons?i=docker,terraform,githubactions,git,github,linux,vscode,postman&perline=10" alt="DevOps"/>

![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black)

**Integrations**

![Paystack](https://img.shields.io/badge/Paystack-00C3F7?style=flat-square)
![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=flat-square&logo=cloudinary&logoColor=white)
![SendGrid](https://img.shields.io/badge/SendGrid-1A82E2?style=flat-square)

**AI / ML**

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-Explainability-555555?style=flat-square)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square)

**Visualisation & BI**

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Metabase](https://img.shields.io/badge/Metabase-509EE3?style=flat-square&logo=metabase&logoColor=white)


---

## 🎓 Education & certifications

**BSc Computer Science** · Kwame Nkrumah University of Science and Technology (KNUST) · 2021 – 2025
Final-year project: an end-to-end sepsis prediction system using a CNN-LSTM model on clinical time-series data, with SHAP explainability.

![AWS](https://img.shields.io/badge/AWS_Certified-Cloud_Practitioner-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)
![DataCamp](https://img.shields.io/badge/DataCamp-Data_Engineer_Associate-03EF62?style=flat-square&logo=datacamp&logoColor=black)
![DataCamp](https://img.shields.io/badge/DataCamp-Machine_Learning_Engineer-03EF62?style=flat-square&logo=datacamp&logoColor=black)

---

## 📈 GitHub activity

<p align="center">
  <img src="https://streak-stats.demolab.com?user=Jerry-Khobby&theme=tokyonight&hide_border=true&date_format=M%20j%5B%2C%20Y%5D" alt="GitHub streak"/>
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Jerry-Khobby&show_icons=true&hide_border=true&theme=tokyonight&count_private=true" height="165" alt="GitHub stats"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Jerry-Khobby&layout=compact&hide_border=true&theme=tokyonight&hide=jupyter%20notebook,cython,html" height="165" alt="Top languages"/>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Jerry-Khobby&theme=tokyo-night&hide_border=true" alt="Contribution graph"/>
</p>

---

<h3 align="center">🤝 Let's work together</h3>

<p align="center">
  I'm open to <b>data engineering</b> and <b>backend engineering</b> roles, remote or any where in Ghana<br/>
  The quickest way to reach me is by <a href="mailto:jeremiah.anku.coblah@gmail.com">email</a> or on <a href="https://www.linkedin.com/in/jeremiah-coblah-anku-2b3732229">LinkedIn</a>.
</p>
