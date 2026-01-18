# 📘 Views and Storage Space in SQL

---

## ❓ Does creating an SQL view use storage space in a database?

---

## ✅ Simple Answer

Creating a **normal SQL view does NOT use extra storage space** because it stores **only the SQL query**, not the actual data.

---

## 📖 Explanation 
An SQL view acts like a **virtual table**.

- It does **not** store data physically
- It stores only a **SELECT statement**
- Data is retrieved from the **base tables** each time the view is queried
- Since no data is stored, it consumes **negligible storage space**

➡️ Therefore, a **normal view does not significantly increase database storage**.

---

## ⚠️ Materialized View (Important Exception)

Some databases support **materialized views**, which behave differently.

- ✔ Stores the **actual result set**
- ✔ **Consumes storage space**
- ✔ Improves **read performance**
- ❌ Requires **manual or scheduled refresh** to stay updated

---

## 🔍 Comparison: Normal View vs Materialized View

| Feature | Normal View | Materialized View |
|------|-----------|------------------|
| Stores data | ❌ No | ✅ Yes |
| Uses storage space | Minimal | High |
| Performance | Slower | Faster |
| Data freshness | Always latest | Needs refresh |




