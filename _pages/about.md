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

<span class='anchor' id='about-me'></span>

My name is Jiahe Chen, and I am currently a senior student at Zhejiang University of Technology. Soon, I will begin my journey as a Ph.D. at the College of Computer Science and Technology, Zhejiang University.

My research interest includes Machine Learning and computer vision. 

And I work really closely with [Qiyuan Chen](https://qychen2001.github.io/), [Qian Shao](https://abeier87.github.io/), [Jiahe Ying]().

<font color="red">
<span id="lastCommitTime"></span>
</font>

# 🔥 News

- 2024.10, I am honored to have been awarded the National Scholarship.
- 2024.07, One paper is accepted by ECAI 2024.

# 📝 Publications 

- Decoupled Competitive Framework for Semi-supervised medical segmentation. **Jiahe Chen**, Jiahe Ying, Shen Wang, Jianwei Zheng; ECAI 2024. (CCF-B)

# 💻 Projects
## 1、[LLM Application Platform @ Wedoctor Inc.]() (Frontend Developer)

**Introduction:** This is a LLMs application and development platform, designed to help downstream engineers better compare and use LLMs. It includes model square, knowledge square, comparison center, document center, etc.

In this project, I completed the development of all front-end pages and interactions with [Qiyuan Chen](https://qychen2001.github.io/).


<!-- # 🎖 Honors and Awards -->

# 📖 Educations

- *2025.09 - 2030.06 (expected)*, Ph.D. in Computer Science and Technology, [College of Computer Science and Technology](http://www.cs.zju.edu.cn/), Zhejiang University.

- *2021.09 - 2025.06 (expected)*, B.S. in Software Engineer, [School of Computer Science and Technology](https://cs.zjut.edu.cn/jsp/index.jsp), Zhejiang University of Technology. Advised by Prof. [Jianwei Zheng](https://homepage.zjut.edu.cn/zjw/). Many thanks to Prof. [Jianwei Zheng](https://homepage.zjut.edu.cn/zjw/) for my academic enlightenment and guidance.


<div align="center">
<script async src="//busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js"></script>
This homepage is visited <font color="purple" size="5"><span id="busuanzi_value_site_pv"></span></font> times
</div>

<div>

<script>
async function fetchLastCommitTime() {

  // https://github.com/JiaheChen2002/JiaheChen2002.github.io
    const owner = 'JiaheChen2002';
    const repo = 'JiaheChen2002.github.io';
    const url = `https://api.github.com/repos/${owner}/${repo}/commits`;
    try {
        const response = await fetch(url);
        if (!response.ok) {
            throw new Error(`Failed to fetch data from GitHub: ${response.statusText}`);
        }
        const data = await response.json();
        const lastCommitDate = new Date(data[0].commit.committer.date);
        document.getElementById('lastCommitTime').textContent = `Last Updated in ${lastCommitDate.toLocaleDateString()}`;
    } catch (error) {
        console.error('Error fetching commit time:', error);
        // document.getElementById('lastCommitTime').textContent = 'Failed to fetch commit time.';
    }
}
fetchLastCommitTime();
</script>
</div>