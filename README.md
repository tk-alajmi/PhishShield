<!--
  README.md — PhishShield – AI-Powered Email Security & Anti-Phishing Platform
  Author: Turki Alajmi
  Notes:
  • This file mixes Markdown + inline HTML for best GitHub rendering.
  • Put images in docs/img/ and update the src paths below.
-->

<p align="center">
  <img src="https://github.com/user-attachments/assets/ad8673ff-c8bd-447b-b16d-250e7df9cb4b" alt="PhishShield Banner" width="100%" style="border-radius:14px;">
</p>

<h1 align="center">🛡️ PhishShield – AI-Powered Email Security & Anti-Phishing Platform</h1>
<p align="center"><em>“Building intelligent defense through automation, analytics, and awareness.”</em></p>

<p align="center">
  <img alt="Status" src="https://img.shields.io/badge/status-Planning%20%2B%20MVP%20Docs%20Complete-brightgreen">
  <img alt="License" src="https://img.shields.io/badge/license-MIT-blue">
  <img alt="Methodology" src="https://img.shields.io/badge/methodology-Agile%20(Sprints)-orange">
  <img alt="Security" src="https://img.shields.io/badge/security-ISO%2027001%20%7C%20NCA%20ECC--2%20aligned-purple">
</p>

<p align="center">
  <a href="#-executive-summary">Executive Summary</a> ·
  <a href="#-project-overview">Overview</a> ·
  <a href="#-goals--problem">Goals & Problem</a> ·
  <a href="#-architecture">Architecture</a> ·
  <a href="#-management-artifacts">PM Artifacts</a> ·
  <a href="#-milestones--gantt">Milestones</a> ·
  <a href="#-risk-management">Risks</a> ·
  <a href="#-rtm">RTM</a> ·
  <a href="#-sprints--lessons">Sprints & Lessons</a> ·
  <a href="#-success--kpis">Success & KPIs</a> ·
  <a href="#-future-roadmap">Roadmap</a> ·
  <a href="#-contact">Contact</a>
</p>

<hr>

<h2 id="-executive-summary">📘 Executive Summary</h2>
<p>
PhishShield is an <strong>AI-driven email security initiative</strong> designed to detect and stop phishing through <strong>real-time analysis</strong>, <strong>NLP/ML classification</strong>, and <strong>threat-intelligence enrichment</strong>. It was developed as a full <strong>Project Management Plan</strong> in La Trobe University’s <strong>CSE3PM</strong> unit using <strong>Agile sprints</strong>, and aligned to <strong>ISO/IEC 27001</strong> and <strong>Saudi NCA ECC-2</strong>. Core deliverables include Objectives & Stakeholders, Scope & Boundaries, WBS, Gantt & Milestones, Activity List, Risk Management, Resource Allocation, Communication Plan, Success Criteria, RTM, Sprint Reflections, and Project Closure.
</p>


<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/2989e83e-32b2-4063-bafc-88c6b1a84956" />


<hr>

<h2 id="-project-overview">🧩 Project Overview</h2>

<table>
  <tr><td><strong>Project Name</strong></td><td>PhishShield – AI-Powered Email Security & Anti-Phishing Platform</td></tr>
  <tr><td><strong>Duration</strong></td><td>22 Sep 2025 – 19 Oct 2025 (Two sprints)</td></tr>
  <tr><td><strong>Methodology</strong></td><td>Agile (sprint ceremonies, Jira + Confluence)</td></tr>
  <tr><td><strong>Standards</strong></td><td>ISO/IEC 27001 · NCA ECC-2 · GDPR principles · OWASP Email Security</td></tr>
  <tr><td><strong>Team</strong></td><td>Turki Alajmi (PM/Risk), Al Waleed Alajmi (Integration), Adel Bin Jaber (Model Quality), Sodararith Suong (UI/Mobile), Hussain Albaghli (Security/Compliance)</td></tr>
  <tr><td><strong>Deliverable Type</strong></td><td>Project Management Plan + Technical Concept</td></tr>
  <tr><td><strong>Collab Tools</strong></td><td>Jira (tracking), Confluence (docs), MS Project/Excel (WBS/Gantt)</td></tr>
</table>

<hr>

<h2 id="-goals--problem">🎯 Goals & Problem</h2>

<h3>Project Objectives</h3>
<ul>
  <li>Deliver a documented MVP plan by <strong>19 Oct 2025</strong> that is realistic and auditable.</li>
  <li>Target <strong>≥ 90% detection accuracy</strong> with <strong>≤ 10% false positives</strong> (pilot evaluation).</li>
  <li>Demonstrate <strong>Gmail</strong> and <strong>Microsoft 365</strong> integration feasibility.</li>
  <li>Provide <strong>user/admin dashboards</strong> with real-time alerts and severity levels.</li>
  <li>Complete <strong>DPIA outline</strong> and privacy controls (RBAC, SSO, encryption, retention).</li>
</ul>

<h3>Problem Statement</h3>
<p>
Phishing is a top initial access vector; static filters lag behind adversaries’ speed and creativity. PhishShield closes the gap via <strong>context-aware NLP</strong>, <strong>ML classification</strong>, and <strong>live TI enrichment</strong>, with clear governance for privacy and risk.
</p>


<hr>

<h2 id="-architecture">🏗️ Architecture</h2>

<p><strong>High-Level Components</strong></p>
<pre>
[Mail Ingestor] → [Backend API] → [ML/NLP Classifier] → [Threat Intel Enrichment]
                                     ↓
                              [Data Store / Logs]
                                     ↓
                            [Dashboard & Alerts]
</pre>

<ul>
  <li><strong>Detection Engine</strong>: NLP features (headers/body/URLs/attachments), heuristics, and classification (Legitimate / Suspicious / Phishing)</li>
  <li><strong>Threat Intelligence</strong>: Google Safe Browsing, VirusTotal, PhishTank (URL/file reputation)</li>
  <li><strong>Backend</strong>: Node/Express or Django/Flask REST services for analyze/query/report</li>
  <li><strong>UI</strong>: React / React Admin with Tailwind, charts for triage and trend analysis</li>
  <li><strong>Security</strong>: Auth0/Firebase, RBAC, TLS, KMS at rest, audit logging</li>
</ul>



<hr>

<h2 id="-management-artifacts">🗂️ Management Artifacts</h2>

<h3>Stakeholders & Roles</h3>
<table>
  <thead><tr><th>Name</th><th>Role</th><th>Responsibility</th></tr></thead>
  <tbody>
    <tr><td><strong>Turki Alajmi</strong></td><td>PM / Risk Lead</td><td>Risk governance, Jira/Confluence alignment, documentation</td></tr>
    <tr><td><strong>Al Waleed Alajmi</strong></td><td>Integration</td><td>APIs, quotas, mail platform feasibility</td></tr>
    <tr><td><strong>Adel Bin Jaber</strong></td><td>Model Quality</td><td>Data, features, evaluation</td></tr>
    <tr><td><strong>Sodararith Suong</strong></td><td>UI/Mobile</td><td>Dashboard UX, stability</td></tr>
    <tr><td><strong>Hussain Albaghli</strong></td><td>Security/Compliance</td><td>DPIA, RBAC, encryption & controls</td></tr>
  </tbody>
</table>

<h3>Scope & Boundaries</h3>

<table>
  <tr>
    <td><strong>In Scope</strong></td>
    <td>
      Real-time detection (NLP/ML); Gmail + M365 integration; Web/Mobile dashboards;
      Threat Intel (GSB, VT, PhishTank); Alerts & severity; GDPR controls (DPIA, RBAC,
      encryption, retention); Training & awareness prompts; Cloud deployment (AWS/Azure/Firebase).
    </td>
  </tr>
  <tr>
    <td><strong>Out of Scope</strong></td>
    <td>
      Full production SOC; third-party email hosting beyond pilot; enterprise SIEM integration;
      billing & multi-tenant models.
    </td>
  </tr>
  <tr>
    <td><strong>Constraints</strong></td>
    <td>
      Two-sprint timeline (22 Sep – 19 Oct 2025); limited academic resources & API quotas;
      sandbox testing only (no live prod data).
    </td>
  </tr>
  <tr>
    <td><strong>Assumptions</strong></td>
    <td>
      Test tenants & datasets available; vendor APIs remain stable; weekly team syncs.
    </td>
  </tr>
</table>



<hr>

<h2 id="-wbs">🧱 Work Breakdown Structure (WBS v1.1)</h2>

<p><strong>Level 1 (WBS 1.0 – 11.0)</strong></p>
<ol>
  <li>Initiation & Planning</li>
  <li>Requirements & Analysis</li>
  <li>Architecture & Design</li>
  <li>Detection Engine Development</li>
  <li>Dashboards (Web/Mobile)</li>
  <li>Integration & Alerts</li>
  <li>Testing & QA</li>
  <li>Deployment & Operations</li>
  <li>Security / Privacy / Compliance</li>
  <li>Project Controls & Documentation</li>
  <li>Handover & Closure</li>
</ol>



<hr>

<h2 id="-milestones--gantt">🗓️ Milestones & Gantt</h2>

<table>
  <thead><tr><th>Milestone</th><th>Date</th><th>Outcome</th></tr></thead>
  <tbody>
    <tr><td>Tools Ready (Jira/Confluence)</td><td>23 Sep 2025</td><td>Collaboration configured</td></tr>
    <tr><td>Charter Approved</td><td>25 Sep 2025</td><td>Baseline authorized</td></tr>
    <tr><td>Requirements Baseline</td><td>03 Oct 2025</td><td>Scope locked</td></tr>
    <tr><td>UX Prototypes Approved</td><td>02 Oct 2025</td><td>Design validated</td></tr>
    <tr><td>Detection Engine Prototype</td><td>05 Oct 2025</td><td>Functional prototype</td></tr>
    <tr><td>Real-Time Alerting</td><td>08 Oct 2025</td><td>Live monitoring</td></tr>
    <tr><td>Alert Center & Dashboard</td><td>10 Oct 2025</td><td>UI integration</td></tr>
    <tr><td>Cloud Security Enforced</td><td>16 Oct 2025</td><td>RBAC + TLS setup</td></tr>
    <tr><td>UAT (Pilot) Accepted</td><td>17 Oct 2025</td><td>Feedback closed</td></tr>
    <tr><td>MVP Go-Live & Closure</td><td>19 Oct 2025</td><td>Delivered</td></tr>
  </tbody>
</table>



<hr>

<h2 id="-activity-list">🧩 Activity List & Dependencies</h2>

<p>
The activity list maps each WBS work package to granular tasks with owners and dependencies (tracked in Jira). Sequencing emphasizes early risk/quality gates before integration work, reducing rework during UI and alerting assembly.
</p>



<hr>

<h2 id="-risk-management">⚙️ Risk Management</h2>

<h3>Approach</h3>
<ul>
  <li>Iterative cycle per sprint: <strong>Identify → Assess → Respond → Monitor</strong></li>
  <li>Qualitative matrix: <strong>Probability × Impact</strong> prioritization</li>
  <li>Responses: <strong>Avoid</strong>, <strong>Mitigate</strong>, <strong>Transfer</strong>, <strong>Accept</strong></li>
  <li>Governance: Risk Lead = <strong>Turki</strong>; owners by domain</li>
</ul>

<h3>Top Risks & Owners</h3>
<table>
  <thead><tr><th>Risk</th><th>Rating</th><th>Owner</th><th>Primary Treatment</th></tr></thead>
  <tbody>
    <tr><td>Vendor API quota exhaustion</td><td>High × High</td><td>Al Waleed</td><td>Quota monitoring; fallback TI; caching; request shaping</td></tr>
    <tr><td>GDPR non-compliance</td><td>High × High</td><td>Hussain</td><td>DPIA; data minimization; anonymization; access logging</td></tr>
    <tr><td>UI/UX instability</td><td>High × Medium</td><td>Sodararith</td><td>Component tests; UX review; performance budget</td></tr>
    <tr><td>Cloud misconfiguration</td><td>Medium × High</td><td>Hussain</td><td>Baseline IaC; least privilege; CIS benchmarks</td></tr>
    <tr><td>3rd-party breach</td><td>Low × High</td><td>Turki</td><td>Vendor assessment; API scoping; secrets rotation</td></tr>
  </tbody>
</table>



<hr>

<h2 id="-resources">👥 Resource Allocation</h2>
<p>Balanced workloads across Sprint 1 (planning foundation) and Sprint 2 (governance completeness + integration readiness).</p>



<hr>

<h2 id="-communication">💬 Communication Plan</h2>

<table>
  <thead><tr><th>Audience</th><th>Channel</th><th>Frequency</th><th>Purpose</th></tr></thead>
  <tbody>
    <tr><td>Project Team</td><td>Jira / Confluence / Teams</td><td>Daily</td><td>Progress, blockers, decisions</td></tr>
    <tr><td>Tutor / Supervisor</td><td>Email + Meeting</td><td>Weekly</td><td>Review, approvals</td></tr>
    <tr><td>Stakeholders</td><td>Presentation + Confluence</td><td>Bi-Weekly</td><td>Status, risks, demos</td></tr>
    <tr><td>PM</td><td>Jira dashboards</td><td>Continuous</td><td>Velocity, burndown</td></tr>
  </tbody>
</table>



<hr>

<h2 id="-success--kpis">📊 Success Factors & KPIs</h2>

<ul>
  <li><strong>Technical</strong>: Stable architecture; Gmail/M365 + TI APIs integrated; Model accuracy ≥ 90%, FP ≤ 10%</li>
  <li><strong>Security & Compliance</strong>: DPIA before go-live; RBAC/SSO; encryption in transit/at rest; audit logs</li>
  <li><strong>Usability</strong>: Dashboards pass usability tests; UAT satisfaction ≥ 80%</li>
  <li><strong>Team & Execution</strong>: Balanced workload; timely ceremonies; traceability in Jira/Confluence</li>
</ul>



<hr>

<h2 id="-rtm">🧾 Requirements Traceability Matrix (RTM)</h2>
<p>
RTM links requirements → design → implementation → test artifacts → acceptance. It ensured that success criteria and risk treatments were verifiably addressed across sprints and during handover.
</p>



<hr>

<h2 id="-execution-monitoring">📈 Execution & Monitoring Readiness</h2>
<ul>
  <li><strong>Jira</strong> for daily tracking & sprint progress</li>
  <li><strong>Confluence</strong> for documentation & version control</li>
  <li><strong>Weekly</strong> sprint reviews, retrospectives, and risk/issue updates</li>
  <li><strong>Comms</strong>: standing updates via meetings, reports, Confluence pages</li>
</ul>

<hr>

<h2 id="-sprints--lessons">🏁 Sprints & Lessons</h2>

<h3>Sprint 1 — Foundation</h3>
<ul>
  <li>Jira & Confluence environments structured</li>
  <li>Core planning docs (T1–T5) completed, reviewed, versioned</li>
  <li>Collaboration & document sharing rules established</li>
</ul>

<h3>Sprint 2 — Governance & Integration Readiness</h3>
<ul>
  <li>Risk, communication, and resource plans expanded</li>
  <li>Dependencies integrated among T6–T10 and RTM</li>
  <li>Traceability, risk transparency, and stakeholder alignment achieved</li>
</ul>

<h3>Lessons Learned</h3>
<ul>
  <li><strong>Team coordination matters</strong>: Early Jira/Confluence alignment avoided confusion</li>
  <li><strong>Structure before speed</strong>: Clear scope/WBS/milestones simplified later tasks</li>
  <li><strong>Communication is a tool</strong>: Short syncs + transparent updates improved trust</li>
  <li><strong>Risk thinking early pays off</strong>: Planning risks first made resource allocation logical</li>
  <li><strong>Traceability builds quality</strong>: Linking every requirement/success factor improves validation</li>
</ul>



<hr>

<h2 id="-closure">📦 Handover & Closure</h2>
<ul>
  <li>Final documentation package delivered</li>
  <li>Review against Success Criteria and RTM</li>
  <li>Knowledge transfer via Confluence + recorded demo</li>
  <li>Client sign-off and feedback session</li>
  <li>Project closure report and lessons learned</li>
</ul>



<hr>

<h2 id="-api-sample">📡 API Sample (Concept)</h2>

<details>
  <summary><code>POST /api/v1/analyze</code> — Score & Enrich Email</summary>
  <pre>{
  "headers": {"from":"alerts@bank.com","subject":"Urgent: account locked"},
  "body": "Please verify your account at https://example-secure-login.com",
  "attachments": [],
  "meta": {"messageId":"&lt;abc@mx&gt;","receivedAt":"2025-10-02T09:22:31Z"}
}</pre>
  <p><strong>Response</strong></p>
  <pre>{
  "classification":"Phishing",
  "severity":"High",
  "score":0.94,
  "signals":{
    "nlp":{"terms":["urgent","verify","locked"]},
    "urls":[{"url":"https://example-secure-login.com","reputation":"malicious"}],
    "auth":{"spf":"fail","dmarc":"none","dkim":"fail"}
  },
  "caseId":"CASE-002134"
}</pre>
</details>

<hr>

<h2 id="-security">🔐 Security & Privacy (Mapping)</h2>

<table>
  <thead><tr><th>Area</th><th>Practices</th><th>Mapping</th></tr></thead>
  <tbody>
    <tr><td>Access Control</td><td>Auth0/Firebase, RBAC, least privilege</td><td>ISO 27001 A.9, NCA ECC-2 IAM</td></tr>
    <tr><td>Crypto</td><td>TLS in transit, KMS at rest, rotation</td><td>ISO 27001 A.10, NCA ECC-2 CRY</td></tr>
    <tr><td>Ops Sec</td><td>Secure SDLC, SAST, dependency scans</td><td>ISO 27001 A.12, OWASP ASVS</td></tr>
    <tr><td>Privacy</td><td>DPIA, minimization, anonymization</td><td>ISO 27701, GDPR</td></tr>
    <tr><td>Logging</td><td>Immutable audit logs, time sync</td><td>ISO 27001 A.12.4, NCA ECC-2 LOG</td></tr>
  </tbody>
</table>

<hr>

<h2 id="-future-roadmap">🔮 Future Enhancements & Roadmap</h2>
<ul>
  <li>Wazuh SIEM integration for live alert simulation</li>
  <li>Public Flask demo endpoint for inference showcase</li>
  <li>Active learning loop (analyst feedback → retrain)</li>
  <li>Mobile phishing (SMS/social) coverage</li>
  <li>SOC campaign analytics (trends, actors, lures)</li>
</ul>

<hr>

<h2 id="-contact">🌐 Contact</h2>
<p>
  📧 <a href="mailto:21934095@students.latrobe.edu.a">Email Turki Alajmi</a><br>
  💼 <a href="https://www.linkedin.com/in/turki1alajm1">LinkedIn</a><br>
  📍 Australia · Melbourne
</p>
