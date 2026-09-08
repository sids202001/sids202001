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

## 🚀 What I've Been Building

* **Autonomous AI Job Scout (`autonomous-ai-job-scout`)**
  An autonomous AI browser agent built with Python and Playwright to automate the repetitive tech job application lifecycle across LinkedIn, Greenhouse, Lever, and Ashby.
  * **How it Works & Technical Architecture:** Uses `PyPDF2` to dynamically extract technical skill vectors from PDF resumes and generate targeted search queries. Upstream regex filters automatically drop roles requiring >3 years of experience or lacking visa sponsorship (OPT/H-1B). Launches asynchronous Chromium sessions to navigate multi-step ATS workflows, uploads resumes, and injects native browser events to bypass synthetic React input blocks.
  * **AI & Guardrails:** Integrates an LLM reasoning engine to contextually resolve unpredictable open-ended screening questions (*"Why this company?"*, technical background blurbs) and map custom dropdowns. Non-negotiable fields (work authorization, salary thresholds, clearance) pull from hardcoded deterministic profile rules to eliminate hallucination risks.
  * **Practical Usage:** Runs as a background pipeline that discovers openings, fills forms, submits applications, records transactions in a local SQLite database (`jobs.db`), and streams real-time status alerts to a private Telegram channel.
  * *Key Skills:* Python 3, Playwright (Chromium), LLM Prompt Orchestration & Guardrails, PyPDF2, AsyncIO, SQLite, Telegram Bot API.

* **Stock Market Analyzer Dashboard (`stock-market-analyzer-dashboard`)**
  A high-throughput equity intelligence platform delivering real-time technical indicators, options analytics, and automated financial research with zero API key dependencies.
  * **How it Works & Technical Architecture:** A multi-threaded Python backend (`ThreadingHTTPServer`) connects directly to Yahoo Finance via `yfinance`. Implements an in-memory 2-minute TTL cache protected by `threading.Lock` across bulk price and macro queries, eliminating upstream `429 Too Many Requests` rate-limiting and cutting network egress by over 70%.
  * **Quantitative Math & AI Synthesis:** Processes raw pandas price matrices to compute 50/200 SMA crossovers (Golden/Death Crosses), 14-period RSI (Wilder's smoothing), MACD (12/26/9 EMA), and 52-week Fibonacci swing levels. Pipes balance sheets, cash flow, debt-to-cash ratios, and EPS surprises into an LLM reasoning engine to automatically generate executive-level Moat, Catalyst, and Stop-Loss briefs.
  * **Practical Usage:** Investors and traders run the server locally to monitor 20+ live equities classified by Buy/Hold/Avoid technical badges, search any global ticker (e.g., `AAPL`, `NVDA`, `RELIANCE.NS`), inspect options chain liquidity, and validate trade setups in sub-second Canvas charts rendered via Chart.js.
  * *Key Skills:* Python 3, ThreadingHTTPServer, Generative AI Financial Reasoning, yfinance, pandas, NumPy, Chart.js, In-Memory Caching.

* **Itemized Bill & Expense Splitter (`itemized-bill-splitter`)**
  A zero-dependency, client-side financial application engineered to eliminate regressive cost burdens on shared dining and household tabs through mathematically fair tax and tip attribution.
  * **How it Works & Technical Architecture:** Instead of naive flat splits ($\text{Total} / N$) that force lower spenders to cross-subsidize others' extra fees, the engine implements a consumption-weighted proportional attribution algorithm:
    $$\text{Member Fee Liability} = \text{Total Extra Fees} \times \left(\frac{\text{Member Pre-Tax Subtotal}}{\sum \text{All Pre-Tax Subtotals}}\right)$$
    Accommodates 4 discrete partitioning paradigms: Equal Split, Exact Dollar ($) with an automated "Fill Remaining" deficit solver, Percentages (%), and Weighted Ratio Shares (x:y). Eliminates JavaScript IEEE-754 floating-point rounding drift using integer-cent reconciliation.
  * **Practical Usage:** Open the web app on any mobile or desktop browser at a restaurant table with zero login or setup. Log receipt items, assign who ordered what, enter the bill's total tax and tip, and tap "Copy Bill for WhatsApp" to instantly paste an itemized breakdown into the group chat for immediate settlement via Venmo or Zelle.
  * *Key Skills:* Vanilla JavaScript (ES6+), Financial Allocation Algorithms, Tailwind CSS, Offline-First Architecture, Data URI CSV & Clipboard API.

* **Automated Data Release Gates (Amazon)**
  At Amazon, preventing invalid data from reaching production was a top priority. I worked on developing an automated validation framework using AWS Step Functions, Batch, and S3. This system served as a release gate for our pipelines, running rigorous sanity checks to actively intercept and quarantine malformed data, ensuring downstream analytics ran smoothly.
  * *Key Skills:* AWS Step Functions, AWS Batch, Amazon S3, Python, ETL, Data Sanity Checks, Data Validation.


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

