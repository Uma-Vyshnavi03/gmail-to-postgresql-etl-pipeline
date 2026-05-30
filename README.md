# 📥 Automated Gmail to PostgreSQL ETL Pipeline

An end-to-end automation pipeline that extracts CSV 
file attachments from Gmail and automatically loads 
them into a PostgreSQL database — eliminating manual 
data imports entirely.

---

## 💡 Problem Statement

Monthly data files arrive as CSV attachments in Gmail. 
Manually downloading, cleaning, and importing them 
into a database is repetitive and time-consuming. 
This pipeline automates the entire process from 
email inbox to database table.

---

## ⚙️ How It Works

1. **Gmail Trigger** — n8n monitors Gmail inbox for 
   emails with CSV attachments
2. **File Extraction** — CSV attachment is extracted 
   automatically from the email
3. **Supabase Connection** — CSV data is loaded into 
   Supabase, which provides a managed PostgreSQL 
   database
4. **PostgreSQL Insert** — Data is inserted directly 
   into the target database table via PostgreSQL 
   node in n8n
5. **Result** — Database is updated automatically 
   every time a new CSV arrives in Gmail, 
   with zero manual intervention

---

## 🔧 Workflow Architecture
Gmail Inbox
↓
n8n Gmail Node (trigger on new email with attachment)
↓
Extract CSV Attachment
↓
Supabase (PostgreSQL connection)
↓
PostgreSQL Insert Node
↓
Data loaded into database ✅

> 📸 Workflow screenshot will be added once 
> Supabase project is resumed

---

## 🛠️ Tools Used

- **n8n** — workflow automation platform
- **Gmail API** — email monitoring and attachment extraction
- **Supabase** — managed PostgreSQL database hosting
- **PostgreSQL** — target database for CSV data storage

---

## 🎯 Key Concepts Demonstrated

- ETL pipeline design (Extract, Transform, Load)
- API-based email automation
- Cloud database integration
- Automated data ingestion without manual imports
- No-code/low-code workflow orchestration

---

## 📌 Use Case

Any business that receives regular data reports 
via email can use this pipeline to automatically 
keep their database updated — saving hours of 
manual work every month.
