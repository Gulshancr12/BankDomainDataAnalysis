## 🏦 Bank Domain Data Analysis – Power BI Project

### 📊 Executive Summary  
This project focuses on **risk analytics in banking and financial services**, using **Power BI** to visualize and analyze customer data.  
The dashboard helps financial institutions **make informed lending decisions** — determining whether a client is likely to repay a loan or not, thus minimizing financial risks.

---

### 🧩 Problem Statement  
> Develop a basic understanding of risk analytics in banking and financial services and analyze how data can minimize the risk of losing money while lending to customers.

---

### 💡 Solution Overview  
A **Power BI Dashboard** was designed using the latest tools to provide:
- Detailed client and loan analysis  
- Insights into deposits, loans, and fee structures  
- A data-driven approach for **loan approval decisions**

---

### 🧠 About the Dataset  
The dataset contains various interconnected tables related to banking operations:

- `Banking Relationship`  
- `Client–Banking`  
- `Gender`  
- `Investment Advisor`  
- `Period`

These tables are connected using **primary and foreign keys**, enabling relational data modeling in Power BI.

---

### 🧹 Data Cleaning & Transformation  
Performed key cleaning steps to improve data quality and analytical accuracy:

1. Created a new column **Engagement Timeframe** to calculate client duration in banks.  
2. Added **Engagement Days** column to measure total days since joining.  
3. Defined **Income Band** (`Low`, `Mid`) based on estimated income.  
4. Created **Processing Fees** column based on fee structure category.  

---

### 🧮 Calculated Functions Used  

| Function | Description | Example |
|-----------|--------------|----------|
| **SUM()** | Adds all numeric values in a column | `Bank Deposit = SUM('Clients - Banking'[Bank Deposits])` |
| **DISTINCTCOUNT()** | Counts unique values | `Total Clients = DISTINCTCOUNT('Clients - Banking'[Client ID])` |
| **SUMX()** | Evaluates an expression for each row, then sums | `Total Fees = SUMX('Clients - Banking', [Total Loan] * 'Clients - Banking'[Processing Fees])` |
| **SWITCH()** | Evaluates expressions and returns results conditionally | Used for conditional KPIs |
| **DATEDIFF()** | Returns interval difference between two dates | `Engagement Days = DATEDIFF([Joined Bank], TODAY(), DAY)` |

---

### 🎯 Key Performance Indicators (KPIs)  

- **Total Clients** – Total number of clients in the dataset  
- **Total Loan** – Sum of all banking, business, and credit loans  
- **Bank Loan** – Total amount owed by clients  
- **Business Lending** – Loan amount given to small businesses  
- **Total Deposit** – Combined deposits from all accounts  
- **Total Fees** – Amount charged for account setup and maintenance  
- **Credit Card Balance** – Outstanding credit card dues  
- **Savings Account Amount** – Total savings held  
- **Foreign Currency Account** – Non-Indian currency account values  
- **Engagement Length** – Sum of engagement days per client  

---

### 📈 Visualizations  

The Power BI dashboard contains the following pages:

- 🏠 **Home Dashboard** – Overview of all key metrics  
- 💰 **Loan Analysis** – Visual representation of loan and risk patterns  
- 🏦 **Deposit Analysis** – Deep dive into deposit trends  
- 📊 **Summary Dashboard** – Combined view of KPIs and client behavior  

---

### 🧾 Insights & Results  

- Private banks have a higher number of clients compared to other banks.  
- Identifies which nationalities have higher loan burdens.  
- Highlights total loan distribution and deposit ratios.  
- Provides understanding of customer engagement duration and repayment capability.  

---

### 🔮 Future Scope  

- Integrate **Machine Learning models** for loan default prediction.  
- Automate data refresh from SQL or cloud-based sources.  
- Add **geographical insights** and **customer segmentation** dashboards.  

---

### 🧰 Tools & Technologies  

- 🖥 **Power BI**  
- 📂 **Excel / CSV Dataset**  
- 🧮 **DAX (Data Analysis Expressions)**  

---

### 💻 Project Link  
🔗 [**View Repository**](https://github.com/Gulshancr12/BankDomainDataAnalysis)

---

### 🏁 Conclusion  
> Empowered by the latest visualization techniques, Power BI dashboards are among the most effective tools for decision-making in the banking sector.  
> This project showcases how banks can leverage analytics to optimize risk management, improve customer insights, and make better financial decisions.

---

### ✨ Author  

👨‍💻 **Gulshan Kumar Jadoun**  
🎓 *Data Science & Computer Engineering Enthusiast*  
📍 India  
💼 *Passionate about Analytics, Power BI & Data Visualization*  

---

⭐ **If you found this helpful, don't forget to star this repo!** 🌟  

---

