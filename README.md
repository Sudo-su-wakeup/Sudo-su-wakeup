<div align="center">

  <!-- Interactive Typing Animation Header -->
  <a href="https://github.com/Sudo-su-wakeup">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1000&color=00F3FF&center=true&vCenter=true&width=700&height=50&lines=Hi%2C+I'm+Manish+Yadav+%F0%9F%91%8B;Aspiring+Cloud+%26+DevOps+Engineer+%E2%98%81%EF%B8%8F;Final-Year+MCA+(Cloud+Computing)+%F0%9F%8E%93;Linux+%7C+Bash+%7C+AWS+%7C+Docker+%7C+Terraform+%7C+K8s;Building+Automated+%26+Reliable+Infrastructure+%E2%9A%99%EF%B8%8F" alt="Typing Animation" />
  </a>

  <p align="center">
    <b>Turning cloud concepts into resilient, production-ready architectures.</b>
  </p>

  <!-- Interactive Social & Profile Badges -->
  <a href="https://github.com/Sudo-su-wakeup?tab=repositories" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-0d1117?style=for-the-badge&logo=git&logoColor=00f3ff" alt="Portfolio" />
  </a>
  &nbsp;
  <a href="https://www.linkedin.com/in/manish-yadav-a1a280263/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  &nbsp;
  <a href="mailto:manishyadav192004@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=Sudo-su-wakeup&label=Profile%20Views&color=00f3ff&style=for-the-badge" alt="Profile Views" />

</div>

<br>

---

### 👨‍💻 About Me

- 🎓 **Education:** Final-Year MCA Student specializing in **Cloud Computing**.
- 🎯 **Career Goal:** Aspiring **Cloud & DevOps Engineer** focused on Infrastructure as Code, CI/CD automation, and cloud scalability.
- 🐧 **Core Learning Stack:** Linux Administration, Bash Scripting, AWS, Docker, Kubernetes, Terraform, Git, and CI/CD pipelines.
- 💻 **Operating Environment:** Windows 11 Pro host paired with WSL2 (Ubuntu), Linux Virtual Machines, and AWS cloud sandboxes.
- 🌟 **Engineering Philosophy:** *"Automate repetitive manual operations, codify infrastructure, and design systems for high availability."*

---

### 🛠️ Tech Stack & Tooling

<div align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=linux,bash,aws,azure,docker,kubernetes,terraform,git,github,python,ubuntu&theme=dark" alt="Technical Stack" />
  </a>
</div>

---

### 🏗️ Featured Engineering Architecture (Collapsible Deep Dive)

<details>
  <summary><b>📐 [CLICK TO EXPAND] Production-Ready 3-Tier Web Architecture on AWS</b></summary>
  <br>

```
                       [ Internet Users ]
                               │
                       [ Route 53 DNS ]
                               │
                    [ CloudFront / HTTPS ]
                               │
                 [ Internet Gateway (VPC Entry) ]
                               │
               ┌───────────────┴───────────────┐
               │    Application Load Balancer  │ (Public Subnets, Multi-AZ)
               └───────────────┬───────────────┘
                               │ (Target Group / Health Checks)
        ┌──────────────────────┴──────────────────────┐
        ▼                                             ▼
  [ AZ-1 Web / App Tier ]                       [ AZ-2 Web / App Tier ]
  EC2 Auto Scaling Group                        EC2 Auto Scaling Group
  (Private Subnets)                             (Private Subnets)
  Traffic restricted to ALB                     Traffic restricted to ALB
        │                                             │
        └──────────────────────┬──────────────────────┘
                               │ (Database Port 5432 / 3306)
                               ▼
                [ Multi-AZ Database Subnets ]
                Amazon RDS (Primary & Standby)
                Isolated, encrypted at rest via KMS
```

#### Architecture Breakdown

1. **Presentation / Web Tier (Public Subnets):**
   - Deployed across 2 Availability Zones for high availability.
   - **Internet Gateway** provides ingress/egress to the public subnets.
   - **Application Load Balancer (ALB)** terminates SSL/TLS and distributes incoming traffic evenly across healthy backend targets.

2. **Application / Logic Tier (Private Subnets):**
   - **EC2 instances inside an Auto Scaling Group (ASG)** scale dynamically based on CPU/traffic thresholds.
   - Hosted in isolated private subnets with **zero direct public internet access**.
   - Outbound internet access for software updates handled via **NAT Gateways**.
   - Security Groups enforce strict least privilege: only traffic from the ALB security group is permitted.

3. **Database / Data Tier (Secure Database Subnets):**
   - **Amazon RDS (PostgreSQL/MySQL)** deployed in a Multi-AZ standby configuration for automated failover.
   - Placed in dedicated DB subnets inaccessible from the public internet.
   - Data encrypted at rest via **AWS KMS** and in transit using SSL.

4. **Security, Automation & Observability:**
   - **Infrastructure as Code (IaC):** Modular Terraform templates with remote state locking in S3 + DynamoDB.
   - **IAM Security:** EC2 Instance Profiles configured with Principle of Least Privilege (PoLP).
   - **Monitoring:** CloudWatch Metrics, Alarms, and VPC Flow Logs enabled for security telemetry.

---

#### 🐧 Live Scripting Project: Linux System Health Reporter
- **Repository:** [`linux-system-health-reporter`](https://github.com/Sudo-su-wakeup/linux-system-health-reporter)
- **Tech Stack:** Bash, Linux, AWS EC2
- **Capabilities:** Real-time CLI telemetry capturing hostname, OS kernel releases, system uptime, memory usage, and root disk capacity across cloud instances.

</details>

---

### 📊 Live GitHub Analytics

<div align="center">
  <table border="0">
    <tr>
      <td align="center">
        <img src="https://github-readme-stats.vercel.app/api?username=Sudo-su-wakeup&show_icons=true&theme=tokyonight&bg_color=0d1117&border_color=162b4c&title_color=00f3ff&text_color=e2e8f0&icon_color=bd00ff" alt="GitHub Stats" width="410" />
      </td>
      <td align="center">
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=Sudo-su-wakeup&theme=tokyonight&background=0d1117&border=162b4c&stroke=00f3ff&ring=bd00ff&fire=00f3ff&currStreakLabel=00f3ff" alt="GitHub Streak" width="410" />
      </td>
    </tr>
    <tr>
      <td align="center" colspan="2">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Sudo-su-wakeup&layout=compact&theme=tokyonight&bg_color=0d1117&border_color=162b4c&title_color=00f3ff&text_color=e2e8f0" alt="Top Languages" width="410" />
      </td>
    </tr>
  </table>
</div>

---

### 🐍 Contribution Activity Snake

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Sudo-su-wakeup/Sudo-su-wakeup/output/github-contribution-grid-snake-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Sudo-su-wakeup/Sudo-su-wakeup/output/github-contribution-grid-snake.svg">
    <img alt="GitHub Contribution Grid Snake" src="https://raw.githubusercontent.com/Sudo-su-wakeup/Sudo-su-wakeup/output/github-contribution-grid-snake.svg">
  </picture>
</div>

---

<div align="center">
  <a href="https://github.com/Sudo-su-wakeup?tab=repositories">
    <img src="https://img.shields.io/badge/Browse%20My%20Repositories-0d1117?style=for-the-badge&logo=github&logoColor=00f3ff" alt="Browse Repositories" />
  </a>
  <br><br>
  <sub><code>[EOF] CONNECTION TERMINATED — SESSION SAVED</code></sub>
</div>
