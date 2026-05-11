<style>
:root {
  --ink: #172033;
  --muted: #5c667a;
  --line: #d8dde8;
  --paper: #ffffff;
  --soft: #f6f8fb;
  --navy: #173b6c;
  --teal: #08756f;
  --gold: #a96f12;
}

.academic-home {
  max-width: 1080px;
  margin: 0 auto;
  color: var(--ink);
}

.lang-toggle {
  display: flex;
  justify-content: flex-end;
  gap: 8px;
  margin: 8px 0 18px;
}

.lang-btn {
  border: 1px solid var(--navy);
  background: var(--paper);
  color: var(--navy);
  border-radius: 999px;
  padding: 6px 14px;
  font-size: 0.9rem;
  cursor: pointer;
  transition: background 0.2s ease, color 0.2s ease, transform 0.2s ease;
}

.lang-btn.active,
.lang-btn:hover {
  background: var(--navy);
  color: #fff;
}

.lang-btn:hover {
  transform: translateY(-1px);
}

.profile-hero {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 260px;
  gap: 28px;
  align-items: stretch;
  border: 1px solid var(--line);
  border-radius: 8px;
  background: linear-gradient(135deg, #ffffff 0%, #f4f8fc 64%, #eef6f4 100%);
  padding: 30px;
  margin-bottom: 18px;
}

.hero-kicker {
  margin: 0 0 8px;
  color: var(--teal);
  font-size: 0.86rem;
  font-weight: 700;
  letter-spacing: 0;
  text-transform: uppercase;
}

.profile-hero h1 {
  margin: 0 0 8px;
  font-size: 2.25rem;
  line-height: 1.15;
}

.subtitle {
  margin: 0 0 16px;
  color: var(--muted);
  font-size: 1.04rem;
}

.profile-hero p {
  margin: 10px 0;
  line-height: 1.72;
}

.hero-links {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 18px;
}

.hero-links a,
.hero-links span {
  display: inline-flex;
  align-items: center;
  border: 1px solid var(--line);
  border-radius: 999px;
  padding: 6px 12px;
  background: rgba(255, 255, 255, 0.72);
  color: var(--navy);
  text-decoration: none;
  font-size: 0.92rem;
}

.hero-links a:hover {
  border-color: var(--navy);
  text-decoration: none;
}

.profile-panel {
  border-left: 4px solid var(--teal);
  background: rgba(255, 255, 255, 0.8);
  padding: 18px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.profile-panel dl {
  margin: 0;
}

.profile-panel dt {
  margin-top: 14px;
  color: var(--muted);
  font-size: 0.8rem;
  font-weight: 700;
  text-transform: uppercase;
}

.profile-panel dt:first-child {
  margin-top: 0;
}

.profile-panel dd {
  margin: 4px 0 0;
  line-height: 1.55;
}

.metric-row {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 12px;
  margin-bottom: 18px;
}

.metric {
  border: 1px solid var(--line);
  border-radius: 8px;
  background: var(--paper);
  padding: 14px;
}

.metric strong {
  display: block;
  color: var(--navy);
  font-size: 1.45rem;
  line-height: 1.2;
}

.metric span {
  color: var(--muted);
  font-size: 0.9rem;
}

.section-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 16px;
  margin-bottom: 16px;
}

.section-card,
.wide-section {
  border: 1px solid var(--line);
  border-radius: 8px;
  background: var(--paper);
  padding: 20px;
  box-shadow: 0 8px 24px rgba(23, 32, 51, 0.04);
}

.wide-section {
  margin-bottom: 16px;
}

.section-card h2,
.wide-section h2 {
  margin: 0 0 14px;
  padding-left: 11px;
  border-left: 4px solid var(--navy);
  font-size: 1.22rem;
  line-height: 1.3;
}

.section-card ul,
.wide-section ul {
  margin: 0;
  padding-left: 20px;
}

.section-card li,
.wide-section li {
  margin-bottom: 9px;
  line-height: 1.65;
}

.section-card li:last-child,
.wide-section li:last-child {
  margin-bottom: 0;
}

.tag-list {
  display: flex;
  flex-wrap: wrap;
  gap: 9px;
  margin-top: 12px;
}

.tag {
  border: 1px solid #cfd9e6;
  border-radius: 999px;
  background: var(--soft);
  color: #24364f;
  padding: 5px 10px;
  font-size: 0.88rem;
}

.timeline-item {
  border-left: 2px solid #d7e0ee;
  padding-left: 14px;
  margin-bottom: 14px;
}

.timeline-item:last-child {
  margin-bottom: 0;
}

.time {
  color: var(--gold);
  font-weight: 700;
  font-size: 0.9rem;
}

.role {
  margin-top: 3px;
  font-weight: 700;
}

.meta {
  color: var(--muted);
  font-size: 0.95rem;
}

.pub-list {
  list-style: none;
  padding-left: 0 !important;
}

.pub-list li {
  position: relative;
  padding-left: 42px;
}

.pub-label {
  position: absolute;
  left: 0;
  top: 0;
  color: var(--teal);
  font-weight: 700;
}

.subhead {
  margin: 16px 0 8px;
  color: var(--navy);
  font-size: 1rem;
}

.two-column-list {
  columns: 2;
  column-gap: 28px;
}

.footer-note {
  border-left: 4px solid var(--teal);
  background: #f4f8f7;
  color: #2f3d4f;
  padding: 13px 15px;
  margin: 18px 0 0;
  line-height: 1.65;
}

[data-lang] {
  display: none;
}

[data-lang].visible {
  display: block;
}

@media (max-width: 820px) {
  .profile-hero,
  .section-grid,
  .metric-row {
    grid-template-columns: 1fr;
  }

  .profile-hero {
    padding: 22px;
  }

  .profile-hero h1 {
    font-size: 1.8rem;
  }

  .two-column-list {
    columns: 1;
  }
}
</style>

<div class="academic-home">
  <div class="lang-toggle">
    <button class="lang-btn active" id="btn-en" type="button" onclick="setLang('en')">English</button>
    <button class="lang-btn" id="btn-zh" type="button" onclick="setLang('zh')">中文</button>
  </div>

  <div data-lang="en" class="visible">
    <section class="profile-hero">
      <div>
        <p class="hero-kicker">Academic Homepage</p>
        <h1>Jiangyu Lan</h1>
        <p class="subtitle">Ph.D. Candidate in Information and Communication Engineering, Beijing Jiaotong University</p>
        <p>
          I work on adaptive networking for distributed intelligence in UAV and low-altitude networks. My research emphasizes edge intelligence, learning-enabled network optimization, and programmable routing and forwarding for emerging intelligent services.
        </p>
        <p>
          Recent work explores networking support for federated learning, multi-stage UAV collaboration, and LLM-agent cooperation in dynamic wireless environments.
        </p>
        <div class="hero-links">
          <a href="mailto:lanjiangyu@bjtu.edu.cn">lanjiangyu@bjtu.edu.cn</a>
          <a href="https://scholar.google.com/citations?user=sa89XfwAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a>
          <span>Expected Ph.D. graduation: Dec. 2026</span>
        </div>
      </div>
      <aside class="profile-panel">
        <dl>
          <dt>Affiliation</dt>
          <dd>Beijing Jiaotong University</dd>
          <dt>Advisor</dt>
          <dd>Prof. Shuai Gao</dd>
          <dt>Research Mentor</dt>
          <dd>Assoc. Prof. Weiting Zhang</dd>
          <dt>Background</dt>
          <dd>UAV networks, edge intelligence, programmable network systems</dd>
        </dl>
      </aside>
    </section>

    <section class="metric-row" aria-label="Profile highlights">
      <div class="metric"><strong>6</strong><span>Ph.D.-stage first-author papers and manuscripts</span></div>
      <div class="metric"><strong>4</strong><span>Chinese patents published or pending</span></div>
      <div class="metric"><strong>2</strong><span>IEEE journal reviewer roles</span></div>
      <div class="metric"><strong>1</strong><span>Year carrier network engineering experience</span></div>
    </section>

    <section class="wide-section">
      <h2>Research Interests</h2>
      <div class="tag-list">
        <span class="tag">UAV and low-altitude networks</span>
        <span class="tag">Mobile and edge intelligence</span>
        <span class="tag">LLM-enabled wireless and edge networks</span>
        <span class="tag">Reinforcement learning for network optimization</span>
        <span class="tag">Federated learning over dynamic wireless networks</span>
        <span class="tag">Programmable network systems</span>
      </div>
    </section>

    <section class="section-grid">
      <article class="section-card">
        <h2>Education</h2>
        <div class="timeline-item">
          <div class="time">Sep. 2022 - Dec. 2026 expected</div>
          <div class="role">Ph.D. in Information and Communication Engineering</div>
          <div class="meta">Beijing Jiaotong University</div>
        </div>
        <div class="timeline-item">
          <div class="time">Sep. 2018 - Jun. 2021</div>
          <div class="role">M.S. in Electronics and Communication Engineering</div>
          <div class="meta">Beijing Information Science and Technology University</div>
        </div>
        <div class="timeline-item">
          <div class="time">Sep. 2014 - Jun. 2018</div>
          <div class="role">B.E. in Communication Engineering</div>
          <div class="meta">Beijing Information Science and Technology University</div>
        </div>
      </article>

      <article class="section-card">
        <h2>Experience</h2>
        <div class="timeline-item">
          <div class="time">Jul. 2021 - Jul. 2022</div>
          <div class="role">Network Engineer</div>
          <div class="meta">China Telecom</div>
        </div>
        <ul>
          <li>Worked on operation and maintenance for carrier-grade communication networks.</li>
          <li>Gained practical experience in network management and communication infrastructure.</li>
        </ul>
      </article>
    </section>

    <section class="wide-section">
      <h2>Selected Publications</h2>
      <p>
        During my Ph.D., I have led work on adaptive UAV/low-altitude networking, including one IEEE IoTJ paper, two IEEE conference papers, and three manuscripts under revision at IEEE TMC, IEEE TNSE, and IEEE Communications Magazine.
      </p>
      <h3 class="subhead">Journal Papers and Manuscripts</h3>
      <ul class="pub-list">
        <li><span class="pub-label">J1</span> <strong>J. Lan</strong>, S. Gao, W. Zhang, X. Hou, M. Xi, Y. Zhang, B. Lei, H. Zhang, and X. Shen, "OpenL3: Embedding Diverse Network Services into MANETs Using Multidimensional Identifier," <em>IEEE Internet of Things Journal</em>, vol. 12, no. 11, pp. 17700-17716, 2025.</li>
        <li><span class="pub-label">J2</span> <strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, D. Niyato, and H. Zhang, "X-CFL: A Cross-Layer Clustered Federated Learning Framework for UAV Networks," submitted to <em>IEEE Transactions on Mobile Computing</em>, under review after major revision.</li>
        <li><span class="pub-label">J3</span> <strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, and H. Zhang, "HierTask: Enabling QoS-Aware Hierarchical Task-Centric Routing for UAV Swarms," submitted to <em>IEEE Transactions on Network Science and Engineering</em>, under review after major revision.</li>
        <li><span class="pub-label">J4</span> <strong>J. Lan</strong>, S. Gao, B. Lei, W. Zhang, Y. Wang, and H. Zhang, "AgentNet: An Agent-Centric Network Architecture for LLM-Enabled Low-Altitude Wireless Networks," submitted to <em>IEEE Communications Magazine</em>, under review after minor revision.</li>
      </ul>
      <h3 class="subhead">Conference and Other Peer-Reviewed Papers</h3>
      <ul class="pub-list">
        <li><span class="pub-label">C1</span> <strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "X-CFL: Enabling Cross-Layer Clustered Federated Learning in UAV Swarms," in Proc. <em>IEEE GLOBECOM</em>, 2025, pp. 4403-4408.</li>
        <li><span class="pub-label">C2</span> <strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "Enabling QoS-Aware Multi-Stage Task Allocation in FANETs: A Hierarchical Learning Approach," accepted for publication in Proc. <em>IEEE ICC</em>, 2026.</li>
        <li><span class="pub-label">O1</span> R. Ping and <strong>J. Lan</strong> (corresponding author), "A Trustworthy Service Authorization Mechanism for Multidimensional Identifier Networks," accepted for publication in Proc. <em>ICCCS</em>, 2026.</li>
        <li><span class="pub-label">O2</span> Q. Ma, S. Gao, M. Xi, and <strong>J. Lan</strong>, "A Multi-Dimensional Identifier-Based Routing Mechanism for Flying Ad-Hoc Networks," in Proc. <em>ICCCS</em>, 2024, pp. 691-697.</li>
        <li><span class="pub-label">O3</span> <strong>J. Lan</strong>, Y. Xie, G. Liu, and M. Cao, "A Multi-Objective Trajectory Planning Method for Collaborative Robot," <em>Electronics</em>, vol. 9, no. 5, article 859, 2020.</li>
      </ul>
    </section>

    <section class="section-grid">
      <article class="section-card">
        <h2>Research Experience</h2>
        <ul>
          <li><strong>Agentic AI and LLM-enabled networking:</strong> designed AgentNet for LLM-agent cooperation in low-altitude wireless networks, including agent-aware routing, session management, and context-preserving forwarding.</li>
          <li><strong>Network-aware edge intelligence:</strong> designed X-CFL to jointly consider data similarity, link quality, energy, and mobility for clustered federated learning in UAV networks.</li>
          <li><strong>Task-oriented UAV autonomy:</strong> developed HierTask for QoS-aware multi-stage UAV collaboration and task-centric many-to-many communication.</li>
          <li><strong>Programmable mobile architecture:</strong> designed OpenL3 and implemented an SDN/P4-based prototype for flexible routing, forwarding, and service coexistence.</li>
        </ul>
      </article>

      <article class="section-card">
        <h2>Projects and Service</h2>
        <ul>
          <li>Participated in national, municipal, and industry-funded projects on cloud-network convergence, intelligent computing networks, multidimensional identifiers, and unmanned swarm networking.</li>
          <li>Project experience includes the NSFC Joint Fund Key Program on trustworthy multidimensional identifiers for cloud-network convergence, an NSFC Major Research Program subproject on intelligent computing-network service orchestration, and a Beijing Natural Science Foundation project on unmanned swarm networking.</li>
          <li>Participated in China Telecom industry-academia projects on cloud-network convergence, intelligent inference, and identifier-integrated networking.</li>
          <li>Contributed to technical proposal writing, literature review, research problem formulation, and project planning.</li>
          <li>Reviewer for <em>IEEE Transactions on Network Science and Engineering</em> and <em>IEEE Transactions on Cognitive Communications and Networking</em>.</li>
        </ul>
      </article>
    </section>

    <section class="section-grid">
      <article class="section-card">
        <h2>Patents</h2>
        <ul>
          <li>S. Gao, <strong>J. Lan</strong>, Y. Zhang, T. Zheng, W. Quan, and W. Su, "Clustered Federated Learning Method, Apparatus, and Electronic Device for UAV Swarms," Chinese Patent, No. CN121865363A.</li>
          <li>S. Gao, Y. Zhang, Y. Yi, <strong>J. Lan</strong>, W. Su, and H. Zhang, "A Multicast Communication Method, System, and Electronic Device Based on 3D Geographic Location," Chinese Patent, No. CN122001807A.</li>
          <li>Two additional Chinese patent applications on QoS-aware task allocation for UAV swarms and identifier-based multicast communication are pending.</li>
        </ul>
      </article>

      <article class="section-card">
        <h2>Technical Skills</h2>
        <ul class="two-column-list">
          <li>Python</li>
          <li>C/C++</li>
          <li>MATLAB</li>
          <li>LaTeX</li>
          <li>PyTorch</li>
          <li>TensorFlow</li>
          <li>scikit-learn</li>
          <li>Pandas / NumPy</li>
          <li>SDN / P4</li>
          <li>NS-3</li>
          <li>ROS</li>
          <li>Linux</li>
        </ul>
      </article>
    </section>

    <div class="footer-note">
      I am open to research discussions and collaborations related to UAV networking, edge intelligence, programmable networks, and LLM-enabled wireless systems.
    </div>
  </div>

  <div data-lang="zh">
    <section class="profile-hero">
      <div>
        <p class="hero-kicker">个人学术主页</p>
        <h1>兰江雨</h1>
        <p class="subtitle">北京交通大学信息与通信工程博士研究生</p>
        <p>
          我的研究聚焦面向无人机与低空网络中分布式智能服务的自适应网络技术，重点关注边缘智能、学习驱动的网络优化，以及可编程路由与转发机制。
        </p>
        <p>
          近期工作探索面向联邦学习、多阶段无人机协同和大模型智能体协作的网络支撑机制，目标是在动态无线环境中提升智能服务的可靠性、灵活性与可扩展性。
        </p>
        <div class="hero-links">
          <a href="mailto:lanjiangyu@bjtu.edu.cn">lanjiangyu@bjtu.edu.cn</a>
          <a href="https://scholar.google.com/citations?user=sa89XfwAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a>
          <span>预计博士毕业时间：2026 年 12 月</span>
        </div>
      </div>
      <aside class="profile-panel">
        <dl>
          <dt>所在单位</dt>
          <dd>北京交通大学</dd>
          <dt>导师</dt>
          <dd>高帅 教授</dd>
          <dt>研究指导</dt>
          <dd>张维庭 副教授</dd>
          <dt>研究背景</dt>
          <dd>无人机网络、边缘智能、可编程网络系统</dd>
        </dl>
      </aside>
    </section>

    <section class="metric-row" aria-label="个人亮点">
      <div class="metric"><strong>6</strong><span>博士阶段一作论文与在审稿件</span></div>
      <div class="metric"><strong>4</strong><span>已公开或申请中的中国专利</span></div>
      <div class="metric"><strong>2</strong><span>IEEE 期刊审稿服务</span></div>
      <div class="metric"><strong>1</strong><span>年运营商网络工程经验</span></div>
    </section>

    <section class="wide-section">
      <h2>研究方向</h2>
      <div class="tag-list">
        <span class="tag">无人机与低空网络</span>
        <span class="tag">移动与边缘智能</span>
        <span class="tag">大模型赋能的无线与边缘网络</span>
        <span class="tag">面向网络优化的强化学习</span>
        <span class="tag">动态无线网络中的联邦学习</span>
        <span class="tag">可编程网络系统</span>
      </div>
    </section>

    <section class="section-grid">
      <article class="section-card">
        <h2>教育经历</h2>
        <div class="timeline-item">
          <div class="time">2022.09 - 2026.12 预计</div>
          <div class="role">信息与通信工程，博士</div>
          <div class="meta">北京交通大学</div>
        </div>
        <div class="timeline-item">
          <div class="time">2018.09 - 2021.06</div>
          <div class="role">电子与通信工程，硕士</div>
          <div class="meta">北京信息科技大学</div>
        </div>
        <div class="timeline-item">
          <div class="time">2014.09 - 2018.06</div>
          <div class="role">通信工程，学士</div>
          <div class="meta">北京信息科技大学</div>
        </div>
      </article>

      <article class="section-card">
        <h2>工作经历</h2>
        <div class="timeline-item">
          <div class="time">2021.07 - 2022.07</div>
          <div class="role">网络工程师</div>
          <div class="meta">中国电信</div>
        </div>
        <ul>
          <li>参与运营商级通信网络的运行维护工作。</li>
          <li>积累了网络管理与通信基础设施方面的工程实践经验。</li>
        </ul>
      </article>
    </section>

    <section class="wide-section">
      <h2>代表性论文</h2>
      <p>
        博士阶段，我围绕自适应无人机/低空网络开展研究，已主导完成 IEEE IoTJ 论文 1 篇、IEEE 会议论文 2 篇，并有 3 篇稿件分别在 IEEE TMC、IEEE TNSE 和 IEEE Communications Magazine 经修改后审稿中。
      </p>
      <h3 class="subhead">期刊论文与在审稿件</h3>
      <ul class="pub-list">
        <li><span class="pub-label">J1</span> <strong>J. Lan</strong>, S. Gao, W. Zhang, X. Hou, M. Xi, Y. Zhang, B. Lei, H. Zhang, and X. Shen, "OpenL3: Embedding Diverse Network Services into MANETs Using Multidimensional Identifier," <em>IEEE Internet of Things Journal</em>, vol. 12, no. 11, pp. 17700-17716, 2025.</li>
        <li><span class="pub-label">J2</span> <strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, D. Niyato, and H. Zhang, "X-CFL: A Cross-Layer Clustered Federated Learning Framework for UAV Networks," submitted to <em>IEEE Transactions on Mobile Computing</em>, under review after major revision.</li>
        <li><span class="pub-label">J3</span> <strong>J. Lan</strong>, S. Gao, X. Ma, W. Zhang, X. Hou, Y. Wang, and H. Zhang, "HierTask: Enabling QoS-Aware Hierarchical Task-Centric Routing for UAV Swarms," submitted to <em>IEEE Transactions on Network Science and Engineering</em>, under review after major revision.</li>
        <li><span class="pub-label">J4</span> <strong>J. Lan</strong>, S. Gao, B. Lei, W. Zhang, Y. Wang, and H. Zhang, "AgentNet: An Agent-Centric Network Architecture for LLM-Enabled Low-Altitude Wireless Networks," submitted to <em>IEEE Communications Magazine</em>, under review after minor revision.</li>
      </ul>
      <h3 class="subhead">会议论文与其他同行评议论文</h3>
      <ul class="pub-list">
        <li><span class="pub-label">C1</span> <strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "X-CFL: Enabling Cross-Layer Clustered Federated Learning in UAV Swarms," in Proc. <em>IEEE GLOBECOM</em>, 2025, pp. 4403-4408.</li>
        <li><span class="pub-label">C2</span> <strong>J. Lan</strong>, X. Ma, S. Gao, W. Zhang, and X. Hou, "Enabling QoS-Aware Multi-Stage Task Allocation in FANETs: A Hierarchical Learning Approach," accepted for publication in Proc. <em>IEEE ICC</em>, 2026.</li>
        <li><span class="pub-label">O1</span> R. Ping and <strong>J. Lan</strong> (corresponding author), "A Trustworthy Service Authorization Mechanism for Multidimensional Identifier Networks," accepted for publication in Proc. <em>ICCCS</em>, 2026.</li>
        <li><span class="pub-label">O2</span> Q. Ma, S. Gao, M. Xi, and <strong>J. Lan</strong>, "A Multi-Dimensional Identifier-Based Routing Mechanism for Flying Ad-Hoc Networks," in Proc. <em>ICCCS</em>, 2024, pp. 691-697.</li>
        <li><span class="pub-label">O3</span> <strong>J. Lan</strong>, Y. Xie, G. Liu, and M. Cao, "A Multi-Objective Trajectory Planning Method for Collaborative Robot," <em>Electronics</em>, vol. 9, no. 5, article 859, 2020.</li>
      </ul>
    </section>

    <section class="section-grid">
      <article class="section-card">
        <h2>研究经历</h2>
        <ul>
          <li><strong>智能体 AI 与大模型赋能网络：</strong>设计 AgentNet 低空无线网络架构，支撑大模型智能体协作，并研究面向智能体的路由、会话管理和上下文保持转发机制。</li>
          <li><strong>网络感知边缘智能：</strong>设计 X-CFL 跨层聚类联邦学习框架，联合考虑数据相似性、链路质量、能耗与移动性。</li>
          <li><strong>任务驱动无人机网络自治：</strong>开发 HierTask，面向多阶段无人机协同任务研究 QoS 感知任务参与决策与任务中心路由机制。</li>
          <li><strong>可编程移动网络架构：</strong>设计 OpenL3，并实现基于 SDN/P4 的原型系统，用于验证灵活路由、转发与多服务共存能力。</li>
        </ul>
      </article>

      <article class="section-card">
        <h2>项目与学术服务</h2>
        <ul>
          <li>参与国家级、市级及产学研项目，研究方向覆盖云网融合、智能算网、多维标识与无人集群网络等。</li>
          <li>参与项目包括云网融合可信多维标识相关国家自然科学基金联合基金重点项目、智能算网服务编排相关国家自然科学基金重大研究计划子课题，以及无人集群网络相关北京市自然科学基金项目。</li>
          <li>参与中国电信产学研项目，方向包括云网融合、智能推理与标识融合网络。</li>
          <li>参与技术方案撰写、文献调研、研究问题凝练与项目规划。</li>
          <li>担任 <em>IEEE Transactions on Network Science and Engineering</em> 与 <em>IEEE Transactions on Cognitive Communications and Networking</em> 审稿人。</li>
        </ul>
      </article>
    </section>

    <section class="section-grid">
      <article class="section-card">
        <h2>专利</h2>
        <ul>
          <li>高帅、<strong>兰江雨</strong>、张宇、郑涛、权伟、苏伟，“面向无人机集群的聚类联邦学习方法、装置及电子设备”，中国专利，CN121865363A。</li>
          <li>高帅、张宇、易尧、<strong>兰江雨</strong>、苏伟、张宏科，“一种基于三维地理位置的组播通信方法、系统及电子设备”，中国专利，CN122001807A。</li>
          <li>另有两项关于无人机集群 QoS 感知多阶段任务分配与基于标识的组播通信方法的中国专利申请中。</li>
        </ul>
      </article>

      <article class="section-card">
        <h2>技术能力</h2>
        <ul class="two-column-list">
          <li>Python</li>
          <li>C/C++</li>
          <li>MATLAB</li>
          <li>LaTeX</li>
          <li>PyTorch</li>
          <li>TensorFlow</li>
          <li>scikit-learn</li>
          <li>Pandas / NumPy</li>
          <li>SDN / P4</li>
          <li>NS-3</li>
          <li>ROS</li>
          <li>Linux</li>
        </ul>
      </article>
    </section>

    <div class="footer-note">
      欢迎围绕无人机网络、边缘智能、可编程网络与大模型赋能无线系统等方向开展学术交流与合作。
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
