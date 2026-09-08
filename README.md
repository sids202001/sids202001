<p>
  👋 Hi, I’m Siddhesh. I'm a Software Developer and Data Analyst who loves building backend systems and data tools that actually solve real problems. I recently graduated with my Master’s in Information Systems from George Mason University (May 2024), and I currently work as a Software Developer at Talviro Inc.
</p>
<p>
  Before this, I spent time as an SDE at Amazon, where I focused heavily on backend reliability, event-driven AWS pipelines, and integrating LLMs into our internal workflows. My core stack revolves around Python, SQL, and AWS. Outside of standard backend work, I spend a lot of time experimenting with generative AI (like building agents with Gemini and Claude) and writing scripts to analyze stock market data. I just really enjoy bridging the gap between raw data and functional software. 
</p>


- 📧 **Email:** [![Gmail](https://img.shields.io/badge/-siddheshs202001@gmail.com-D14836?style=flat&logo=Gmail&logoColor=white)](mailto:siddheshs202001@gmail.com)
- 👔 **LinkedIn:** [![LinkedIn](https://img.shields.io/badge/-sss20-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/sss20)
- 📞 **Phone:** ![Phone](https://img.shields.io/badge/-+1%20%28445%29%20208--2299-3A3A3A?style=flat&logo=phone&logoColor=white)
  
### 📜 Certifications

- [Data Science and Machine Learning with Python - Udemy](https://www.udemy.com/certificate/UC-4b7cf70f-2e79-4301-ab32-176eb51d4d5e/)
- [SQL for Data Analysis - Udemy](https://www.udemy.com/certificate/UC-153113dd-103b-4e7c-a66e-4beeaf648c5d/)
- [Advanced Power BI: DAX Language, Formulas, and Calculations - LinkedIn Learning](https://www.linkedin.com/learning/certificates/e3857e80994916c164d62c8826bb66dd300d7c6844c163d99bb408db0f6f4cc1?trk=share_certificate&lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_certifications_details%3BlXfuDbXvTsC5P9Cjp8Lyeg%3D%3D)
- [Learning Data Analytics: 1 Foundations - LinkedIn Learning](https://www.linkedin.com/learning/certificates/783518e251f01a3966fadeb4fd526623764b45b584b085c6506d4ea8e3fd7eb3?trk=share_certificate)
- [Microsoft Excel - Learn MS EXCEL For DATA Analysis - Udemy](https://www.udemy.com/certificate/UC-f4ce2ffb-d25c-4b1d-b4f9-3c2ab68962a8/)
- [Machine Learning & Deep Learning in Python & R - Udemy ](https://www.udemy.com/certificate/UC-951d5c9f-65ff-4f74-902d-e465cbf45ea8/)

## 🚀 Featured Engineering Projects

### 🤖 [Automated Job Application Engine](https://github.com/sids202001/autonomous-ai-job-scout)
<p align="left">
  <a href="https://github.com/sids202001/autonomous-ai-job-scout"><img src="https://img.shields.io/badge/GitHub-autonomous--ai--job--scout-181717?style=for-the-badge&logo=github" alt="Repository"/></a>
</p>

Job hunting in tech has become an exhausting, repetitive numbers game. Spending hours every day scrolling job boards, opening dozens of browser tabs, copy-pasting the same resume details into clunky ATS portals, and re-answering the exact same screening questions over and over again drains time that should be spent preparing for interviews. I built this autonomous AI job application engine to take over the entire application lifecycle on autopilot.

You give the system your resume, and it handles the rest: it automatically scrapes live software engineering openings across LinkedIn, Greenhouse, Lever, and Ashby, uses dynamic document parsing to extract your core technical skills, and filters out jobs that demand excessive experience or lack visa sponsorship. From there, an asynchronous browser agent launches real Chromium sessions to navigate the application pages, upload your resume, and fill out multi-step forms. When hit with unpredictable, open-ended screening prompts ("Why are you a fit for this role?", technical experience summaries, or custom questionnaire dropdowns), an integrated AI reasoning engine references your actual candidate background and dynamically synthesizes tailored, professional answers in real time—enforcing strict guardrails on work authorization and compensation to prevent any hallucinated answers. The system submits applications autonomously, records every entry in a local SQLite database, and broadcasts real-time status alerts to a Telegram channel, turning a grueling 20-minute manual application chore into a seamless background workflow that applies to targeted roles while you sleep.

<p align="left">
  <img src="https://img.shields.io/badge/Python_3-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python 3"/>
  <img src="https://img.shields.io/badge/Playwright-Browser_Agent-2EAD33?style=flat-square&logo=playwright&logoColor=white" alt="Playwright"/>
  <img src="https://img.shields.io/badge/AI_Agents-LLM_Guardrails-7952B3?style=flat-square" alt="AI Agents"/>
  <img src="https://img.shields.io/badge/PyPDF2-Resume_Parsing-FF6F00?style=flat-square" alt="PyPDF2"/>
  <img src="https://img.shields.io/badge/AsyncIO-Concurrency-007ACC?style=flat-square" alt="AsyncIO"/>
  <img src="https://img.shields.io/badge/SQLite-Database-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite"/>
  <img src="https://img.shields.io/badge/Telegram_API-Real--time_Alerts-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram API"/>
</p>

---

### 📈 [Real-Time Stock Market Technical Analysis Dashboard](https://github.com/sids202001/stock-market-analyzer-dashboard)
<p align="left">
  <a href="https://github.com/sids202001/stock-market-analyzer-dashboard"><img src="https://img.shields.io/badge/GitHub-stock--market--analyzer--dashboard-181717?style=for-the-badge&logo=github" alt="Repository"/></a>
</p>

Most retail financial screeners rely on expensive third-party APIs, break under strict vendor rate limits, or force users to manage multiple subscription keys. I built this full-stack market analysis platform to provide high-throughput, low-latency equity intelligence in a single browser interface—engineered as a self-contained, zero-dependency system that operates entirely without paid API keys or external database overhead.

The backend is powered by a multi-threaded Python server (`ThreadingHTTPServer`) featuring a thread-safe in-memory 2-minute TTL cache that prevents upstream request throttling during high-frequency queries. When a ticker is searched, the engine executes vectorized time-series processing via `pandas`: computing 50/200-day rolling moving average crossovers, 14-period RSI momentum distributions, exponential MACD signal lines, and 52-week Fibonacci retracement levels. In parallel, a `ThreadPoolExecutor` queries comparative peer metrics while algorithmic evaluation pipelines parse balance sheets, income statements, and cash flow data to calculate Altman Z-Score and Piotroski F-Score metrics. The server also ingests options chains to extract near-the-money implied volatility and Put/Call volume ratios. On the frontend, a lightweight vanilla ES6+ client-side architecture renders interactive Chart.js visualizations, live ticker search, and consensus data models with sub-second response times.

<p align="left">
  <img src="https://img.shields.io/badge/Python_3.9+-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python 3.9+"/>
  <img src="https://img.shields.io/badge/ThreadingHTTPServer-Concurrent_Backend-007ACC?style=flat-square" alt="ThreadingHTTPServer"/>
  <img src="https://img.shields.io/badge/In--Memory_Cache-2--min_TTL-orange?style=flat-square" alt="In-Memory Cache"/>
  <img src="https://img.shields.io/badge/pandas-Vectorized_Time--Series-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas"/>
  <img src="https://img.shields.io/badge/Algorithms-Piotroski_%7C_Altman_Z_%7C_SMA_%7C_RSI-success?style=flat-square" alt="Algorithms"/>
  <img src="https://img.shields.io/badge/Options_Engine-IV_%7C_Put--Call_Ratios-blueviolet?style=flat-square" alt="Options Engine"/>
  <img src="https://img.shields.io/badge/Chart.js-Vanilla_ES6+-FF6384?style=flat-square&logo=chartdotjs&logoColor=white" alt="Chart.js"/>
</p>

---

### 🧾 [Itemized Bill & Expense Splitter](https://github.com/sids202001/itemized-bill-splitter)
<p align="left">
  <a href="https://github.com/sids202001/itemized-bill-splitter"><img src="https://img.shields.io/badge/GitHub-itemized--bill--splitter-181717?style=for-the-badge&logo=github" alt="Repository"/></a>
</p>

Splitting a shared bill after dining out or sharing apartment expenses with friends almost always turns into an awkward math headache. Standard expense-splitting apps either force everyone into a flat equal split—which is unfair when one person ordered an expensive entrée and cocktails while another just had a side salad—or they leave you scribbling on receipts with a phone calculator trying to figure out how to divide variable sales tax, tips, and service fees without shortchanging anyone. I built this web application to solve that exact friction with mathematical fairness and zero hassle.

The application breaks down bills item-by-item and gives users four flexible ways to divide each dish: split equally across a group, assign exact dollar amounts, set custom percentages, or allocate weighted shares. What makes the engine truly fair is its proportional fee distribution algorithm: instead of naively splitting taxes and tips evenly, it calculates each person's exact percentage of the pre-tax food and drink subtotal, dynamically scaling their share of the tax, gratuity, and delivery fees based strictly on what they actually consumed. Built with an offline-first, zero-dependency architecture in pure Vanilla ES6+ and Tailwind CSS, the app loads in under 50ms on any phone or desktop browser with zero login, zero installations, and total client-side privacy. It automatically balances fractional penny rounding errors down to the cent, generates a real-time digital receipt audit log, and lets you export a pre-formatted itemized breakdown directly to WhatsApp or download a complete CSV report with a single tap.

<p align="left">
  <img src="https://img.shields.io/badge/Vanilla_ES6+-Pure_JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="Vanilla ES6+"/>
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white" alt="Tailwind CSS"/>
  <img src="https://img.shields.io/badge/Architecture-Offline--First_%7C_Zero--Dependency-success?style=flat-square" alt="Offline-First"/>
  <img src="https://img.shields.io/badge/Algorithm-Proportional_Fee_Distribution-blue?style=flat-square" alt="Financial Math"/>
  <img src="https://img.shields.io/badge/Precision-Cent_Reconciliation-blueviolet?style=flat-square" alt="Precision"/>
  <img src="https://img.shields.io/badge/Export-WhatsApp_%7C_CSV-25D366?style=flat-square&logo=whatsapp&logoColor=white" alt="Export"/>
</p>

---

### ☁️ Automated Data Release Gates (Amazon)
At Amazon, preventing invalid data from reaching production was a top priority. I worked on developing an automated validation framework using AWS Step Functions, Batch, and S3. This system served as a release gate for our pipelines, running rigorous sanity checks to actively intercept and quarantine malformed data, ensuring downstream analytics ran smoothly.

<p align="left">
  <img src="https://img.shields.io/badge/AWS-Step_Functions-FF9900?style=flat-square&logo=amazonaws&logoColor=white" alt="AWS Step Functions"/>
  <img src="https://img.shields.io/badge/AWS-Batch-FF9900?style=flat-square&logo=amazonaws&logoColor=white" alt="AWS Batch"/>
  <img src="https://img.shields.io/badge/Amazon_S3-Storage-569A31?style=flat-square&logo=amazons3&logoColor=white" alt="Amazon S3"/>
  <img src="https://img.shields.io/badge/Python-ETL_Pipelines-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python ETL"/>
  <img src="https://img.shields.io/badge/Data_Quality-Automated_Sanity_Checks-blue?style=flat-square" alt="Data Quality"/>
</p>


# 🖥️ Technical Skills: 
<p align="left">
<h2>📊 Data Analysis and Visualization Tools and Languages</h2>
<p>
    Proficient in leveraging advanced tools for comprehensive data analysis, visualization, and business intelligence.
</p>

<div>
    <a href="https://www.tutorialspoint.com/tableau/index.htm" target="_blank" rel="noreferrer">
        <img src="https://media.licdn.com/dms/image/D5612AQFE9B10TNNrzQ/article-cover_image-shrink_720_1280/0/1694984434562?e=2147483647&v=beta&t=higFgE-PTBmt66Ozvdj1ZRLYjKR5vzeZChn0xgZGGj8" alt="Tableau" width="40" height="40"/>
    </a>
    <a href="https://www.tutorialspoint.com/power_bi/index.htm" target="_blank" rel="noreferrer">
        <img src="https://upload.wikimedia.org/wikipedia/commons/c/cf/New_Power_BI_Logo.svg" alt="Power BI" width="40" height="40"/>
    </a>
    <a href="https://www.tutorialspoint.com/excel/index.htm" target="_blank" rel="noreferrer">
        <img src="https://img.icons8.com/fluency/48/000000/microsoft-excel-2019.png" alt="Excel" width="40" height="40"/>
    </a>
    <a href="https://www.w3schools.com/python/python_google_colab.asp" target="_blank" rel="noreferrer">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRohwbx4v7reD3YnRsqDuIe4kb-Lx7gc9t0AQ&s" alt="Google Colab" width="40" height="40"/>
    </a>
    <a href="https://www.rstudio.com/" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/rstudio/rstudio-original.svg" alt="RStudio" width="40" height="40"/>
</a>
      <a href="https://www.python.org" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/>
  </a>
    <a href="https://www.w3schools.com/sql/" target="_blank" rel="noreferrer">
    <img src="https://www.shutterstock.com/image-illustration/sql-file-format-3d-illustration-260nw-2343625495.jpg" alt="W3Schools SQL" width="40" height="40"/>
</a>
    <a href="https://plotly.com/python/getting-started/" target="_blank" rel="noreferrer" class="icon">
    <img src="https://plotly.com/favicon.ico" alt="Plotly" width="40" height="40"/>
</a>

<a href="https://www.tutorialspoint.com/scikit_learn/index.htm" target="_blank" rel="noreferrer">
    <img src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" alt="scikit-learn" width="40" height="40"/>
</a>

<a href="https://seaborn.pydata.org/tutorial.html" target="_blank" rel="noreferrer">
    <img src="https://user-images.githubusercontent.com/315810/92255199-f6707f80-ee9f-11ea-9b8d-182dba6a0c59.png" alt="Seaborn" width="40" height="40"/>
</a>
<a href="https://www.geeksforgeeks.org/libraries-in-python/" target="_blank" rel="noreferrer">
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRvqFFhQhO3mktREDyu7pMFtTUjyNpax8Sakg&s" alt="Python Libraries" width="40" height="40"/>
</a>
<a href="https://www.geeksforgeeks.org/natural-language-processing-nlp-tutorial/" target="_blank" rel="noreferrer">
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQRxLNJmf_BKuE63GwFk_bIP_eHZU2aZ804cg&s" alt="NLP" width="40" height="40"/>
</a>
<a href="https://matplotlib.org/stable/tutorials/index.html" target="_blank" rel="noreferrer" class="icon">
    <img src="https://matplotlib.org/stable/_static/logo2.svg" alt="Matplotlib" width="40" height="40"/>
</a>

<a href="https://pandas.pydata.org/docs/getting_started/intro_tutorials/index.html" target="_blank" rel="noreferrer">
    <img src="https://miro.medium.com/v2/resize:fit:880/0*3FLDV31fbkmVfndt.jpeg" alt="Pandas" width="40" height="40"/>
</a>

<a href="https://numpy.org/doc/stable/user/quickstart.html" target="_blank" rel="noreferrer">
    <img src="https://numpy.org/doc/stable/_static/numpylogo.svg" alt="NumPy" width="40" height="40"/>
</a>

 <a href="https://www.tensorflow.org" target="_blank" rel="noreferrer">
    <img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg" alt="tensorflow" width="40" height="40"/>
  </a>
  <a href="https://jupyter.org/documentation" target="_blank" rel="noreferrer">
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSlquQbehFaMuUwUN32KhAS4AxK7WTUtKuZBQ&s" alt="Jupyter Notebook" width="40" height="40"/>
</a>

</div>


<div>
  <h2>🌐 Web Development Technologies Tools and Languages</h2>
  <p>Experienced in building responsive web applications using both front-end and back-end technologies.</p>
  <div> 
    <a href="https://code.visualstudio.com/" target="_blank" rel="noreferrer">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/visualstudio/visualstudio-plain.svg" alt="vscode" width="40" height="40"/>
    </a>
    <a href="https://www.w3schools.com/html/" target="_blank" rel="noreferrer"> 
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="HTML5" width="40" height="40"/> 
    </a>
    <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> 
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="CSS3" width="40" height="40"/> 
    </a>
    <a href="https://www.w3schools.com/nodejs/" target="_blank" rel="noreferrer"> 
      <img src="https://cdn-icons-png.flaticon.com/512/919/919825.png" alt="Node.js" width="40" height="40"/> 
    </a>
    <a href="https://www.tutorialspoint.com/expressjs/index.htm" target="_blank" rel="noreferrer"> 
      <img src="https://media.licdn.com/dms/image/D4E12AQEBg943ptCYpg/article-cover_image-shrink_720_1280/0/1686391647921?e=2147483647&v=beta&t=sTfwUvcIfW7Fuby7hMluDfuRJK3HfYMMWc2SyZR7-GA" alt="Express.js" width="40" height="40"/> 
    </a>
    <a href="https://www.w3schools.com/js/js_json_intro.asp" target="_blank" rel="noreferrer"> 
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c9/JSON_vector_logo.svg/1200px-JSON_vector_logo.svg.png" alt="JSON" width="40" height="40"/> 
    </a>
    <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> 
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" width="40" height="40"/> 
    </a>
    <a href="https://www.mongodb.com/" target="_blank" rel="noreferrer"> 
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="MongoDB" width="40" height="40"/> 
    </a> 
    <a href="https://getbootstrap.com" target="_blank" rel="noreferrer">
      <img src="https://raw.githubusercontent.com/themedotid/bootstrap-icon/HEAD/docs/bootstrap-icon-css.png" alt="bootstrap" width="40" height="40"/>
    </a>
    <a href="https://www.apachefriends.org/index.html" target="_blank" rel="noreferrer">
      <img src="https://undsgn.com/wp-content/uploads/2018/03/XAMPP-3.jpg" alt="XAMPP" width="40" height="40"/>
    </a>
  </div>
</div>



<div>
  <h2>📱 Android Technology</h2>
 <a href="https://developer.android.com/studio" target="_blank" rel="noreferrer">
    <img src="https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/android-studio-icon.png" alt="Android Studio" width="40" height="40" />
</a>
  <a href="https://developer.android.com" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/android/android-original-wordmark.svg" alt="developerandroid" width="40" height="40"/>
  </a>
  <a href="https://www.w3schools.com/xml/" target="_blank" rel="noreferrer">
    <img src="https://cdn.vectorstock.com/i/1000v/66/98/file-xml-icon-colored-symbol-premium-quality-vector-38666698.jpg" alt="XML" width="40" height="40"/>
  </a>
  <a href="https://www.w3schools.com/java/" target="_blank" rel="noreferrer">
    <img src="https://cdn.iconscout.com/icon/free/png-256/free-java-logo-icon-download-in-svg-png-gif-file-formats--programming-language-coding-logos-icons-1720088.png?f=webp" alt="Java" width="40" height="40"/>
  </a>
</div>



  

  

<div>
  <h2>☁️ Cloud Technologies</h2>
  <a href="https://aws.amazon.com" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/>
  </a>
  <a href="https://docs.microsoft.com/en-us/learn/azure/" target="_blank" rel="noreferrer">
    <img src="https://i0.wp.com/www.wattlecorp.com/wp-content/uploads/2023/11/Cloud-Server-Hardening-for-Azure.webp?fit=1024%2C1024&ssl=1" alt="Azure Tutorials" width="40" height="40"/>
  </a>
</div>






<div>
  <h2>🌟 Additional Technologies</h2>
  <div> 
    <a href="https://docs.docker.com/get-started/" target="_blank" rel="noreferrer">
      <img src="https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/05/Docker-New.jpeg" alt="Docker" width="40" height="40"/>
    </a>
    <a href="https://www.tutorialspoint.com/postgresql/index.htm" target="_blank" rel="noreferrer">
      <img src="https://www.postgresql.org/media/img/about/press/elephant.png" alt="PostgreSQL" width="40" height="40"/>
    </a>
    <a href="https://git-scm.com/" target="_blank" rel="noreferrer">
      <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/>
    </a>
    <a href="https://app.diagrams.net/" target="_blank" rel="noreferrer">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRPRl_E1b7DCUorWhVRXXp_xza5CbbTZ79MGAErMXP9mx1niUFWGTJH-ch2mltbyZaMCso&usqp=CAU" alt="draw.io" width="40" height="40"/>
    </a>
    <a href="https://www.python.org" target="_blank" rel="noreferrer">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/>
    </a>
    <a href="https://www.mysql.com/" target="_blank" rel="noreferrer">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/>
    </a>
    <a href="https://www.mysql.com/products/workbench/" target="_blank" rel="noreferrer">
      <img src="https://support.dbconvert.com/hc/article_attachments/360015342380/MySQLWorkbench.png" alt="MySQL Workbench" width="40" height="40"/>
    </a>
       <a href="https://www.pgadmin.org/docs/pgadmin4/development/index.html" target="_blank" rel="noreferrer">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg" alt="pgAdmin" width="40" height="40"/>
    </a>
    <a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/>
    </a>
      <a href="https://www.w3schools.com/c/" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="C Language" width="40" height="40"/>
</a>

  </div>
</div>



</p>

