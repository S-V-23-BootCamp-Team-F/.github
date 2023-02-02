[한국어](README_ko.md) | English

# CropDoctor

![D8771DDC-42B5-42E6-922B-01C0443DB602](https://user-images.githubusercontent.com/83527046/215812755-bda68906-ce2e-41de-b671-4f2a555b3777.png)
<br>

## 🍀 Introduction

Cropdoctor is a service that diagnosis the disease of your crops and offers solutions that fit your disease.👩🏻‍🌾 
<br>

## 📌 System Architecture
![MacBook Pro 16_ - 1](https://user-images.githubusercontent.com/83527046/215812708-2d8dc494-2d49-4aea-8192-152852902497.png)


## 📚 TECH STACKS

|Frontend|Backend|Monitoring|Database&Storage|DevOps|AI| 
| :----: | :---: | :-----: | :---------: | :------: | :-----: |
| <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=Vite&logoColor=white"><br><img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=React&logoColor=white"><br><img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=TypeScript&logoColor=white"><br><img src="https://img.shields.io/badge/Tailwind CSS-06B6D4?style=for-the-badge&logo=Tailwind CSS&logoColor=white"><br> | <br><img src="https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=NGINX&logoColor=white"><br><img src="https://img.shields.io/badge/Gunicorn-499848?style=for-the-badge&logo=Gunicorn&logoColor=white"><br><img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=Django&logoColor=white"><br><img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=RabbitMQ&logoColor=white"><br><img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=Celery&logoColor=white"><br><img src="https://img.shields.io/badge/Swagger-85EA2D.svg?style=for-the-badge&logo=Swagger&logoColor=white"> | <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=Grafana&logoColor=white"><br><img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white"><br><img src="https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=Elasticsearch&logoColor=white"><br><img src="https://img.shields.io/badge/Logstash-005571?style=for-the-badge&logo=Logstash&logoColor=white"><br><img src="https://img.shields.io/badge/Kibana-005571?style=for-the-badge&logo=Kibana&logoColor=white"><br><img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=Slack&logoColor=white"> |<img src="https://img.shields.io/badge/Amazon RDS-527FFF?style=for-the-badge&logo=Amazon RDS&logoColor=white"><br><img src="https://img.shields.io/badge/Amazon S3-569A31?style=for-the-badge&logo=Amazon S3&logoColor=white"><br><img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> <br>| <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=Docker&logoColor=white"><br><img src="https://img.shields.io/badge/Amazon EC2 -FF9900?style=for-the-badge&logo=Amazon EC2&logoColor=white"><br><img src="https://img.shields.io/badge/Github Actions-2088FF?style=for-the-badge&logo=Github Actions&logoColor=white"><br> | <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=PyTorch&logoColor=white"> <br> <img src="https://img.shields.io/badge/YOLO-00FFFF?style=for-the-badge&logo=YOLO&logoColor=white"> <br>|

<br>

## 💻 Installation Process
> <b>Docker repository clone </b>

```
git clone --recursive https://github.com/S-V-23-BootCamp-Team-F/docker.git
```

<br>

> <b>Set .env in the backend folder </b>

```
SECRET_KEY = {Django SECRET_KEY}

# AWS S3 connect
AWS_ACCESS_KEY = {AWS_ACCESS_KEY}
AWS_SECRET_KEY = {AWS_SECRET_KEY}
AWS_REGION = {AWS_REGION}

# S3 Storages
S3_BUCKET_NAME = {S3_BUCKET_NAME}

MYSQL_NAME = {MYSQL_NAME}
MYSQL_USER = {MYSQL_USER}
MYSQL_PASSWORD = {MYSQL_PASSWORD}
MYSQL_HOST = {MYSQL_HOST}
```
<br>


> <b>Run Docker-compose </b>

```
docker-compose up —build
```

## 🗂 Submodule Directories
<details>
<summary> FRONTEND </summary>

 ```sh
 
📦frontend
 ┣ 📂.github
 ┣ 📂dist
 ┣ 📂node_modules
 ┣ 📂public
 ┣ 📂src
 ┃ ┣ 📂components
 ┃ ┃ ┣ 📜Cropchart.tsx
 ┃ ┃ ┣ 📜DetailModalscreen.tsx
 ┃ ┃ ┣ 📜Hamnav.tsx
 ┃ ┃ ┣ 📜Historycard.tsx
 ┃ ┃ ┣ 📜LoadingPage.tsx
 ┃ ┃ ┣ 📜LogInPage.tsx
 ┃ ┃ ┣ 📜Longnav.tsx
 ┃ ┃ ┣ 📜Navbar.tsx
 ┃ ┃ ┣ 📜Periodchart.tsx
 ┃ ┃ ┣ 📜Periodline.tsx
 ┃ ┃ ┗ 📜SignupPage.tsx
 ┃ ┣ 📂fonts
 ┃ ┣ 📂images
 ┃ ┣ 📂pages
 ┃ ┃ ┣ 📜AbnomalResultPage.tsx
 ┃ ┃ ┣ 📜GetStart.tsx
 ┃ ┃ ┣ 📜HistoryPage.tsx
 ┃ ┃ ┣ 📜MainPage.tsx
 ┃ ┃ ┣ 📜NomalResultPage.tsx
 ┃ ┃ ┗ 📜StasticsPage.tsx
 ┃ ┣ 📂utils
 ┃ ┣ 📜App.css
 ┃ ┣ 📜App.tsx
 ┃ ┣ 📜Cookie.ts
 ┃ ┣ 📜index.css
 ┃ ┣ 📜main.tsx
 ┃ ┣ 📜media.css
 ┃ ┗ 📜vite-env.d.ts
 ┣ 📜.dockerignore
 ┣ 📜.git
 ┣ 📜.gitignore
 ┣ 📜Dockerfile
 ┣ 📜README.md
 ┣ 📜index.html
 ┣ 📜index.tsx
 ┣ 📜package-lock.json
 ┣ 📜package.json
 ┣ 📜postcss.config.cjs
 ┣ 📜tailwind.config.cjs
 ┣ 📜tsconfig.json
 ┣ 📜tsconfig.node.json
 ┗ 📜vite.config.ts
```

</details>


<details>
<summary> BACKEND </summary>

 ```sh
📦backend
 ┣ 📂.github
 ┣ 📂backend
 ┃ ┣ 📜__init__.py
 ┃ ┣ 📜asgi.py
 ┃ ┣ 📜celery.py
 ┃ ┣ 📜settings.py
 ┃ ┣ 📜urls.py
 ┃ ┗ 📜wsgi.py
 ┣ 📂members
 ┃ ┣ 📂migrations
 ┃ ┣ 📜__init__.py
 ┃ ┣ 📜admin.py
 ┃ ┣ 📜apps.py
 ┃ ┣ 📜models.py
 ┃ ┣ 📜serializer.py
 ┃ ┣ 📜tests.py
 ┃ ┣ 📜urls.py
 ┃ ┗ 📜views.py
 ┣ 📂plants
 ┃ ┣ 📂inference
 ┃ ┃ ┣ 📂models
 ┃ ┃ ┃ ┣ 📂hub
 ┃ ┃ ┃ ┣ 📂segment
 ┃ ┃ ┃ ┣ 📜__init__.py
 ┃ ┃ ┃ ┣ 📜common.py
 ┃ ┃ ┃ ┣ 📜experimental.py
 ┃ ┃ ┃ ┣ 📜tf.py
 ┃ ┃ ┃ ┣ 📜yolo.py
 ┃ ┃ ┃ ┣ 📜yolov5l.yaml
 ┃ ┃ ┃ ┣ 📜yolov5m.yaml
 ┃ ┃ ┃ ┣ 📜yolov5n.yaml
 ┃ ┃ ┃ ┣ 📜yolov5s.yaml
 ┃ ┃ ┃ ┗ 📜yolov5x.yaml
 ┃ ┃ ┣ 📂utils
 ┃ ┃ ┃ ┣ 📜__init__.py
 ┃ ┃ ┃ ┣ 📜activations.py
 ┃ ┃ ┃ ┣ 📜augmentations.py
 ┃ ┃ ┃ ┣ 📜autoanchor.py
 ┃ ┃ ┃ ┣ 📜autobatch.py
 ┃ ┃ ┃ ┣ 📜callbacks.py
 ┃ ┃ ┃ ┣ 📜dataloaders.py
 ┃ ┃ ┃ ┣ 📜downloads.py
 ┃ ┃ ┃ ┣ 📜general.py
 ┃ ┃ ┃ ┣ 📜loss.py
 ┃ ┃ ┃ ┣ 📜metrics.py
 ┃ ┃ ┃ ┣ 📜plots.py
 ┃ ┃ ┃ ┣ 📜torch_utils.py
 ┃ ┃ ┃ ┗ 📜triton.py
 ┃ ┃ ┣ 📜cucumber.pt
 ┃ ┃ ┣ 📜detect.py
 ┃ ┃ ┣ 📜export.py
 ┃ ┃ ┣ 📜grape.pt
 ┃ ┃ ┣ 📜paprika.pt
 ┃ ┃ ┣ 📜pepper.pt
 ┃ ┃ ┣ 📜strawberry.pt
 ┃ ┃ ┗ 📜tomato.pt
 ┃ ┣ 📂migrations
 ┃ ┣ 📜__init__.py
 ┃ ┣ 📜admin.py
 ┃ ┣ 📜apps.py
 ┃ ┣ 📜models.py
 ┃ ┣ 📜serializer.py
 ┃ ┣ 📜storagess.py
 ┃ ┣ 📜tasks.py
 ┃ ┣ 📜tests.py
 ┃ ┣ 📜urls.py
 ┃ ┗ 📜views.py
 ┣ 📂static
 ┣ 📜.env
 ┣ 📜.git
 ┣ 📜.gitignore
 ┣ 📜Dockerfile
 ┣ 📜README.md
 ┣ 📜manage.py
 ┗ 📜requirements.txt
```

</details>

## Flowchart

![flowchart_en drawio](https://user-images.githubusercontent.com/84130518/216247179-88d776e2-2cdd-419a-b0a0-bdfd28778dae.png)

## 🔍 Features

**SignUp / Login page**

<img  src="https://user-images.githubusercontent.com/97827316/215984078-3cbe440e-c4bc-4ae3-9a2b-662ec2dae079.gif">

- This is a SignUp / Login page using JWT token.

<br>
<br>

**Diagnostic/Diagnostic Results Page**

<img src="https://user-images.githubusercontent.com/97827316/215984379-20db97b3-e90c-4857-bb46-c457b61b632c.gif">

- It is a page that selects an image of a disease crop and diagnoses it with AI, and if it is a disease crop, it provides causes and solutions together.

<br>

**history / history delete**

<img src="https://user-images.githubusercontent.com/97827316/215984492-50f4e265-a738-41a9-8463-532ddb453c68.gif">

- With a function that is only available when logging in, you can collect crops that you have diagnosed by category.
- You can check the detailed information of the selected crop and delete it.

<br>

**Staticstics Page**

![2A005C2A-E092-4315-8DE9-7F42D3C72641](https://user-images.githubusercontent.com/84130518/216145065-275acbcd-2fed-48f2-839c-69294a5dc8e1.gif)

- Statistics are shown based on Cropdoctor diagnostic data.
- Statistics on the number of diseases by crop
  - It provides information on which diseases each crop has a lot in the form of a bar chart.
- Monthly Disease Count Statistics
  - The crops selected in the category are provided in the form of a line graph of how the disease flows per month.


**Responsive Web Pages**

![반응형](https://user-images.githubusercontent.com/84130518/216141786-cdafcb67-0af9-49cb-9e2c-005e14bac7b2.gif)

## AI
AI used YoloV5, and the Precision-Confidence Curve and learning process and performance are as follows.
![그림1](https://user-images.githubusercontent.com/84130518/216386440-c240d681-2f4f-4121-b6da-d630e2d30dbd.png)

![results (1)](https://user-images.githubusercontent.com/84130518/216386411-f00c4c4b-2ebb-49bb-a4fd-82dd63aa1094.png)

The following photos are actually analyzed by AI.
![Group 101111](https://user-images.githubusercontent.com/84130518/216389881-90366a8a-afff-4122-8025-f135ce9fa37a.png)

## 🖥️ Moniterings

<br>

**Kibana Dashboard**

<img src="https://user-images.githubusercontent.com/84130518/216140964-6ae6f082-1a31-4348-8d38-39087ab98a94.png">

<br>

**Grafana Dashboard & Slack Alert**

<img  src="https://user-images.githubusercontent.com/84130518/216139014-d7f93579-66dc-4ec5-8e1e-664fa5258372.png">

<br>

If the storage capacity exceeds 85%, Grafana sends an alarm to Slack.

<img width="320" src="https://user-images.githubusercontent.com/83527046/216155592-6f85fc7f-b30a-426e-bdc5-86cdeb763663.png">
<br>


## Swagger

The use of Swagger for API documentation for Frontend and Backend communication.
<img width="1245" alt="스크린샷 2023-02-01 오후 6 03 44 (1)" src="https://user-images.githubusercontent.com/84130518/216385471-3b8f5d95-b9ca-4705-88df-0426ddba2d8d.png">


## 👥 Our Team

<table width="1000">
    <thead>
    </thead>
    <tbody>
    <tr>
        <th>Pictures</th>
         <td width="100" align="center">
            <a href="https://github.com/goldapple-ce">
                <img src="https://user-images.githubusercontent.com/97827316/215991540-bd09f520-794d-4db2-9bde-955470a96957.png" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/jiyoon0701">
                <img  src="https://user-images.githubusercontent.com/97827316/215991531-8da89dd4-d739-4e37-b5be-2b04c38ec6f3.png" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/TMInstaller">
                <img src="https://user-images.githubusercontent.com/97827316/215991528-8c8a4e08-16ef-46e2-a996-e3a60b937cc3.png" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/yura0302">
                <img src="https://user-images.githubusercontent.com/97827316/215991544-021c3e7a-460b-41a3-a030-2dca6bb0ac20.png" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/fnzl54">
                <img src="https://user-images.githubusercontent.com/97827316/215991516-914ed25d-6759-4478-843c-628a0c6baad1.png" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/hstla">
                <img src="https://user-images.githubusercontent.com/97827316/215991535-aa0d5aeb-363c-41a7-a114-c1448d58d9f1.png" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/Mayreeel">
                <img src="https://user-images.githubusercontent.com/97827316/215991527-9226b9b3-34fa-493b-b2af-c61d15cc13cf.png" width="60" height="60">
            </a>
        </td>
    </tr>
    <tr>
        <th>Name</th>
        <td width="100" align="center">강용민</td>
        <td width="100" align="center">이지윤</td>
        <td width="100" align="center">백동열</td>
        <td width="100" align="center">김유라</td>
        <td width="100" align="center">권찬영</td>
        <td width="100" align="center">황현성</td>
        <td width="100" align="center">이규현</td>
    </tr>
    <tr>
        <th>Position</th>
        <td width="150" align="center">
            Backend<br>
            DevOps<br>
        </td>
        <td width="150" align="center">
            Frontend<br>
            Backend<br>
            DevOps<br>
        </td>
        <td width="150" align="center">
            Frontend<br>
            Backend<br>
        </td>
        <td width="150" align="center">
            Frontend<br>
        </td>
        <td width="150" align="center">
            Backend<br>
            DevOps<br>
            AI<br>
        </td>
        <td width="150" align="center">
            Backend<br>
            DevOps<br>
        </td>
        <td width="150" align="center">
            Frontend<br>
        </td>
    </tr>
    <tr>
        <th>GitHub</th>
        <td width="100" align="center">
            <a href="https://github.com/goldapple-ce">
                <img src="http://img.shields.io/badge/Kyoungmin1016-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/jiyoon0701">
                <img src="http://img.shields.io/badge/jiyoon0701-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/TMInstaller">
                <img src="http://img.shields.io/badge/TMInstaller-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/yura0302">
                <img src="http://img.shields.io/badge/yura0302-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/fnzl54">
                <img src="http://img.shields.io/badge/fnzl54-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/hstla">
                <img src="http://img.shields.io/badge/hstla-green?style=social&logo=github"/>
            </a>
        </td>
         <td width="100" align="center">
            <a href="https://github.com/Mayreeel">
                <img src="http://img.shields.io/badge/Mayreeel-green?style=social&logo=github"/>
            </a>
        </td>
     </tr>
    </tbody>
</table>
