<div align="center">

# 🐼 Pandas Trials

### *Hands-on first steps with Pandas, using real retail data* 🛒

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

<sub>📍 Load it · 🔍 Explore it · 🧹 Spot the gaps · 📊 Summarize it 📍</sub>

</div>

---

## ✨ What's Inside

> A beginner-friendly notebook that walks through the **first things you do with any new dataset** — using the classic **Big Mart Sales** data.

| 📁 File | 💡 What it is |
|:--|:--|
| 📓 **`4. Pandas.ipynb`** | The notebook: an introduction to Pandas, step by step |
| 📊 **`Dataset/big_mart_sales.csv`** | 8,523 product-outlet sales records across 12 columns |

---

## 🧭 The Journey

```
  📥 Import  ──▶  👀 Peek  ──▶  📐 Shape  ──▶  🏷️ Columns  ──▶  🔢 Types  ──▶  🕳️ Nulls  ──▶  📊 Summary
```

| Step | Code | What you learn |
|:-:|:--|:--|
| 1️⃣ | `import pandas as pd` | Bring Pandas into your session |
| 2️⃣ | `pd.__version__` | Check which version you're running |
| 3️⃣ | `pd.read_csv(...)` | Load a CSV into a DataFrame |
| 4️⃣ | `data.head(3)` | Peek at the first rows |
| 5️⃣ | `data.shape` | Count rows × columns |
| 6️⃣ | `data.columns` | List every column name |
| 7️⃣ | `data.dtypes` | See the data type of each column |
| 8️⃣ | `data.isna().sum()` | Find missing values |
| 9️⃣ | `data.describe()` | Get instant summary statistics |

---

## 🛍️ Meet the Dataset

<table>
<tr>
<td align="center">📦<br><b>8,523</b><br><sub>records</sub></td>
<td align="center">🏷️<br><b>1,559</b><br><sub>unique items</sub></td>
<td align="center">🏬<br><b>10</b><br><sub>outlets</sub></td>
<td align="center">🥫<br><b>16</b><br><sub>item categories</sub></td>
</tr>
</table>

<details>
<summary><b>🔎 Click to see all 12 columns</b></summary>

<br>

| Column | Description |
|:--|:--|
| 🆔 `Item_Identifier` | Unique product ID |
| ⚖️ `Item_Weight` | Product weight |
| 🧈 `Item_Fat_Content` | Low Fat or Regular |
| 👁️ `Item_Visibility` | Share of store display area given to the product |
| 🥦 `Item_Type` | Product category (Dairy, Soft Drinks, …) |
| 💲 `Item_MRP` | Maximum retail price |
| 🏪 `Outlet_Identifier` | Unique store ID |
| 📅 `Outlet_Establishment_Year` | Year the store opened |
| 📏 `Outlet_Size` | Small / Medium / High |
| 🗺️ `Outlet_Location_Type` | City tier (Tier 1–3) |
| 🏬 `Outlet_Type` | Grocery store or supermarket type |
| 💰 `Item_Outlet_Sales` | Sales of the product at that store **(target)** |

</details>

> [!NOTE]
> 🕳️ **Missing data alert:** `Item_Weight` has **1,463** blanks and `Outlet_Size` has **2,410**, which you'll find in step 8️⃣.

---

## 🚀 Quick Start

```bash
# 1. Install the tools
pip install pandas jupyter

# 2. Launch Jupyter
jupyter notebook "4. Pandas.ipynb"
```

> [!TIP]
> 📂 The notebook reads `Dataset/big_mart_sales.csv`, so launch Jupyter from the `Pandas_Trials/` folder.

---

## 💪 What Pandas Can Do

- 📄 **Read & write** CSV, JSON, Excel, HTML and more
- 📊 **Summarize** data in a single line
- 🎯 **Filter & modify** data on multiple conditions
- 🔗 **Merge** multiple files together

---

## 📚 Keep Learning

🔗 [Official Pandas Documentation](https://pandas.pydata.org/docs/) &nbsp;•&nbsp; 🔗 [10 Minutes to Pandas](https://pandas.pydata.org/docs/user_guide/10min.html)

---

<div align="center">

**Made with 🐼 and ☕**

⭐ *If this helped you learn, give it a star!* ⭐

</div>
