---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% comment %} 
  自动判断使用 CDN 还是 Raw 链接 
  注意：这里的 @google-scholar-stats 是因为你的 YML 把数据推到了这个特定分支
{% endcomment %}

{% if site.google_scholar_stats_use_cdn %}
  {% assign base_path = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@google-scholar-stats/" %}
{% else %}
  {% assign base_path = "https://raw.githubusercontent.com/" | append: site.repository | append: "/google-scholar-stats/" %}
{% endif %}

{% comment %} 
  注意：
  1. 你的 YML 脚本里，git init 是在 results 文件夹内部执行的。
  2. 这意味着推送到分支后，json 文件是在根目录的，而不是在 results/ 目录下。
  3. 所以这里不需要再加 "results/" 前缀。
{% endcomment %}

{% assign gs_url = base_path | append: "gs_data_shieldsio.json" %}
{% assign scopus_url = base_path | append: "scopus_data_shieldsio.json" %}
<div class='paper-box-text' markdown="1">

<span class='anchor' id='about-me'></span>

本人现于华中科技大学人工智能与自动化学院智能科学与技术专业攻读博士学位，师从李炜教授。<a href='https://scholar.google.com/citations?user=pj7fXtgAAAAJ&hl=zh-CN'><img src="https://img.shields.io/endpoint?url={{ gs_url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=谷歌学术引用"></a><a href='https://www.scopus.com/authid/detail.uri?authorId=59208226300'>
  <img src="https://img.shields.io/endpoint?url={{ scopus_url | url_encode }}&logo=scopus&labelColor=f6f6f6&color=orange&style=flat&label=Scopus引用">
</a>


我的研究兴趣包括
- *宽度学习系统*
- *深度学习*
- *统计分析与预测*
- *自然语言处理* 

本人帮朋友整理的《863概率论与数理统计》考研复习资料(*有些许错误*) [[下载]](/pdf/概率论与数理统计.pdf)


<span class='anchor' id='-xljy'></span>

# 🎓 学历学位
- *2025.09 - 现在*, <a href="http://www.hust.edu.cn/"><img class="jpg" src="/images/HUST.jpg" width="23pt"></a> [华中科技大学人工智能与自动化学院](https://aia.hust.edu.cn/), 智能科学与技术, 博士, 工学博士
- *2022.09 - 2025.06*, <a href="http://www.qdu.edu.cn/"><img class="jpg" src="/images/qdu.jpg" width="23pt"></a> [青岛大学自动化学院](http://zdh.qdu.edu.cn/), 系统科学, 硕士, 理学硕士
- *2017.09 - 2021.06*, <a href="https://www.ahau.edu.cn/"><img class="jpg" src="/images/ahau.jpg" width="23pt"></a> [安徽农业大学工学院](http://gxy.ahau.edu.cn/), 车辆工程, 本科, 工学学士

<span class='anchor' id='-news'></span>

# 🔥 最新消息
- *2026.03*: 🔥🔥我们的论文“Maximum total correntropy-based broad learning system with robust M-estimator”被Neural Networks录用 [[链接]](https://doi.org/10.1016/j.neunet.2026.108917).
- *2025.11*: 🔥🔥我们的论文“Sparse Bayesian Broad Learning System via Adaptive Lasso Priors for Robust Regression”被IEEE TRANSACTIONS ON NEURAL NETWORKS AND LEARNING SYSTEMS录用 [[链接]](https://doi.org/10.1109/TNNLS.2025.3630247).
- *2025.06*: 🔥🔥获评青岛大学2025年优秀硕士学位论文 [[获奖证书]](/images/qduyouxiuxueweilunwen.jpg).

<span class='anchor' id='-kyxm'></span>

# 📚 科研项目
- *2020.04 - 2021.04*, 安徽农业大学第五期“优才计划”学生发展支持项目, XSZZ202006, 新能源汽车销量、股票市场波动及民意调查分析, 主持, [[通知]](http://xszz.ahau.edu.cn/info/1013/1793.htm)或[[名单]](/Excel/安徽农业大学2020年第五期“优才计划”项目拟立项名单.xls).

<span class='anchor' id='-lwzl'></span>

# 📝 学术著作
### 学位论文
---
-  **陈滔**. 基于稀疏贝叶斯宽度学习系统的回归预测方法研究[D]. 青岛: *青岛大学*, 2025. [[链接]](https://kns.cnki.net/kcms2/article/abstract?v=ZBmzy5eCHca5gFH7bvCSIohm5jtvbeEssetopRE781cHD9s0thglqpX5pGQQABJIW0z98mAN0NnvxcTHUCdohOgEViva6B8IcHbbl3MwnMEQ0BqONSs-YiGvEeMjC4HOtZzGDIFofn9s_nPFW6-LzYfYEuN6SHxaCsEzbP0wTOGgXgHjhwH44A==&uniplatform=NZKPT&language=CHS)

### 英文论文
---
- **Chen T**, Chen X, Li W <sup><svg focusable="false" viewBox="0 0 102 128" height="20" title="Author email or social media contact details icon" class="icon icon-envelope react-xocs-author-icon u-fill-grey8"><path d="M55.8 57.2c-1.78 1.31-5.14 1.31-6.9 0L17.58 34h69.54L55.8 57.19zM0 32.42l42.94 32.62c2.64 1.95 6.02 2.93 9.4 2.93s6.78-.98 9.42-2.93L102 34.34V24H0zM92 88.9L73.94 66.16l-8.04 5.95L83.28 94H18.74l18.38-23.12-8.04-5.96L10 88.94V51.36L0 42.9V104h102V44.82l-10 8.46V88.9"></path></svg></sup>. Maximum total correntropy-based broad learning system with robust M-estimator[J]. *Neural Netw.*, 2026, 201: 108917. [[链接]](https://doi.org/10.1016/j.neunet.2026.108917)
  
-  **Chen T**, Wang L J <sup><svg focusable="false" viewBox="0 0 102 128" height="20" title="Author email or social media contact details icon" class="icon icon-envelope react-xocs-author-icon u-fill-grey8"><path d="M55.8 57.2c-1.78 1.31-5.14 1.31-6.9 0L17.58 34h69.54L55.8 57.19zM0 32.42l42.94 32.62c2.64 1.95 6.02 2.93 9.4 2.93s6.78-.98 9.42-2.93L102 34.34V24H0zM92 88.9L73.94 66.16l-8.04 5.95L83.28 94H18.74l18.38-23.12-8.04-5.96L10 88.94V51.36L0 42.9V104h102V44.82l-10 8.46V88.9"></path></svg></sup>, C. L. Philip Chen. Sparse Bayesian broad learning system via adaptive lasso priors for robust regression[J]. *IEEE Trans. Neural Netw. Learn. Syst.*, 2025, Early Access. [[链接]](https://doi.org/10.1109/TNNLS.2025.3630247)

-   **Chen T**, Wang L J <sup><svg focusable="false" viewBox="0 0 102 128" height="20" title="Author email or social media contact details icon" class="icon icon-envelope react-xocs-author-icon u-fill-grey8"><path d="M55.8 57.2c-1.78 1.31-5.14 1.31-6.9 0L17.58 34h69.54L55.8 57.19zM0 32.42l42.94 32.62c2.64 1.95 6.02 2.93 9.4 2.93s6.78-.98 9.42-2.93L102 34.34V24H0zM92 88.9L73.94 66.16l-8.04 5.95L83.28 94H18.74l18.38-23.12-8.04-5.96L10 88.94V51.36L0 42.9V104h102V44.82l-10 8.46V88.9"></path></svg></sup>, Liu Y, et al. Double-kernel based Bayesian approximation broad learning system with dropout[J]. *Neurocomputing*, 2024, 610: 128533.
[[链接]](https://doi.org/10.1016/j.neucom.2024.128533)

-   **Chen T**, Wang L J <sup><svg focusable="false" viewBox="0 0 102 128" height="20" title="Author email or social media contact details icon" class="icon icon-envelope react-xocs-author-icon u-fill-grey8"><path d="M55.8 57.2c-1.78 1.31-5.14 1.31-6.9 0L17.58 34h69.54L55.8 57.19zM0 32.42l42.94 32.62c2.64 1.95 6.02 2.93 9.4 2.93s6.78-.98 9.42-2.93L102 34.34V24H0zM92 88.9L73.94 66.16l-8.04 5.95L83.28 94H18.74l18.38-23.12-8.04-5.96L10 88.94V51.36L0 42.9V104h102V44.82l-10 8.46V88.9"></path></svg></sup>, Liu Y, et al. DACBN: Dual attention convolutional broad network for fine-grained visual recognition[J]. *Pattern Recognit.*, 2024, 156: 110749.
[[链接]](https://doi.org/10.1016/j.patcog.2024.110749)

-  Wang Y J, Wang L J <sup><svg focusable="false" viewBox="0 0 102 128" height="20" title="Author email or social media contact details icon" class="icon icon-envelope react-xocs-author-icon u-fill-grey8"><path d="M55.8 57.2c-1.78 1.31-5.14 1.31-6.9 0L17.58 34h69.54L55.8 57.19zM0 32.42l42.94 32.62c2.64 1.95 6.02 2.93 9.4 2.93s6.78-.98 9.42-2.93L102 34.34V24H0zM92 88.9L73.94 66.16l-8.04 5.95L83.28 94H18.74l18.38-23.12-8.04-5.96L10 88.94V51.36L0 42.9V104h102V44.82l-10 8.46V88.9"></path></svg></sup>, **Chen T**. Broad learning system via adaptive maximum weighted correntropy[J]. *Neural Netw.*, 2026, 193: 108032. [[链接]](https://doi.org/10.1016/j.neunet.2025.108032)

### 中文论文
---
-	**陈滔**, 王立杰 <sup><svg focusable="false" viewBox="0 0 102 128" height="20" title="Author email or social media contact details icon" class="icon icon-envelope react-xocs-author-icon u-fill-grey8"><path d="M55.8 57.2c-1.78 1.31-5.14 1.31-6.9 0L17.58 34h69.54L55.8 57.19zM0 32.42l42.94 32.62c2.64 1.95 6.02 2.93 9.4 2.93s6.78-.98 9.42-2.93L102 34.34V24H0zM92 88.9L73.94 66.16l-8.04 5.95L83.28 94H18.74l18.38-23.12-8.04-5.96L10 88.94V51.36L0 42.9V104h102V44.82l-10 8.46V88.9"></path></svg></sup>, 刘洋, 等. 带有Dropout结构的贝叶斯近似宽度学习系统[J]. *控制理论与应用*, 2025, 42(8): 1632-1640. [[链接]](https://dx.doi.org/10.7641/CTA.2024.30087) 

*[注释]: ### 专利著作
*[注释]: ---
*[注释]: - 测试,***测试***. 专利名. [[网页]]()

**<svg focusable="false" viewBox="0 0 102 128" height="20" title="Author email or social media contact details icon" class="icon icon-envelope react-xocs-author-icon u-fill-grey8"><path d="M55.8 57.2c-1.78 1.31-5.14 1.31-6.9 0L17.58 34h69.54L55.8 57.19zM0 32.42l42.94 32.62c2.64 1.95 6.02 2.93 9.4 2.93s6.78-.98 9.42-2.93L102 34.34V24H0zM92 88.9L73.94 66.16l-8.04 5.95L83.28 94H18.74l18.38-23.12-8.04-5.96L10 88.94V51.36L0 42.9V104h102V44.82l-10 8.46V88.9"></path></svg>：通信作者.**
<span class='anchor' id='-ryjx'></span>

# 📖 荣誉奖项
- *2025年* 获得 青岛大学优秀硕士学位论文 [[获奖证书]](/images/qduyouxiuxueweilunwen.jpg).
- *2024年* 获得 研究生国家奖学金（硕士）[[获奖证书]](/images/guojiang.jpg)、青岛大学2024年夏季学期第三届研究生创新成果展**优秀学术创新成果奖**等.
- *2022年* 获得 山东省研究生“AI+"创新实践大赛**二等奖**.
- *2020年* 获得 第十八届“SuperMap"杯GIS大赛**二等奖**、第十届全国大学生市场调查与分析大赛**三等奖**及安徽赛区**一等奖**、安徽省计算机博弈大赛**一等奖**等.
- *2019年* 获得 第九届全国大学生市场调查与分析大赛**三等奖**及安徽赛区**一等奖**、安徽省大学生统计建模大赛研究生组**三等奖**等.
  
<span class='anchor' id='-xshy'></span>

# 🏭 论坛会议
- *2024.07*, 青岛大学2024年夏季学期第三届研究生创新成果展, 青岛.
- *2024.05*, 第八届中国系统科学大会, 芜湖.
- *2023.05*, 青岛大学“求实创新, 研学笃行”2023年度研究生学术沙龙, 青岛. [[通知]](https://mp.weixin.qq.com/s/iDcZ8NttA1ifqcynNizpSg)

<span class='anchor' id='-gzsx'></span>

# 💻 工作实习
- *2022.11 - 2023.06*, 《武汉大学学报工学版》编辑部, **实习编辑**
- *2021.05 - 2021.08*, 合肥小路数据信息技术有限公司,  **云计算工程师**

---

<span class='anchor' id='-xxly'></span>
# 💬️ 消息留言
<script src="https://giscus.app/client.js"
        data-repo="supersahau/zh-cn"
        data-repo-id="R_kgDOHjFR3A"
        data-category="Q&A"
        data-category-id="DIC_kwDOHjFR3M4CsW4q"
        data-mapping="pathname"
        data-strict="0"
        data-reactions-enabled="0"
        data-emit-metadata="0"
        data-input-position="top"
        data-theme="light"
        data-lang="zh-CN"
        crossorigin="anonymous"
        async>
</script>

  
</div>

