<style>
.lang-toggle {
  display: flex;
  justify-content: flex-end;
  gap: 8px;
  margin: 8px 0 20px;
}

.lang-btn {
  border: 1px solid #0b5cab;
  background: #fff;
  color: #0b5cab;
  border-radius: 999px;
  padding: 6px 14px;
  font-size: 0.9rem;
  cursor: pointer;
  transition: all 0.2s ease;
}

.lang-btn.active,
.lang-btn:hover {
  background: #0b5cab;
  color: #fff;
}

.academic-home {
  max-width: 980px;
  margin: 0 auto;
}

.hero {
  background: linear-gradient(120deg, #f7fbff 0%, #ecf3ff 100%);
  border: 1px solid #dbe8ff;
  border-radius: 14px;
  padding: 24px;
  margin-bottom: 20px;
}

.hero h1 {
  margin: 0 0 8px;
  font-size: 2rem;
}

.hero p {
  margin: 8px 0;
  line-height: 1.7;
}

.tag-list {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 12px;
}

.tag {
  background: #0b5cab;
  color: #fff;
  border-radius: 999px;
  padding: 4px 10px;
  font-size: 0.82rem;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 16px;
}

.card {
  background: #fff;
  border: 1px solid #e6e9ef;
  border-radius: 12px;
  padding: 18px;
  box-shadow: 0 2px 10px rgba(15, 23, 42, 0.04);
}

.card h2 {
  margin-top: 0;
  margin-bottom: 12px;
  font-size: 1.2rem;
  border-left: 4px solid #0b5cab;
  padding-left: 10px;
}

.card ul {
  margin: 0;
  padding-left: 20px;
}

.card li {
  margin-bottom: 8px;
  line-height: 1.65;
}

.publications {
  margin-top: 16px;
}

.pub-group h3 {
  margin-top: 0;
  margin-bottom: 10px;
  color: #0f172a;
}

.pub-group li {
  margin-bottom: 10px;
}

.footer-note {
  margin-top: 20px;
  padding: 12px 14px;
  border-left: 4px solid #0b5cab;
  background: #f8fbff;
  color: #334155;
}

[data-lang] {
  display: none;
}

[data-lang].visible {
  display: block;
}
</style>

<div class="academic-home">
  <div class="lang-toggle">
    <button class="lang-btn active" id="btn-en" onclick="setLang('en')">English</button>
    <button class="lang-btn" id="btn-zh" onclick="setLang('zh')">中文</button>
  </div>

  <section class="hero">
    <div data-lang="en" class="visible">
      <h1>Jiangyu Lan</h1>
      <p>PhD Student, Information and Communication Engineering, Beijing Jiaotong University.</p>
      <p>
        Welcome to my academic homepage. My research focuses on UAV networking,
        future networking architectures, and robot motion planning. I am interested
        in bridging theoretical network design with practical intelligent systems.
      </p>
      <div class="tag-list">
        <span class="tag">UAV Networks</span>
        <span class="tag">Future Network</span>
        <span class="tag">Robot Motion Planning</span>
      </div>
    </div>

    <div data-lang="zh">
      <h1>兰江雨</h1>
      <p>北京交通大学 信息与通信工程博士研究生。</p>
      <p>
        欢迎访问我的学术主页。我的研究方向聚焦于无人机网络、未来网络架构与机器人运动规划，
        致力于将网络理论设计与智能系统工程实践相结合。
      </p>
      <div class="tag-list">
        <span class="tag">无人机网络</span>
        <span class="tag">未来网络</span>
        <span class="tag">机器人运动规划</span>
      </div>
    </div>
  </section>

  <section class="grid">
    <article class="card">
      <div data-lang="en" class="visible">
        <h2>Education</h2>
        <ul>
          <li><strong>2022.09 – Present</strong><br/>PhD, Information and Communication Engineering, Beijing Jiaotong University</li>
          <li><strong>2018.09 – 2021.06</strong><br/>MEng, Electronics and Communication Engineering, Beijing Information Science & Technology University</li>
          <li><strong>2014.09 – 2018.06</strong><br/>BEng, Communication Engineering, Beijing Information Science & Technology University</li>
        </ul>
      </div>
      <div data-lang="zh">
        <h2>教育经历</h2>
        <ul>
          <li><strong>2022.09 – 至今</strong><br/>北京交通大学，信息与通信工程，博士</li>
          <li><strong>2018.09 – 2021.06</strong><br/>北京信息科技大学，电子与通信工程，硕士</li>
          <li><strong>2014.09 – 2018.06</strong><br/>北京信息科技大学，通信工程，学士</li>
        </ul>
      </div>
    </article>

    <article class="card">
      <div data-lang="en" class="visible">
        <h2>Experience</h2>
        <ul>
          <li><strong>2021.07 – 2022.07</strong><br/>Network Engineer, China Telecom</li>
        </ul>
      </div>
      <div data-lang="zh">
        <h2>工作经历</h2>
        <ul>
          <li><strong>2021.07 – 2022.07</strong><br/>中国电信，网络工程师</li>
        </ul>
      </div>
    </article>
  </section>

  <section class="card publications">
    <div data-lang="en" class="visible">
      <h2>Selected Publications</h2>
      <div class="pub-group">
        <h3>English</h3>
        <ul>
          <li><strong>Jiangyu Lan</strong>, Shuai Gao, Weiting Zhang, Xindu Hou, Minghui Xi, Yuming Zhang, Bo Lei, Hongke Zhang, and Xuemin (Sherman) Shen. OpenL3: Embedding Diverse Network Services Into MANETs Using Multi-Dimensional Identifier. <em>IEEE Internet of Things Journal</em>, 2025.</li>
          <li>Qianru Ma, Shuai Gao, Minghui Xi, and <strong>Jiangyu Lan</strong>. A Multi-Dimensional Identifier-Based Routing Mechanism for Flying Ad-Hoc Networks. In <em>ICCCS 2024</em>, pp. 691-697.</li>
          <li><strong>Jiangyu Lan</strong>, Yinggang Xie, Guangjun Liu, and Manxin Cao. A Multi-Objective Trajectory Planning Method for Collaborative Robot. <em>Electronics</em>, 2020, 9, 859.</li>
        </ul>
      </div>
      <div class="pub-group">
        <h3>Chinese</h3>
        <ul>
          <li>席铭辉，郜帅，<strong>兰江雨</strong>，侯心迪. 一种无人机自组网中基于身份加密的认证方案. 计算机技术与发展, 2024.</li>
          <li>柴若楠，郜帅，<strong>兰江雨</strong>，刘宁春. 算力网络中高效算力资源度量方法. 计算机研究与发展, 2023.</li>
          <li>解迎刚，<strong>兰江雨</strong>. 协作机器人及其运动规划方法研究综述. 计算机工程与应用, 2021.</li>
        </ul>
      </div>
      <p><strong>Full list:</strong> <a href="https://scholar.google.com/citations?user=sa89XfwAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a></p>
    </div>

    <div data-lang="zh">
      <h2>代表性成果</h2>
      <div class="pub-group">
        <h3>英文论文</h3>
        <ul>
          <li><strong>Jiangyu Lan</strong>, Shuai Gao, Weiting Zhang, Xindu Hou, Minghui Xi, Yuming Zhang, Bo Lei, Hongke Zhang, and Xuemin (Sherman) Shen. OpenL3: Embedding Diverse Network Services Into MANETs Using Multi-Dimensional Identifier. <em>IEEE Internet of Things Journal</em>, 2025.</li>
          <li>Qianru Ma, Shuai Gao, Minghui Xi, and <strong>Jiangyu Lan</strong>. A Multi-Dimensional Identifier-Based Routing Mechanism for Flying Ad-Hoc Networks. In <em>ICCCS 2024</em>, pp. 691-697.</li>
          <li><strong>Jiangyu Lan</strong>, Yinggang Xie, Guangjun Liu, and Manxin Cao. A Multi-Objective Trajectory Planning Method for Collaborative Robot. <em>Electronics</em>, 2020, 9, 859.</li>
        </ul>
      </div>
      <div class="pub-group">
        <h3>中文论文</h3>
        <ul>
          <li>席铭辉，郜帅，<strong>兰江雨</strong>，侯心迪. 一种无人机自组网中基于身份加密的认证方案. 计算机技术与发展, 2024.</li>
          <li>柴若楠，郜帅，<strong>兰江雨</strong>，刘宁春. 算力网络中高效算力资源度量方法. 计算机研究与发展, 2023.</li>
          <li>解迎刚，<strong>兰江雨</strong>. 协作机器人及其运动规划方法研究综述. 计算机工程与应用, 2021.</li>
        </ul>
      </div>
      <p><strong>完整列表：</strong><a href="https://scholar.google.com/citations?user=sa89XfwAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a></p>
    </div>
  </section>

  <div class="footer-note">
    <span data-lang="en" class="visible">If you are interested in collaboration opportunities, feel free to reach out.</span>
    <span data-lang="zh">如果您对学术合作感兴趣，欢迎与我联系。</span>
  </div>
</div>

<script>
  function setLang(lang) {
    document.querySelectorAll('[data-lang]').forEach((el) => {
      if (el.getAttribute('data-lang') === lang) {
        el.classList.add('visible');
      } else {
        el.classList.remove('visible');
      }
    });

    document.getElementById('btn-en').classList.toggle('active', lang === 'en');
    document.getElementById('btn-zh').classList.toggle('active', lang === 'zh');

    localStorage.setItem('preferred_lang', lang);
  }

  (function initLang() {
    const saved = localStorage.getItem('preferred_lang');
    const browserLang = (navigator.language || 'en').toLowerCase();
    const defaultLang = saved || (browserLang.startsWith('zh') ? 'zh' : 'en');
    setLang(defaultLang);
  })();
</script>
