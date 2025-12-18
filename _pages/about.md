---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<style>
  .centered {
    text-align: center;
    font-size: 24px;
    background: linear-gradient(to right, #81c784, #ff6b6b); /* 西瓜绿到西瓜红的渐变色 */
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
   .intro {
    margin-top: 50px; /* 调整分割线顶部间距 */
    padding-top: 50px; /* 调整分割线底部间距 */
    border-top: 2px solid #ccc; /* 分割线样式 */
  }
  .image-container {
    display: flex;
    justify-content: flex-start; /* 左对齐 */
    align-items: center; /* 垂直居中 */
    margin-bottom: 20px; /* 可选：设置下方间距 */
  }
  .image-container img {
    margin: 30px; /* 可选：设置图片之间的间距 */
  }
    .skill-container {
    max-width: 800px;
    margin: 10 auto;
    background-color: #ddd;
    padding: 20px; /* 设置内边距 */
    border-radius: 10px; /* 圆角 */
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* 阴影 */
}
</style>
<div class="centered">
  <h2>Hi, I am Shaobin</h2>
</div>

I am currently pursuing my master's degree at [Fudan University](https://www.fudan.edu.cn/en/) under the supervision of Professor [Yang Chen](https://chenyang03.wordpress.com/). Prior to this, I earned my Bachelor's degree from the School of Cyber Science and Engineering at [Zhengzhou University](https://english.zzu.edu.cn/) in 2023.

Since September 2023, I have been involved in research at the School of Computer Science at Fudan University, with a focus on network systems and social network.

# 📄 Publications

Energy-Aware Collaborative Perception in HetVNETs: Balancing Accuracy and Sustainability.  
Mengying Zhou, **Shaobin Wang**, Qiang Duan, Aaron Yi Ding, Xin Wang\*, Yang Chen\*.  
To appear: IEEE Communications Magazine.

---

Understanding Cross-Platform Links in User Profiles: A Data-Driven Analysis on Mastodon.  
Shaojie Min, **Shaobin Wang**, Yaxiao Luo, Qingyuan Gong\*, Yang Chen\*.  
Proc. of the 10th China National Conference on Big Data and Social Computing (BDSC’25), Kunming, China, Aug. 2025.(Most Welcomed Paper Award)

---

FediLive: A Framework for Collecting and Preprocessing Snapshots of Decentralized Online Social Networks.  
Shaojie Min#, **Shaobin Wang#**, Yaxiao Luo, Min Gao, Qingyuan Gong\*, Yu Xiao, Yang Chen\*.  
***Proc. of the Web Conference (WWW’25), Resource Track, Sydney, Australia, Apr.-May 2025.***  

---

Towards the Predictability of IPFS Nodes’ Session Time Using Machine Learning.  
Dan Zhuo, Jiawei Tang, Yang Chen\*, **Shaobin Wang**, Xin Wang.  
***Proc. of Turing Award Celebration Conference (TURC'23), Poster, Wuhan, China, July 2023.***  
[Detail]((https://dl.acm.org/doi/10.1145/3603165.3607397)  )

---

# 🛠️ Projects

### Community Building Assistant（社造助理） - WeChat Mini Program (2023 - Present)

**Project Description**:    
Social Assistant is a WeChat mini program designed to help elderly residents in communities by allowing them to initiate help requests. Community staff and volunteers can view and respond to these requests, providing assistance. The program also allows for the recording of these activities, helping to build a supportive community.  

**Responsibilities**:  
- Developed the WeChat Mini Program for elderly residents to request help and for volunteers to respond.  
- Designed the backend API using Node.js and MongoDB to manage user data, activity logs, and help requests.  
- Built web-based tools for viewing, modifying, and exporting activity data.  

**Tech Stack**:  
- **Frontend**: WeChat Mini Program, HTML, CSS, JavaScript  
- **Backend**: Node.js, Express, MongoDB  
- **Other**: Python (for exporting data to Excel), Multer (for file uploads)  

---

### Intelligent Mine Inspection Solution - Project Leader (March 2021 - June 2021)

**Project Description**:    
This project consists of components such as STM32, Raspberry Pi, robotic arms, and servos, and is designed to replace manual inspection in hazardous areas like mines. It deploys LoRa gateways for communication and detects whether workers are wearing safety helmets.  

**Responsibilities**:  
- Led the development of the safety helmet detection algorithm on the Raspberry Pi using YOLOv5 for training the dataset.  

**Results**:  
- Awarded 3rd place in the National Finals of the 2021 IoT Design Competition (Huawei Cup).  
- Won 2nd place in the Central China Region of the 2021 Network Technology Challenge.  

**Tech Stack**:  
- **Programming Languages**: Python  
- **Machine Learning**: PyTorch, YOLOv5  

---

# 🎓 Education

- **Graduate Student of Computer Science (Sep.2023 - now)**

<div style="display: flex; align-items: center;">
    <img src="../images/Fudan_University_Logo.svg.png" alt="fdu" width="100" height="100" style="margin-right: 2ch;">
    <div>
        <blockquote>
             Fudan University<br>
             School of Computer Science Fudan University
        </blockquote>
    </div>
</div>

- **Undergraduate Student of Internet of Things Engineering (Sep. 2019 - Jun. 2023)**

<div style="display: flex; align-items: center;">
    <img src="../images/zzulogo.png" alt="fdu" width="100" height="100" style="margin-right: 2ch;">
    <div>
        <blockquote>
            Zhengzhou University<br>
            School of Cyber Science and Engineering
        </blockquote>
    </div>
</div>



# 🏆 Honors and Awards

<ul>
  <li>Third Class Academic Scholarship, School of Cyber Science and Engineering, Zhengzhou University, 2023</li>
  <li>Outstanding Cadre of the Communist Youth League, Zhengzhou University, 2020</li>
</ul>
