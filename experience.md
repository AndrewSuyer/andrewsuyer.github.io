---
layout: experience
title: Experience
permalink: /experience/

# Which sections to show, and in what order. Remove a name to hide that section.
section_order: [skills, experience, education, projects]

# Icons are optional. To add one, put an image in assets/icons/ and add e.g.
#   icon: /assets/icons/wpi.png
# Without one, a tile with the first letter of the name is shown.

experience:
  - company: Quantum Gears (Forum Systems)
    url: https://www.forumsys.com/
    icon: /assets/icons/quantum-gears-logo.jpg
    location: Needham Heights, MA
    role: Software Engineering Intern - AI Agents
    dates:
      - May 2025 – August 2025
      - July 2026 – August 2026
    bullets:
      - text: "Rebuilt and optimized a large language model (LLM) prompt chain for a health insurance benefits chatbot that was used by over 5 million users to answer questions about their health plans"
        children:
          - "Enhanced the input/output schema for all LLM interactions, improving output extraction reliability by 50–80%"
          - "Optimized instruction prompts using ground-truth datasets, increasing response accuracy from ~60% to ~80%"
      - text: "Developed specialized enterprise-grade AI agents that integrated into commercial software products"
        children:
          - "Deployed an agent which leverages Yahoo Finance APIs and LLM reasoning to perform financial analysis"
          - "Created web crawling agents that answer queries by searching the web, saving users hours of manual searching"
          - "Implemented an Oracle Agent Manager, an agent capable of calling other specialized Oracle Fusion agents as tools to answer complex queries about contracts, requisitions, purchase orders, and procurement activities"
      - text: "Evaluated several agent frameworks on metrics like token efficiency, extensibility, and reliability, then configured one for a developer portal"
        children:
          - "Built custom skills, plugins, and a RAG system for document retrieval, then tested the agent on a variety of use cases"

  - company: Math Altitude School of Mathematics
    url: https://www.mathaltitude.com/
    icon: /assets/icons/math-altitude.jpg
    location: Worcester, MA
    role: Mathematics Tutor, Assistant Teacher (part time)
    dates: September 2021 – May 2024
    bullets:
      - "Co-taught a computer programming course that was aimed towards a young audience (grades 4 - 6)"
      - "Tutored a wide range of students (grades 1 - 10), helping them become proficient in complex topics in programming, algebra, geometry, & trigonometry"
      - "Students gained a fresh perspective and felt more at ease working with a teacher who was also a student/peer"

education:
  - school: Worcester Polytechnic Institute (WPI)
    url: https://www.wpi.edu/
    icon: /assets/icons/wpi-goat.png
    location: Worcester, MA
    degree: B.S. and M.S. in Computer Science
    dates: August 2024 – May 2027
    bullets:
      - "Cumulative GPA: 4.0/4.0; Dean’s List all semesters"
      - "Notable courses: Software Engineering, Computer Networks, Database Systems, Object-Oriented Analysis and Design, Distributed Computer Systems, Algorithms, Operating Systems, Computational Engineering"

  - school: DeepLearning.AI, Stanford University
    url: https://www.deeplearning.ai/
    icon: /assets/icons/deeplearning-ai.png
    location: Online/Asynchronous
    degree: Machine Learning Specialization
    dates: March 2025 – May 2025
    bullets:
      - "Topics: Regression, Classification, Neural Networks, Decision Trees, Recommender Systems, Reinforcement Learning"

  - school: Doherty Memorial High School
    icon: /assets/icons/doherty.png
    location: Worcester, MA
    degree: High School Diploma
    dates: September 2020 – June 2024
    bullets:
      - "GPA 4.89/4.00, Class rank 2 (top 1%)"
      - "Senior year: dual enrollment at [Quinsigamond Community College](https://www.qcc.edu/) (Worcester, MA)"

projects:
  - name: Designing and Prototyping a Website for the Zoological Society of London’s Biobank
    url: /projects/biobank
    icon: /assets/icons/zsl.webp
    location: London, England
    role: Software Engineer - WordPress
    dates: May 2026 – July 2026
    bullets:
      - "Owned the full website lifecycle for the Zoological Society of London’s Biobank, from requirements gathering through design, development, and delivery"
      - "Surveyed 50+ prospective users and conducted follow-up interviews, then used findings to inform website design"
      - "Facilitated numerous user testing sessions, then translated user feedback into design and functionality changes"
      - "Led regular stakeholder meetings to communicate project progress and keep technical delivery aligned with business goals"

  - name: ShopComp — A receipt sharing platform to help you find the best deals
    url: /projects/shopcomp
    icon: /assets/icons/ShopComp-logo.png
    location: Worcester, MA
    role: Software Engineer - Web App
    dates: October 2025 – December 2025
    bullets:
      - "Leveraged the AWS CDK to define and deploy a RESTful API with API Gateway and Lambda Proxy integrations"
      - "Implemented CI/CD scripts to enable automated builds and deployments"
      - "Implemented user authentication with AWS Cognito, secured API Gateway endpoints with a Cognito Authorizer, then built a React login and account creation page"
      - "Coordinated regular team meetings, tracked project progress, and guided team members to ensure milestones were met"

  - name: Greendale Youth Flag Football Registration Website
    icon: /assets/icons/gyffl.jpg
    location: Worcester, MA
    role: Web Developer
    dates: December 2020 – June 2021
    bullets:
      - "Consulted with the league owner about creating a website; presented different options to the league for online proprietary tools, including benefits and costs of different options"
      - "Developed an online registration website for my community flag football team using [Sports Connect](https://sportsconnect.com/) (Blue Sombrero)"
      - "Designed a user-friendly home page which includes pictures, links to relevant pages, and instructions for how to register"
      - "Online registration process saves 100's of hours per year of manual registration management"

# Skill icons: `icon` is a devicon name (https://devicon.dev), a full URL, or a /local/path.svg.
# Tiles without a `url` are not clickable; tiles without an `icon` show a letter.
skills:
  - category: Programming Languages
    items:
      - name: JavaScript
        url: https://developer.mozilla.org/en-US/docs/Web/JavaScript
        icon: javascript
      - name: TypeScript
        url: https://www.typescriptlang.org/
        icon: typescript
      - name: Python
        url: https://www.python.org/
        icon: python
      - name: Java
        url: https://www.java.com/
        icon: java
      - name: C
        url: https://www.open-std.org/jtc1/sc22/wg14/
        icon: c
      - name: C++
        url: https://isocpp.org/
        icon: cplusplus
      - name: SQL
        icon: /assets/icons/sql.png
      - name: HTML
        url: https://developer.mozilla.org/en-US/docs/Web/HTML
        icon: html5
      - name: CSS
        url: https://developer.mozilla.org/en-US/docs/Web/CSS
        icon: css3
      - name: PHP
        url: https://www.php.net/
        icon: php
      - name: Lua
        url: https://www.lua.org/
        icon: lua
      - name: LaTeX
        url: https://www.latex-project.org/
        icon: latex

  - category: Databases
    items:
      - name: Oracle
        url: https://www.oracle.com/database/
        icon: oracle
      - name: MySQL
        url: https://www.mysql.com/
        icon: mysql
      - name: PostgreSQL
        url: https://www.postgresql.org/
        icon: postgresql

  - category: Dev Tools
    items:
      - name: Git
        url: https://git-scm.com/
        icon: git
      - name: Linux
        url: https://www.kernel.org/
        icon: linux
      - name: SSH
        url: https://www.openssh.com/
        icon: ssh
      - name: Docker
        url: https://www.docker.com/
        icon: docker
      - name: Nix
        url: https://nixos.org/
        icon: nixos
      - name: Jira
        url: https://www.atlassian.com/software/jira
        icon: jira

  - category: AI Agents
    items:
      - name: Hermes
        url: https://hermes-agent.nousresearch.com/
        icon: /assets/icons/hermes-agent.png
      - name: OpenClaw
        url: https://openclaw.ai/
        icon: /assets/icons/openclaw-agent.png
      - name: Claude Code
        url: https://claude.com/product/claude-code
        icon: /assets/icons/claude-code.png
      - name: NemoClaw
        url: https://www.nvidia.com/en-us/ai/nemoclaw/
        icon: /assets/icons/nemoclaw.png
      - name: OpenCode
        url: https://opencode.ai/
        icon: /assets/icons/opencode.png
---

# Experience

This is a full listing of all my work experience, education, and projects. See my
[projects page](/projects/) for more details about my projects. See my 
[resumes](/resume.html) for more specialized and recent listings of my experience.


