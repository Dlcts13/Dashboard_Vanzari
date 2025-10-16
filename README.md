# 📊 Dashboard Analiză Vânzări | SQL, Excel, Power BI

## 🧠 Descriere
Acest proiect prezintă un flux complet de analiză a datelor de vânzări — de la prelucrarea datelor brute în Excel, la modelarea relațională în SQL Server (Star Schema) și până la vizualizarea interactivă în Power BI.

Scopul proiectului este de a demonstra competențe practice în **Data Cleaning, Data Modeling și Business Intelligence**, folosind un set de date real (Online Retail Dataset).

---

## ⚙️ Tehnologii utilizate
- **Microsoft Excel** – sursa de date inițială (`vanzari.xlsx`)
- **SQL Server (SSMS)** – curățare și modelare date
- **Power BI Desktop** – dashboard interactiv și KPIs
- **GitHub** – documentare și versiuni ale proiectului

---

## 🧱 Structura proiectului
Dashboard_Vanzari/
├── data/ # fișierul Excel original

├── powerbi/ # fișierul Power BI (.pbix) + export PDF

├── sql/ # scripturi SQL (creare și populare tabele)

└── README.md # documentația proiectului

---

## 🧩 Model de date (Star Schema)
Modelul de date respectă o arhitectură în formă de stea:
dim_Produse ← fact_Vanzari → dim_Clienti
                   |
                dim_Date

---

### 🔹 Tabele:
- **dim_Produse** – detalii despre produse (StockCode, Description)
- **dim_Clienti** – informații despre clienți și țări
- **dim_Date** – calendar (DateKey, Date, Month, Year)
- **fact_Vanzari** – tranzacții (InvoiceNo, Quantity, UnitPrice, LineTotal)

---

## 📈 Dashboard (Power BI)
Dashboardul final include:
- KPI-uri principale: **Total Sales, Total Quantity, Total Customers, Average Order Value**
- Top 10 produse după vânzări
- Evoluția lunară a vânzărilor
- Distribuția vânzărilor pe țări
- Filtre interactive pentru an, țară și produs

---

## 🧮 Insight-uri cheie
- Top 10 produse generează ~60% din totalul vânzărilor
- UK contribuie cu peste 80% din venituri
- Q4 (Octombrie–Decembrie) este perioada cu cele mai mari vânzări
- Valoarea medie a unei comenzi: ~480 RON

---

## 👨‍💻 Autor
**Darius Nicolae Lăcătușu**  
📍 Bucharest, Romania  
📧 lacatusudariusnicolae@gmail.com  
🌐 [LinkedIn](https://www.linkedin.com/in/darius-nicolae-l%C4%83c%C4%83tu%C8%99u/)  
💻 [GitHub](https://github.com/Dlcts13)

---

## 📄 Licență
Proiect creat în scop educațional. Datele provin dintr-un Online Retail Dataset

