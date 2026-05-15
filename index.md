<style>
:root {
  --text: #222;
  --muted: #666;
  --line: #e5e5e5;
  --link: #2b6dad;
  --link-dark: #1f4f7f;
  --soft: #f7f7f7;
}

/* Overrides for the default GitHub Pages Architect theme. */
header .button,
#sidebar {
  display: none !important;
}

header {
  padding: 22px 0 !important;
}

header h1 {
  font-size: 2rem !important;
}

header h2 {
  font-size: 1rem !important;
  line-height: 1.5 !important;
}

#content-wrapper .inner,
header .inner {
  width: auto !important;
  max-width: 1120px !important;
  padding-left: 24px !important;
  padding-right: 24px !important;
}

#main-content {
  float: none !important;
  width: 100% !important;
}

.academic-home {
  max-width: 1120px;
  margin: 0 auto;
  color: var(--text);
  font-family: "Segoe UI", "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif;
  font-size: 16px;
  line-height: 1.7;
}

.lang-toggle {
  display: flex;
  justify-content: flex-end;
  gap: 8px;
  margin: 6px 0 18px;
}

.lang-btn {
  border: 1px solid #b8c7d8;
  background: #fff;
  color: var(--link-dark);
  border-radius: 4px;
  padding: 4px 10px;
  font-size: 0.9rem;
  cursor: pointer;
}

.lang-btn.active,
.lang-btn:hover {
  background: var(--link);
  border-color: var(--link);
  color: #fff;
}

.page-layout {
  display: grid;
  grid-template-columns: 220px minmax(0, 1fr);
  gap: 42px;
  align-items: start;
}

.sidebar {
  border-right: 1px solid var(--line);
  padding-right: 24px;
  font-size: 0.86rem;
  line-height: 1.58;
}

.profile-photo {
  width: 155px;
  margin: 0 0 18px;
}

.profile-photo img {
  display: block;
  width: 155px;
  height: 200px;
  border-radius: 4px;
  object-fit: cover;
  border: 1px solid var(--line);
}

.name {
  margin: 0 0 8px;
  font-size: 1.45rem;
  line-height: 1.2;
}

.position {
  margin: 0 0 14px;
  color: var(--muted);
  line-height: 1.55;
}

.profile-links {
  list-style: none;
  margin: 0;
  padding: 12px 0 0;
  border-top: 1px solid var(--line);
}

.profile-links li {
  display: grid;
  grid-template-columns: 20px minmax(0, 1fr);
  gap: 8px;
  align-items: start;
  margin-bottom: 9px;
}

.profile-icon {
  color: var(--muted);
  text-align: center;
  line-height: 1.55;
}

.content section {
  margin-bottom: 30px;
}

.content h1 {
  margin: 0 0 10px;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 1.55rem;
  font-weight: 600;
  line-height: 1.25;
}

.content h2 {
  margin: 0 0 12px;
  border-bottom: 1px solid var(--line);
  padding-bottom: 5px;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 1.18rem;
  font-weight: 600;
}

.content h3 {
  margin: 20px 0 8px;
  font-size: 1rem;
  font-weight: 600;
}

.content p {
  margin: 0 0 12px;
}

.content ul,
.content ol {
  margin: 0;
  padding-left: 22px;
}

.content li {
  margin-bottom: 9px;
}

.pub-list {
  padding-left: 22px;
}

.pub-list li {
  margin-bottom: 12px;
}

.meta {
  color: var(--muted);
}

.tag-line {
  margin-top: 10px;
  color: var(--muted);
}

.news-list strong,
.time {
  color: var(--link-dark);
}

a {
  color: var(--link);
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

[data-lang] {
  display: none;
}

[data-lang].visible {
  display: block;
}

@media (max-width: 820px) {
  .page-layout {
    grid-template-columns: 1fr;
    gap: 24px;
  }

  .sidebar {
    border-right: 0;
    border-bottom: 1px solid var(--line);
    padding-right: 0;
    padding-bottom: 18px;
  }
}
</style>

<div class="academic-home">
  <div class="lang-toggle">
    <button class="lang-btn active" id="btn-en" type="button" onclick="setLang('en')">English</button>
    <button class="lang-btn" id="btn-zh" type="button" onclick="setLang('zh')">中文</button>
  </div>

  <div data-lang="en" class="visible">
    <div class="page-layout">
      <aside class="sidebar">
        <div class="profile-photo">
          <img src="assets/profile.jpg" alt="Jiangyu Lan" onerror="this.parentElement.style.display='none'">
        </div>
        <h1 class="name">Jiangyu Lan</h1>
        <p class="position">
          Ph.D. Candidate<br>
          Information and Communication Engineering
        </p>

        <ul class="profile-links">
          <li><span class="profile-icon">🏛</span><span>Beijing Jiaotong University</span></li>
          <li><span class="profile-icon">✉</span><a href="mailto:lanjiangyu@bjtu.edu.cn">lanjiangyu@bjtu.edu.cn</a></li>
          <li><span class="profile-icon">🎓</span><a href="https://scholar.google.com/citations?user=sa89XfwAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a></li>
        </ul>
      </aside>

      <main class="content">
        <section>
          <p>
            I am a Ph.D. candidate inthe National Engineering Research Center of Advanced Network Technologies (lead by Prof. Hongke Zhang, Member of the Chinese Academy of Engineering and IEEE Fellow) at Beijing Jiaotong University, advised by Prof. Shuai Gao and Assoc. Prof. Weiting Zhang. I am expected to graduate in December 2026. My research focuses on networking for distributed intelligence in low-altitude networks.
          </p>
          <p>
            I am interested in edge intelligence, learning-enabled network optimization, and programmable routing and forwarding. My recent work explores networking support for federated learning, multi-stage UAV collaboration, and LLM-agent cooperation in dynamic wireless environments.
          </p>
          <p class="tag-line">
            Research interests: UAV and low-altitude networks; mobile and edge intelligence; LLM-enabled wireless and edge networks; reinforcement learning; federated learning; programmable network systems.
          </p>
        </section>

        <section>
          <h2>News</h2>
          <ul class="news-list">
            <li><strong>2026:</strong> One paper accepted by IEEE ICC 2026.</li>
            <li><strong>2025:</strong> OpenL3 published in IEEE Internet of Things Journal.</li>
            <li><strong>2025:</strong> X-CFL published in IEEE GLOBECOM 2025.</li>
          </ul>
        </section>

        <section>
          <h2>Selected Publications</h2>
          <h3>Journal Papers and Manuscripts</h3>
          <ol class="pub-list">
            <li><strong>J. Lan</strong>, S. Gao, W. Zhang, X. Hou, M. Xi, Y. Zhang, B. Lei, H. Zhang, and X. Shen, "OpenL3: Embedding Diverse Network Services into MANETs Using Multidimensional Identifier," <em>IEEE Internet of Things Journal</em>, vol. 12, no. 11, pp. 17700-17716, 2025.</li>
            <li><strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, D. Niyato, and H. Zhang, "X-CFL: A Cross-Layer Clustered Federated Learning Framework for UAV Networks," submitted to <em>IEEE Transactions on Mobile Computing</em>, under review after major revision.</li>
            <li><strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, and H. Zhang, "HierTask: Enabling QoS-Aware Hierarchical Task-Centric Routing for UAV Swarms," submitted to <em>IEEE Transactions on Network Science and Engineering</em>, under review after major revision.</li>
            <li><strong>J. Lan</strong>, S. Gao, B. Lei, W. Zhang, Y. Wang, and H. Zhang, "AgentNet: An Agent-Centric Network Architecture for LLM-Enabled Low-Altitude Wireless Networks," submitted to <em>IEEE Communications Magazine</em>, under review after minor revision.</li>
          </ol>

          <h3>Conference and Other Peer-Reviewed Papers</h3>
          <ol class="pub-list">
            <li><strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "X-CFL: Enabling Cross-Layer Clustered Federated Learning in UAV Swarms," in Proc. <em>IEEE GLOBECOM</em>, 2025, pp. 4403-4408.</li>
            <li><strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "Enabling QoS-Aware Multi-Stage Task Allocation in FANETs: A Hierarchical Learning Approach," accepted for publication in Proc. <em>IEEE ICC</em>, 2026.</li>
            <li>R. Ping and <strong>J. Lan</strong> (corresponding author), "A Trustworthy Service Authorization Mechanism for Multidimensional Identifier Networks," accepted for publication in Proc. <em>ICCCS</em>, 2026.</li>
            <li>Q. Ma, S. Gao, M. Xi, and <strong>J. Lan</strong>, "A Multi-Dimensional Identifier-Based Routing Mechanism for Flying Ad-Hoc Networks," in Proc. <em>ICCCS</em>, 2024, pp. 691-697.</li>
            <li><strong>J. Lan</strong>, Y. Xie, G. Liu, and M. Cao, "A Multi-Objective Trajectory Planning Method for Collaborative Robot," <em>Electronics</em>, vol. 9, no. 5, article 859, 2020.</li>
          </ol>
        </section>

        <section>
          <h2>Research Experience</h2>
          <ul>
            <li><strong>Agentic AI and LLM-enabled networking:</strong> designed AgentNet, an agent-centric architecture for LLM-agent cooperation in low-altitude wireless networks.</li>
            <li><strong>Network-aware edge intelligence:</strong> designed X-CFL, a cross-layer clustered federated learning framework considering data similarity, link quality, energy, and mobility.</li>
            <li><strong>Task-oriented UAV network autonomy:</strong> developed HierTask for QoS-aware multi-stage UAV collaboration and task-centric routing.</li>
            <li><strong>Programmable mobile network architecture:</strong> designed OpenL3 and implemented an SDN/P4-based prototype for flexible routing, forwarding, and service coexistence.</li>
          </ul>
        </section>

        <section>
          <h2>Education</h2>
          <ul>
            <li><span class="time">Sep. 2022 - Dec. 2026 expected:</span> Ph.D. in Information and Communication Engineering, Beijing Jiaotong University.</li>
            <li><span class="time">Sep. 2018 - Jun. 2021:</span> M.S. in Electronics and Communication Engineering, Beijing Information Science and Technology University.</li>
            <li><span class="time">Sep. 2014 - Jun. 2018:</span> B.E. in Communication Engineering, Beijing Information Science and Technology University.</li>
          </ul>
        </section>

        <section>
          <h2>Work Experience</h2>
          <ul>
            <li><span class="time">Jul. 2021 - Jul. 2022:</span> Network Engineer, China Telecom.</li>
            <li>Worked on operation and maintenance for carrier-grade communication networks, gaining practical experience in network management and communication infrastructure.</li>
          </ul>
        </section>

        <section>
          <h2>Research Projects</h2>
          <ul>
            <li>Participating researcher and proposal contributor for national, municipal, and industry-funded projects on cloud-network convergence, intelligent computing networks, multidimensional identifiers, and unmanned swarm networking.</li>
            <li>Participated in the NSFC Joint Fund Key Program on trustworthy multidimensional identifiers for cloud-network convergence, an NSFC Major Research Program subproject on intelligent computing-network service orchestration, and a Beijing Natural Science Foundation project on unmanned swarm networking.</li>
            <li>Participated in China Telecom industry-academia projects on cloud-network convergence, intelligent inference, and identifier-integrated networking.</li>
            <li>Contributed to technical proposal writing, literature review, research problem formulation, and project planning.</li>
          </ul>
        </section>

        <section>
          <h2>Patents</h2>
          <ul>
            <li>S. Gao, <strong>J. Lan</strong>, Y. Zhang, T. Zheng, W. Quan, and W. Su, "Clustered Federated Learning Method, Apparatus, and Electronic Device for UAV Swarms," Chinese Patent, No. CN121865363A.</li>
            <li>S. Gao, Y. Zhang, Y. Yi, <strong>J. Lan</strong>, W. Su, and H. Zhang, "A Multicast Communication Method, System, and Electronic Device Based on 3D Geographic Location," Chinese Patent, No. CN122001807A.</li>
            <li>S. Gao, <strong>J. Lan</strong>, W. Zhang, Y. Zhang, and H. Zhang, "QoS-Aware Multi-Stage Task Allocation Method and System for UAV Swarms," Chinese Patent, pending.</li>
            <li>S. Gao, Y. Zhang, Y. Li, <strong>J. Lan</strong>, P. Dong, and H. Zhang, "Identifier-Based Communication Method, Data Forwarding Method, and Apparatus for Identity-Based Multicast," Chinese Patent, pending.</li>
          </ul>
        </section>

        <section>
          <h2>Academic Service</h2>
          <ul>
            <li>Reviewer for <em>IEEE Transactions on Network Science and Engineering</em>.</li>
            <li>Reviewer for <em>IEEE Transactions on Cognitive Communications and Networking</em>.</li>
          </ul>
        </section>

        <section>
          <h2>Technical Skills</h2>
          <ul>
            <li><strong>Programming:</strong> Python, C/C++, MATLAB, LaTeX.</li>
            <li><strong>Machine learning:</strong> PyTorch, TensorFlow, scikit-learn, Pandas, NumPy.</li>
            <li><strong>Networking and systems:</strong> SDN, P4, NS-3, ROS, Linux.</li>
            <li><strong>Research methods:</strong> federated learning, reinforcement learning, UAV network simulation.</li>
          </ul>
        </section>
      </main>
    </div>
  </div>

  <div data-lang="zh">
    <div class="page-layout">
      <aside class="sidebar">
        <div class="profile-photo">
          <img src="assets/profile.jpg" alt="兰江雨" onerror="this.parentElement.style.display='none'">
        </div>
        <h1 class="name">兰江雨</h1>
        <p class="position">
          博士研究生<br>
          信息与通信工程
        </p>

        <ul class="profile-links">
          <li><span class="profile-icon">🏛</span><span>北京交通大学</span></li>
          <li><span class="profile-icon">✉</span><a href="mailto:lanjiangyu@bjtu.edu.cn">lanjiangyu@bjtu.edu.cn</a></li>
          <li><span class="profile-icon">🎓</span><a href="https://scholar.google.com/citations?user=sa89XfwAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a></li>
        </ul>
      </aside>

      <main class="content">
        <section>
          <p>
            我目前博士就读于北京交通大学移动专用网络国家工程研究中心（张宏科院士团队）。我的导师是郜帅教授，同时受到了张维庭副教授的学术指导。我预计于 2026 年 12 月毕业，研究聚焦面向低空网络中分布式智能服务的网络系统与技术。
          </p>
          <p>
            我的研究兴趣包括边缘智能、学习驱动的网络优化，以及可编程路由与转发机制。近期工作主要探索面向联邦学习、多阶段无人机协同和大模型智能体协作的网络支撑机制。
          </p>
          <p class="tag-line">
            研究方向：无人机与低空网络；移动与边缘智能；大模型赋能的无线与边缘网络；强化学习；联邦学习；可编程网络系统。
          </p>
        </section>

        <section>
          <h2>近期动态</h2>
          <ul class="news-list">
            <li><strong>2026：</strong>一篇论文被 IEEE ICC 2026 接收。</li>
            <li><strong>2025：</strong>OpenL3 论文发表于 IEEE Internet of Things Journal。</li>
            <li><strong>2025：</strong>X-CFL 论文发表于 IEEE GLOBECOM 2025。</li>
          </ul>
        </section>

        <section>
          <h2>代表性论文</h2>
          <h3>期刊论文与在审稿件</h3>
          <ol class="pub-list">
            <li><strong>J. Lan</strong>, S. Gao, W. Zhang, X. Hou, M. Xi, Y. Zhang, B. Lei, H. Zhang, and X. Shen, "OpenL3: Embedding Diverse Network Services into MANETs Using Multidimensional Identifier," <em>IEEE Internet of Things Journal</em>, vol. 12, no. 11, pp. 17700-17716, 2025.</li>
            <li><strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, D. Niyato, and H. Zhang, "X-CFL: A Cross-Layer Clustered Federated Learning Framework for UAV Networks," submitted to <em>IEEE Transactions on Mobile Computing</em>, under review after major revision.</li>
            <li><strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, and H. Zhang, "HierTask: Enabling QoS-Aware Hierarchical Task-Centric Routing for UAV Swarms," submitted to <em>IEEE Transactions on Network Science and Engineering</em>, under review after major revision.</li>
            <li><strong>J. Lan</strong>, S. Gao, B. Lei, W. Zhang, Y. Wang, and H. Zhang, "AgentNet: An Agent-Centric Network Architecture for LLM-Enabled Low-Altitude Wireless Networks," submitted to <em>IEEE Communications Magazine</em>, under review after minor revision.</li>
          </ol>

          <h3>会议论文与其他同行评议论文</h3>
          <ol class="pub-list">
            <li><strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "X-CFL: Enabling Cross-Layer Clustered Federated Learning in UAV Swarms," in Proc. <em>IEEE GLOBECOM</em>, 2025, pp. 4403-4408.</li>
            <li><strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "Enabling QoS-Aware Multi-Stage Task Allocation in FANETs: A Hierarchical Learning Approach," accepted for publication in Proc. <em>IEEE ICC</em>, 2026.</li>
            <li>R. Ping and <strong>J. Lan</strong> (corresponding author), "A Trustworthy Service Authorization Mechanism for Multidimensional Identifier Networks," accepted for publication in Proc. <em>ICCCS</em>, 2026.</li>
            <li>Q. Ma, S. Gao, M. Xi, and <strong>J. Lan</strong>, "A Multi-Dimensional Identifier-Based Routing Mechanism for Flying Ad-Hoc Networks," in Proc. <em>ICCCS</em>, 2024, pp. 691-697.</li>
            <li><strong>J. Lan</strong>, Y. Xie, G. Liu, and M. Cao, "A Multi-Objective Trajectory Planning Method for Collaborative Robot," <em>Electronics</em>, vol. 9, no. 5, article 859, 2020.</li>
          </ol>
        </section>

        <section>
          <h2>研究经历</h2>
          <ul>
            <li><strong>智能体 AI 与大模型赋能网络：</strong>设计 AgentNet 低空无线网络架构，支撑大模型智能体协作。</li>
            <li><strong>网络感知边缘智能：</strong>设计 X-CFL 跨层聚类联邦学习框架，联合考虑数据相似性、链路质量、能耗与移动性。</li>
            <li><strong>任务驱动无人机网络自治：</strong>开发 HierTask，面向多阶段无人机协同任务研究 QoS 感知任务决策与任务中心路由。</li>
            <li><strong>可编程移动网络架构：</strong>设计 OpenL3，并实现基于 SDN/P4 的原型系统，用于验证灵活路由、转发与多服务共存能力。</li>
          </ul>
        </section>

        <section>
          <h2>教育经历</h2>
          <ul>
            <li><span class="time">2022.09 - 2026.12 预计：</span>北京交通大学，信息与通信工程，博士。</li>
            <li><span class="time">2018.09 - 2021.06：</span>北京信息科技大学，电子与通信工程，硕士。</li>
            <li><span class="time">2014.09 - 2018.06：</span>北京信息科技大学，通信工程，学士。</li>
          </ul>
        </section>

        <section>
          <h2>工作经历</h2>
          <ul>
            <li><span class="time">2021.07 - 2022.07：</span>中国电信，网络工程师。</li>
            <li>参与运营商级通信网络的运行维护工作，积累了网络管理与通信基础设施方面的工程实践经验。</li>
          </ul>
        </section>

        <section>
          <h2>科研项目</h2>
          <ul>
            <li>作为参与研究人员和申请书撰写参与者，参与国家级、市级及产学研项目，研究方向覆盖云网融合、智能算网、多维标识与无人集群网络等。</li>
            <li>参与云网融合可信多维标识相关国家自然科学基金联合基金重点项目、智能算网服务编排相关国家自然科学基金重大研究计划子课题，以及无人集群网络相关北京市自然科学基金项目。</li>
            <li>参与中国电信产学研项目，方向包括云网融合、智能推理与标识融合网络。</li>
            <li>参与技术方案撰写、文献调研、研究问题凝练与项目规划。</li>
          </ul>
        </section>

        <section>
          <h2>专利</h2>
          <ul>
            <li>郜帅、<strong>兰江雨</strong>、张宇明、郑涛、权伟、苏伟，“无人机集群分簇联邦学习方法、装置及电子设备”，中国发明专利，CN121865363A。</li>
            <li>郜帅、张宇明、伊摇、<strong>兰江雨</strong>、苏伟、张宏科，“一种基于三维地理位置的组播通信方法、系统及电子设备”，中国发明专利，CN122001807A。</li>
            <li>郜帅、<strong>兰江雨</strong>、张维庭、张宇明、张宏科，“面向无人机集群的 QoS 感知多阶段任务分配方法及系统”，中国发明专利申请中。</li>
            <li>郜帅、张宇明、李语涵、<strong>兰江雨</strong>、董平、张宏科，“面向基于身份组播的标识通信方法、数据转发方法及装置”，中国发明专利申请中。</li>
          </ul>
        </section>

        <section>
          <h2>学术服务</h2>
          <ul>
            <li>担任 <em>IEEE Transactions on Network Science and Engineering</em> 审稿人。</li>
            <li>担任 <em>IEEE Transactions on Cognitive Communications and Networking</em> 审稿人。</li>
          </ul>
        </section>

        <section>
          <h2>技术能力</h2>
          <ul>
            <li><strong>编程语言：</strong>Python、C/C++、MATLAB、LaTeX。</li>
            <li><strong>机器学习：</strong>PyTorch、TensorFlow、scikit-learn、Pandas、NumPy。</li>
            <li><strong>网络与系统：</strong>SDN、P4、NS-3、ROS、Linux。</li>
            <li><strong>研究方法：</strong>联邦学习、强化学习、无人机网络仿真。</li>
          </ul>
        </section>
      </main>
    </div>
  </div>
</div>

<script>
  function setLang(lang) {
    document.querySelectorAll('[data-lang]').forEach((el) => {
      el.classList.toggle('visible', el.getAttribute('data-lang') === lang);
    });

    document.getElementById('btn-en').classList.toggle('active', lang === 'en');
    document.getElementById('btn-zh').classList.toggle('active', lang === 'zh');

    localStorage.setItem('preferred_lang', lang);
    document.documentElement.setAttribute('lang', lang === 'zh' ? 'zh-CN' : 'en');
  }

  (function initLang() {
    const saved = localStorage.getItem('preferred_lang');
    const browserLang = (navigator.language || 'en').toLowerCase();
    const defaultLang = saved || (browserLang.startsWith('zh') ? 'zh' : 'en');
    setLang(defaultLang);
  })();
</script>
