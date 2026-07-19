# University Textbook Management System (SQL & R)

This project implements a relational database system using SQLite to manage universities, academic departments, students, courses, and their corresponding recommended textbooks. The implementation is written in **R**, making it ideal for execution within Google Colab or Jupyter Notebook environments[cite: 1, 2].

## Project Overview
The project is designed based on a specific Entity-Relationship Diagram (ERD) and includes[cite: 2]:
1. **Schema Design & Table Creation** using SQL Data Definition Language (DDL)[cite: 1, 2].
2. **Mock Data Insertion** using SQL Data Manipulation Language (DML) to populate and test the database[cite: 1, 2].
3. **Execution of 10 Complex SQL Queries** covering joins, aggregations, subqueries, and conditional groupings (`GROUP BY` / `HAVING`)[cite: 1, 2].

---

## Entity-Relationship Diagram (ERD)
The relational schema comprises the following entities and relationships[cite: 2]:
* **UNIVERSITY (PANEPISTIMIO):** `(KodikosP, Onomasia)`[cite: 1, 2]
* **DEPARTMENT (TMHMA):** `(KodikosT, Onomasia, KodikosP)`[cite: 1, 2]
* **COURSE (MATHIMA):** `(KodikosM, Titlos, EtosSpoudwn, ExaminoSpoudwn, KodikosT)`[cite: 1, 2]
* **STUDENT (FOITHTHS):** `(KodikosF, EtosEggrafis, KodikosT)`[cite: 1, 2]
* **TEXTBOOK (SUGGRAMMA):** `(KodikosS, Titlos, Suggrafeis, ArithmosEkdosis, EtosEkdosis, EkdotikosOikos, Timi, URL)`[cite: 1, 2]
* **RECOMMENDS (PROTEINEI):** A many-to-many (M:N) relationship between Courses and Textbooks[cite: 1, 2].
* **DECLARES (DILWNEI):** A relationship tracking which Textbooks are selected by Students for specific Courses[cite: 1, 2].

---

## Tech Stack & Requirements
* **Programming Language:** R[cite: 1, 2]
* **Database Engine:** SQLite
* **R Libraries:** `DBI`, `RSQLite`
* **Development Environment:** Google Colab / Jupyter Notebook (`.ipynb`)[cite: 1, 2]

---

## Execution Instructions (Google Colab)
1. Open a new notebook on [Google Colab](https://colab.research.google.com/).
2. Change the runtime environment to **R** (`Runtime` -> `Change runtime type` -> `R`).
3. Copy and paste the code from your notebook file into a code cell.
4. Run the cell. The required packages (`DBI` and `RSQLite`) will automatically install and run the queries.

---

## SQL Queries & Sample Outputs
