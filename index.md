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
            I am a Ph.D. candidate in Information and Communication Engineering at Beijing Jiaotong University, affiliated with the National Engineering Research Center for Advanced Network Technologies, led by Prof. Hongke Zhang, Academician of the Chinese Academy of Engineering and IEEE Fellow. I am advised by Prof. Shuai Gao and closely mentored by Assoc. Prof. Weiting Zhang. I am expected to graduate in December 2026. My research focuses on networking for distributed intelligence in low-altitude networks.
          </p>
          <p>
            My research background spans robot motion planning during my master's study and, during my Ph.D., UAV networking, LLM agents, network systems and protocols, federated learning, and reinforcement learning. Working across these topics has strengthened my ability to conduct interdisciplinary research and quickly adapt to new research directions. In addition to publishing peer-reviewed papers and building prototype systems, I have contributed to several research grant proposals, which has also strengthened my technical writing and project-planning skills. I am seeking postdoctoral opportunities where I can contribute both rigorous research and practical system experience.
          </p>
          <p class="tag-line">
            Research interests: UAV and low-altitude networks; mobile and edge intelligence; LLM-enabled wireless and edge networks; reinforcement learning; federated learning; programmable network systems.
          </p>
        </section>

        <section>
          <h2>News</h2>
          <ul class="news-list">
            <li><strong>2026:</strong> AgentNet accepted by IEEE Communications Magazine.</li>
            <li><strong>2026:</strong> HierTask published online in IEEE Transactions on Network Science and Engineering.</li>
            <li><strong>2026:</strong> One paper accepted by IEEE ICC 2026.</li>
            <li><strong>2025:</strong> OpenL3 published in IEEE Internet of Things Journal.</li>
            <li><strong>2025:</strong> X-CFL published in IEEE GLOBECOM 2025.</li>
          </ul>
        </section>

        <section>
          <h2>Publications</h2>
          <h3>Journal Papers</h3>
          <ol class="pub-list">
            <li><strong>J. Lan</strong>, S. Gao, W. Zhang, X. Hou, M. Xi, Y. Zhang, B. Lei, H. Zhang, and X. Shen, "OpenL3: Embedding Diverse Network Services into MANETs Using Multidimensional Identifier," <em>IEEE Internet of Things Journal</em>, vol. 12, no. 11, pp. 17700-17716, 2025. <a href="https://ieeexplore.ieee.org/abstract/document/10870164" target="_blank" rel="noopener">[paper]</a></li>
            <li><strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, and H. Zhang, "HierTask: Enabling QoS-Aware Hierarchical Task-Centric Routing for UAV Swarms," <em>IEEE Transactions on Network Science and Engineering</em>, 2026. <a href="https://ieeexplore.ieee.org/abstract/document/11535666" target="_blank" rel="noopener">[paper]</a></li>
            <li><strong>J. Lan</strong>, S. Gao, B. Lei, W. Zhang, Y. Wang, and H. Zhang, "AgentNet: An Agent-Centric Network Architecture for LLM-Enabled Low-Altitude Wireless Networks," accepted for publication in <em>IEEE Communications Magazine</em>.</li>
            <li><strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, and H. Zhang, "X-CFL: A Cross-Layer Clustered Federated Learning Framework for UAV Networks," submitted to <em>IEEE/ACM Transactions on Networking</em>, under review.</li>
            <li>R. Chai, S. Gao, <strong>J. Lan</strong>, and N. Liu, "Efficient Computing Resource Measurement Method in Computing Power Networks," <em>Journal of Computer Research and Development</em>, vol. 60, no. 4, pp. 763-771, 2023. <a href="https://kns.cnki.net/kcms2/article/abstract?v=mX7l0X-lXK1Dh5aNVZhNR6yZAJ-FXqWcX4q4RlAMfT4q-5Fzl6MaJ6lp__obgoYqAKt2sV9ntEQJOFZB1o7PynAqFIZmQoDnMrFK28XxjZFPawV1BInEdKUM_WopSb8hIkqVR0EBVl1bm30Kc5nFuNbSheAGUfEvLWoob_Jn8EU1Zsa5Vcv2Tw==&uniplatform=NZKPT&language=CHS" target="_blank" rel="noopener">[paper]</a></li>
            <li>Y. Xie and <strong>J. Lan</strong>, "Review of Collaborative Robots and Their Motion Planning Methods," <em>Journal of Computer Engineering &amp; Applications</em>, vol. 57, no. 13, 2021. <a href="https://www.researchgate.net/profile/Jiangyu-Lan/publication/370779755_Review_of_Collaborative_Robot_and_Its_Motion_Planning_Methods/links/64636252f43b8a29ba53bfe8/Review-of-Collaborative-Robot-and-Its-Motion-Planning-Methods.pdf" target="_blank" rel="noopener">[paper]</a></li>
            <li><strong>J. Lan</strong>, Y. Xie, G. Liu, and M. Cao, "A Multi-Objective Trajectory Planning Method for Collaborative Robot," <em>Electronics</em>, vol. 9, no. 5, article 859, 2020. <a href="https://www.mdpi.com/2079-9292/9/5/859" target="_blank" rel="noopener">[paper]</a></li>
            <li>Y. Xie, G. Liu, <strong>J. Lan</strong>, and B. Gao, "Abdominal Needle Assisted Robotic Arm Motion Control and Trajectory Planning," <em>J. Computers</em>, vol. 31, no. 2, pp. 298-311, 2020. <a href="https://scholar.google.com/citations?view_op=view_citation&hl=en&user=sa89XfwAAAAJ&citation_for_view=sa89XfwAAAAJ:d1gkVwhDpl0C" target="_blank" rel="noopener">[paper]</a></li>
            <li>Y. Xie, J. Xing, G. Liu, <strong>J. Lan</strong>, and Y. Dong, "Real-Time Reconstruction of Unstructured Scenes Based on Binocular Vision Depth," <em>Journal of Internet Technology</em>, vol. 20, no. 5, pp. 1611-1623, 2019. <a href="https://jit.ndhu.edu.tw/article/view/2142" target="_blank" rel="noopener">[paper]</a></li>
            <li>Y. Xie, H. Wang, H. Su, and <strong>J. Lan</strong>, "Noise Reduction Based on Kalman Filter of Low Precision Gyroscope," <em>Journal of Computers</em>, vol. 30, no. 5, pp. 313-327, 2019. <a href="https://www.airitilibrary.com/Article/Detail/19911599-201910-201911070003-201911070003-313-327" target="_blank" rel="noopener">[paper]</a></li>
          </ol>

          <h3>Conference Papers</h3>
          <ol class="pub-list">
            <li><strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "X-CFL: Enabling Cross-Layer Clustered Federated Learning in UAV Swarms," in Proc. <em>IEEE GLOBECOM</em>, 2025, pp. 4403-4408. <a href="https://ieeexplore.ieee.org/abstract/document/11432689" target="_blank" rel="noopener">[paper]</a></li>
            <li><strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "Enabling QoS-Aware Multi-Stage Task Allocation in FANETs: A Hierarchical Learning Approach," accepted for publication in Proc. <em>IEEE ICC</em>, 2026.</li>
            <li>R. Ping and <strong>J. Lan</strong> (corresponding author), "A Trustworthy Service Authorization Mechanism for Multidimensional Identifier Networks," accepted for publication in Proc. <em>ICCCS</em>, 2026.</li>
            <li>Q. Ma, S. Gao, M. Xi, and <strong>J. Lan</strong>, "A Multi-Dimensional Identifier-Based Routing Mechanism for Flying Ad-Hoc Networks," in Proc. <em>ICCCS</em>, 2024, pp. 691-697. <a href="https://ieeexplore.ieee.org/abstract/document/10603072" target="_blank" rel="noopener">[paper]</a></li>
            <li><strong>J. Lan</strong>, Y. Xie, H. Wang, and G. Liu, "A Face Recognition System Based on Improved Convolutional Neural Network," in Proc. <em>2019 2nd International Conference on Algorithms, Computing and Artificial Intelligence</em>, 2019. <a href="https://dl.acm.org/doi/abs/10.1145/3377713.3377765" target="_blank" rel="noopener">[paper]</a></li>
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
            我目前博士就读于北京交通大学移动专用网络国家工程研究中心（张宏科院士团队），导师为郜帅教授，同时受张维庭副教授学术指导，预计于 2026 年 12 月毕业。我的研究主要聚焦面向低空网络中分布式智能服务的网络系统与技术。
          </p>
          <p>
            我的研究经历覆盖多个方向：硕士期间主要从事机器人运动规划研究，博士期间进一步拓展到无人机网络、LLM agent、网络系统与协议、联邦学习和强化学习算法等方向。不同研究主题的训练使我具备较强的跨学科交叉研究能力，也能够较快学习并适应新的研究方向。博士期间，除发表论文和参与工程原型系统搭建外，我还参与了多个基金申请书的撰写，积累了较强的技术写作和项目规划能力。未来我希望在博士后工作中继续贡献扎实的研究能力和系统实现经验。
          </p>
          <p class="tag-line">
            研究方向：无人机与低空网络；移动与边缘智能；大模型赋能的无线与边缘网络；强化学习；联邦学习；可编程网络系统。
          </p>
        </section>

        <section>
          <h2>近期动态</h2>
          <ul class="news-list">
            <li><strong>2026：</strong>AgentNet 论文被 IEEE Communications Magazine 接收。</li>
            <li><strong>2026：</strong>HierTask 论文在 IEEE Transactions on Network Science and Engineering 网络出版。</li>
            <li><strong>2026：</strong>一篇论文被 IEEE ICC 2026 接收。</li>
            <li><strong>2025：</strong>OpenL3 论文发表于 IEEE Internet of Things Journal。</li>
            <li><strong>2025：</strong>X-CFL 论文发表于 IEEE GLOBECOM 2025。</li>
          </ul>
        </section>

        <section>
          <h2>论文列表</h2>
          <h3>期刊论文</h3>
          <ol class="pub-list">
            <li><strong>J. Lan</strong>, S. Gao, W. Zhang, X. Hou, M. Xi, Y. Zhang, B. Lei, H. Zhang, and X. Shen, "OpenL3: Embedding Diverse Network Services into MANETs Using Multidimensional Identifier," <em>IEEE Internet of Things Journal</em>, vol. 12, no. 11, pp. 17700-17716, 2025. <a href="https://ieeexplore.ieee.org/abstract/document/10870164" target="_blank" rel="noopener">[paper]</a></li>
            <li><strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, and H. Zhang, "HierTask: Enabling QoS-Aware Hierarchical Task-Centric Routing for UAV Swarms," <em>IEEE Transactions on Network Science and Engineering</em>, 2026. <a href="https://ieeexplore.ieee.org/abstract/document/11535666" target="_blank" rel="noopener">[paper]</a></li>
            <li><strong>J. Lan</strong>, S. Gao, B. Lei, W. Zhang, Y. Wang, and H. Zhang, "AgentNet: An Agent-Centric Network Architecture for LLM-Enabled Low-Altitude Wireless Networks," accepted for publication in <em>IEEE Communications Magazine</em>.</li>
            <li><strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, and H. Zhang, "X-CFL: A Cross-Layer Clustered Federated Learning Framework for UAV Networks," submitted to <em>IEEE/ACM Transactions on Networking</em>, under review.</li>
            <li>柴若楠，郜帅，<strong>兰江雨</strong>，刘宁春，“算力网络中高效算力资源度量方法”，<em>计算机研究与发展</em>，60(4): 763-771, 2023. <a href="https://kns.cnki.net/kcms2/article/abstract?v=mX7l0X-lXK1Dh5aNVZhNR6yZAJ-FXqWcX4q4RlAMfT4q-5Fzl6MaJ6lp__obgoYqAKt2sV9ntEQJOFZB1o7PynAqFIZmQoDnMrFK28XxjZFPawV1BInEdKUM_WopSb8hIkqVR0EBVl1bm30Kc5nFuNbSheAGUfEvLWoob_Jn8EU1Zsa5Vcv2Tw==&uniplatform=NZKPT&language=CHS" target="_blank" rel="noopener">[paper]</a></li>
            <li>解迎刚，<strong>兰江雨</strong>，“协作机器人及其运动规划方法研究综述”，<em>计算机工程与应用</em>，57(13), 2021. <a href="https://www.researchgate.net/profile/Jiangyu-Lan/publication/370779755_Review_of_Collaborative_Robot_and_Its_Motion_Planning_Methods/links/64636252f43b8a29ba53bfe8/Review-of-Collaborative-Robot-and-Its-Motion-Planning-Methods.pdf" target="_blank" rel="noopener">[paper]</a></li>
            <li><strong>J. Lan</strong>, Y. Xie, G. Liu, and M. Cao, "A Multi-Objective Trajectory Planning Method for Collaborative Robot," <em>Electronics</em>, vol. 9, no. 5, article 859, 2020. <a href="https://www.mdpi.com/2079-9292/9/5/859" target="_blank" rel="noopener">[paper]</a></li>
            <li>Y. Xie, G. Liu, <strong>J. Lan</strong>, and B. Gao, "Abdominal Needle Assisted Robotic Arm Motion Control and Trajectory Planning," <em>J. Computers</em>, vol. 31, no. 2, pp. 298-311, 2020. <a href="https://scholar.google.com/citations?view_op=view_citation&hl=en&user=sa89XfwAAAAJ&citation_for_view=sa89XfwAAAAJ:d1gkVwhDpl0C" target="_blank" rel="noopener">[paper]</a></li>
            <li>Y. Xie, J. Xing, G. Liu, <strong>J. Lan</strong>, and Y. Dong, "Real-Time Reconstruction of Unstructured Scenes Based on Binocular Vision Depth," <em>Journal of Internet Technology</em>, vol. 20, no. 5, pp. 1611-1623, 2019. <a href="https://jit.ndhu.edu.tw/article/view/2142" target="_blank" rel="noopener">[paper]</a></li>
            <li>Y. Xie, H. Wang, H. Su, and <strong>J. Lan</strong>, "Noise Reduction Based on Kalman Filter of Low Precision Gyroscope," <em>Journal of Computers</em>, vol. 30, no. 5, pp. 313-327, 2019. <a href="https://www.airitilibrary.com/Article/Detail/19911599-201910-201911070003-201911070003-313-327" target="_blank" rel="noopener">[paper]</a></li>
          </ol>

          <h3>会议论文</h3>
          <ol class="pub-list">
            <li><strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "X-CFL: Enabling Cross-Layer Clustered Federated Learning in UAV Swarms," in Proc. <em>IEEE GLOBECOM</em>, 2025, pp. 4403-4408. <a href="https://ieeexplore.ieee.org/abstract/document/11432689" target="_blank" rel="noopener">[paper]</a></li>
            <li><strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "Enabling QoS-Aware Multi-Stage Task Allocation in FANETs: A Hierarchical Learning Approach," accepted for publication in Proc. <em>IEEE ICC</em>, 2026.</li>
            <li>R. Ping and <strong>J. Lan</strong> (corresponding author), "A Trustworthy Service Authorization Mechanism for Multidimensional Identifier Networks," accepted for publication in Proc. <em>ICCCS</em>, 2026.</li>
            <li>Q. Ma, S. Gao, M. Xi, and <strong>J. Lan</strong>, "A Multi-Dimensional Identifier-Based Routing Mechanism for Flying Ad-Hoc Networks," in Proc. <em>ICCCS</em>, 2024, pp. 691-697. <a href="https://ieeexplore.ieee.org/abstract/document/10603072" target="_blank" rel="noopener">[paper]</a></li>
            <li><strong>J. Lan</strong>, Y. Xie, H. Wang, and G. Liu, "A Face Recognition System Based on Improved Convolutional Neural Network," in Proc. <em>2019 2nd International Conference on Algorithms, Computing and Artificial Intelligence</em>, 2019. <a href="https://dl.acm.org/doi/abs/10.1145/3377713.3377765" target="_blank" rel="noopener">[paper]</a></li>
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
