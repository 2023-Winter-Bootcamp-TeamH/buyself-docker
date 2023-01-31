<p align="center">
<img width="1470" alt="스크린샷 2023-01-31 오후 2 34 10" src="https://user-images.githubusercontent.com/77673029/215676052-3c6b8760-c5c6-4ce5-8553-5668a4953f12.png">
</p>

# 🍰 BuySelf

<p align="center">
<strong>무인 상품 인식 계산대 <br></strong>계산할 때 바코드로 하나하나 찍지 말고 사진 한 장으로 상품을 인식해보세요!
</p>
<br>



## 📹 Demo



## 💡Tech Stack

<br>

<p align="center">
<img src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black"> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=TypeScript&logoColor=white"> <img src="https://img.shields.io/badge/styled components-DB7093?style=for-the-badge&logo=styledcomponents&logoColor=black">

</p>  
<p align="center">
<img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=Flask&logoColor=white">  <img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=Celery&logoColor=white"> <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=RabbitMQ&logoColor=white"> <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=white"> <img src="https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=NGINX&logoColor=white"> <img src="https://img.shields.io/badge/Gunicorn-499848?style=for-the-badge&logo=Gunicorn&logoColor=white">
  </p>
<p align="center">
<img src="https://img.shields.io/badge/Amazon AWS-232F3E?style=for-the-badge&logo=Amazon AWS&logoColor=white"> <img src="https://img.shields.io/badge/Amazon S3-569A31?style=for-the-badge&logo=Amazon S3&logoColor=white"> <img src="https://img.shields.io/badge/GitKraken-179287?style=for-the-badge&logo=GitKraken&logoColor=white"> <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=Docker&logoColor=white"> <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=Swagger&logoColor=white">   <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=black">
<img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=black"> <img src="https://img.shields.io/badge/redis-DC382D?style=for-the-badge&logo=redis&logoColor=black">

</p>

```
- Frontend : React
- Backend : Flask
- Web Server: Nginx
- Middleware : Gunicorn
- AI model : YOLOv5
- DevOps : Docker
- Database: MySQL
- API Documentation : Swagger
- Deployment : AWS
- VCS: Git
- Monitoring: Prometheus, Grafana, Elastic stack
- Cache: Redis
```



## 💻 System Architecture

![image](https://user-images.githubusercontent.com/77673029/215631738-2e080de9-8002-4de0-b064-12560660a59a.png)



## 📗 API

![image](https://user-images.githubusercontent.com/77673029/215632356-09bdb1d4-50b1-4f5e-a6cc-c7a6cad63179.png)



## 📈 Monitoring

![image](https://user-images.githubusercontent.com/77673029/215633253-6baf3c12-faf7-46f0-b69e-b4a8f4539721.png)



## 🤖 AI

![image](https://user-images.githubusercontent.com/77673029/215633498-0f75dcf2-29d9-4bd3-8f82-1075acc73d60.png)



## 🚀 How to Start

### 1. Clone Repository

```
https://github.com/2023-Winter-Bootcamp-TeamH/buyself-docker
```

### 2. Install Pacakages

```
$ cd buyself-frontend
$ npm run build
```

### 3. Set .env file

```bash
### buyself-backedn/config
# === Database ===
DB_USERNAME =
DB_PASSWORD =
DB_HOST =
DB_SCHEMA =
DB_PORT =
# === S3Bucket ===
ACCESS_KEY_ID =
SECRET_ACCESS_KEY =
S3_BUCKET_REGION =
S3_BUCKET_NAME =
```

### 4. Run Docker

```
$ docker-compose up --build         # build images and run containers
```



## 📂 Directory Structure

```bash
📦buyself-docker
 ┣ 📂logging-example
 ┃ ┣ 📂elasticsearch
 ┃ ┃ ┣ 📂config
 ┃ ┃ ┃ ┗ 📜elasticsearch.yml
 ┃ ┃ ┗ 📜Dockerfile
 ┃ ┣ 📂filebeat
 ┃ ┃ ┣ 📂config
 ┃ ┃ ┃ ┗ 📜filebeat.yml
 ┃ ┃ ┗ 📜Dockerfile
 ┃ ┣ 📂kibana
 ┃ ┃ ┣ 📂config
 ┃ ┃ ┃ ┗ 📜kibana.yml
 ┃ ┃ ┗ 📜Dockerfile
 ┃ ┗ 📂logstash
 ┃ ┃ ┣ 📂config
 ┃ ┃ ┃ ┗ 📜logstash.yml
 ┃ ┃ ┣ 📂pipeline
 ┃ ┃ ┃ ┗ 📜logstash.conf
 ┃ ┃ ┗ 📜Dockerfile
 ┣ 📂nginx
 ┃ ┣ 📂log
 ┃ ┃ ┣ 📜access.log
 ┃ ┃ ┗ 📜error.log
 ┃ ┣ 📜Dockerfile
 ┃ ┗ 📜nginx.conf
 ┣ 📂settings
 ┃ ┗ 📜.env
 ┣ 📜.gitignore
 ┣ 📜datasource.yml
 ┣ 📜docker-compose.prod.yml
 ┣ 📜docker-compose.yml
 ┗ 📜prometheus.yml
📦buyself-backend
 ┣ 📂.idea
 ┃ ┣ 📂inspectionProfiles
 ┃ ┃ ┣ 📜profiles_settings.xml
 ┃ ┃ ┗ 📜Project_Default.xml
 ┃ ┣ 📜.gitignore
 ┃ ┣ 📜buyself-backend.iml
 ┃ ┣ 📜modules.xml
 ┃ ┣ 📜vcs.xml
 ┃ ┗ 📜workspace.xml
 ┣ 📂config
 ┃ ┣ 📜DatabaseConfig.py
 ┃ ┣ 📜s3bucketConfig.py
 ┃ ┣ 📜s3Connection.py
 ┃ ┗ 📜__init__.py
 ┣ 📂controller
 ┃ ┣ 📜elasticSearch.py
 ┃ ┣ 📜imageController.py
 ┃ ┣ 📜listController.py
 ┃ ┣ 📜paymentController.py
 ┃ ┣ 📜predictController.py
 ┃ ┣ 📜productData.json
 ┃ ┣ 📜searchController.py
 ┃ ┗ 📜__init__.py
 ┣ 📂migrations
 ┃ ┣ 📂versions
 ┃ ┃ ┣ 📜3cb8144b6381_.py
 ┃ ┃ ┗ 📜60f0e59f54f4_.py
 ┃ ┣ 📜alembic.ini
 ┃ ┣ 📜env.py
 ┃ ┣ 📜README
 ┃ ┗ 📜script.py.mako
 ┣ 📂models
 ┃ ┣ 📜products.py
 ┃ ┗ 📜__init__.py
 ┣ 📜.git
 ┣ 📜.gitignore
 ┣ 📜app.py
 ┣ 📜best.pt
 ┣ 📜detect.py
 ┣ 📜Dockerfile
 ┣ 📜README.md
 ┣ 📜requirements.txt
 ┣ 📜tasks.py
 ┣ 📜views.py
 ┗ 📜wsgi.py
 📦buyself-frontend
 ┣ 📂node_modules
 ┣ 📂public
 ┣ 📂src
 ┃ ┣ 📂components
 ┃ ┃ ┣ 📂buy
 ┃ ┃ ┃ ┣ 📜BuyButton.tsx
 ┃ ┃ ┃ ┣ 📜BuyInfoBox.tsx
 ┃ ┃ ┃ ┣ 📜BuyInfoLabel.tsx
 ┃ ┃ ┃ ┣ 📜BuyTable.tsx
 ┃ ┃ ┃ ┣ 📜Divisions.tsx
 ┃ ┃ ┃ ┣ 📜LeftLayout.tsx
 ┃ ┃ ┃ ┣ 📜TdProduct.tsx
 ┃ ┃ ┃ ┗ 📜TextBox.tsx
 ┃ ┃ ┣ 📂checklist
 ┃ ┃ ┃ ┣ 📜CheckList.tsx
 ┃ ┃ ┃ ┣ 📜CheckListCard.tsx
 ┃ ┃ ┃ ┣ 📜CheckListItemList.tsx
 ┃ ┃ ┃ ┣ 📜Division.ts
 ┃ ┃ ┃ ┗ 📜Footer.tsx
 ┃ ┃ ┣ 📂common
 ┃ ┃ ┃ ┣ 📜CustomAxios.ts
 ┃ ┃ ┃ ┣ 📜Header.tsx
 ┃ ┃ ┃ ┣ 📜Loading.tsx
 ┃ ┃ ┃ ┣ 📜Modal.tsx
 ┃ ┃ ┃ ┣ 📜NotFound.tsx
 ┃ ┃ ┃ ┗ 📜ScrollToTop.tsx
 ┃ ┃ ┣ 📂main
 ┃ ┃ ┃ ┣ 📜Button.tsx
 ┃ ┃ ┃ ┣ 📜ButtonBox.tsx
 ┃ ┃ ┃ ┣ 📜MainContainer.tsx
 ┃ ┃ ┃ ┣ 📜MainPage.css
 ┃ ┃ ┃ ┣ 📜MainPage.css.map
 ┃ ┃ ┃ ┗ 📜MainPage.scss
 ┃ ┃ ┣ 📂Payment
 ┃ ┃ ┃ ┣ 📜PaymentButton.tsx
 ┃ ┃ ┃ ┣ 📜Paymentmain.css
 ┃ ┃ ┃ ┗ 📜Paymentmain.tsx
 ┃ ┃ ┣ 📂PaymentFail
 ┃ ┃ ┃ ┣ 📜PaymentFail.css
 ┃ ┃ ┃ ┣ 📜PaymentFail.tsx
 ┃ ┃ ┃ ┗ 📜PaymentFailButton.tsx
 ┃ ┃ ┣ 📂products
 ┃ ┃ ┃ ┣ 📜Pagination.tsx
 ┃ ┃ ┃ ┣ 📜ProductCard.tsx
 ┃ ┃ ┃ ┣ 📜ProductCardList.tsx
 ┃ ┃ ┃ ┣ 📜productSearch.tsx
 ┃ ┃ ┃ ┣ 📜Toast.tsx
 ┃ ┃ ┃ ┗ 📜ToastStyle.tsx
 ┃ ┃ ┣ 📂scan
 ┃ ┃ ┃ ┣ 📜BuyCard.tsx
 ┃ ┃ ┃ ┣ 📜BuyList.tsx
 ┃ ┃ ┃ ┣ 📜ChecklistBox.tsx
 ┃ ┃ ┃ ┣ 📜MediaQuery.ts
 ┃ ┃ ┃ ┣ 📜ScanButton.tsx
 ┃ ┃ ┃ ┗ 📜Scanner.tsx
 ┃ ┃ ┗ 📂search
 ┃ ┃ ┃ ┗ 📜SearchCardList.tsx
 ┃ ┣ 📂images
 ┃ ┣ 📂pages
 ┃ ┃ ┣ 📜BuyPage.tsx
 ┃ ┃ ┣ 📜MainPage.tsx
 ┃ ┃ ┣ 📜PaymentFailPage.tsx
 ┃ ┃ ┣ 📜PaymentPage.tsx
 ┃ ┃ ┣ 📜ProductPage.tsx
 ┃ ┃ ┣ 📜ScanPage.tsx
 ┃ ┃ ┗ 📜SearchPage.tsx
 ┃ ┣ 📜App.css
 ┃ ┣ 📜App.test.tsx
 ┃ ┣ 📜App.tsx
 ┃ ┣ 📜index.css
 ┃ ┣ 📜index.tsx
 ┃ ┣ 📜logo.svg
 ┃ ┣ 📜react-app-env.d.ts
 ┃ ┣ 📜reportWebVitals.ts
 ┃ ┣ 📜setupTests.ts
 ┃ ┗ 📜store.ts
 ┣ 📜.eslintrc.json
 ┣ 📜.gitignore
 ┣ 📜.prettierrc
 ┣ 📜Dockerfile
 ┣ 📜package-lock.json
 ┣ 📜package.json
 ┣ 📜README.md
 ┣ 📜tsconfig.json
 ┗ 📜.gitignore
┣ 📜 README.md
┣ 📜 .gitignore
┣ 📜 datasource.yml
┣ 📜 docker-compose.prod.yml
┣ 📜 docker-compose.yml
┣ 📜 prometheus.yml
┣ 📂 nginx
┣ 📂 logging-example
┗ 📂 prometheus
```



## 👨‍👩‍👧‍👧 팀원

|                                              [최지미](https://github.com/rabbit-22)                                               |                                              [백한결](https://github.com/snake7667)                                               |                                           [박준수](https://github.com/GaBaljaintheroom)                                           |                                               [윤일권](https://github.com/1ilkwon)                                                |                                               [엄선아](https://github.com/eomseona)                                               |                    [권광재](https://github.com/kwongwangjae)                     |
| :-------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------: |
| <img width = "520" src ="https://user-images.githubusercontent.com/77673029/215674043-950d2d6b-b220-460c-bb72-f1d77beb81c4.jpeg"> | <img width = "520" src ="https://user-images.githubusercontent.com/77673029/215674489-3e420f79-7ef2-4f2b-8d9d-d4b48a0ad1ce.jpeg"> | <img width = "520" src ="https://user-images.githubusercontent.com/77673029/215674065-f2b6cd3a-c1f4-4288-988a-2a08e6d52e39.jpeg"> | <img width = "520" src ="https://user-images.githubusercontent.com/77673029/215676854-4ad23ce2-5182-4d76-9dd8-27940d78dd8a.jpeg"> | <img width = "520" src ="https://user-images.githubusercontent.com/77673029/215674500-3a48f7d6-6e1e-41ec-9d48-3f7f537ec695.jpeg"> | <img width = "520" src ="https://user-images.githubusercontent.com/77673029/215679951-f252b196-a69b-4b28-8b46-d9ab9a041d9f.jpeg"> |
|                                                    Leader, Front-end Developer                                                    |                                                      Back-end Developer, AI                                                       |                                                    Back-end Developer, DevOps                                                     |                                                    Back-end Developer, DevOps                                                     |                                                        Front-end Developer                                                        |                               Front-end Developer                                |
