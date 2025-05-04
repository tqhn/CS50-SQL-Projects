# Players

**Inspired by:** CS50's Introduction to Databases with SQL  
**Topic:** Aggregation, counting, group-based filtering

---

## 🔍 Problem Summary

This problem involved analyzing a football (soccer) team database to extract statistics about players — such as team sizes, goal counts, and top scorers.

---

## 🧠 Key Concepts Used

- `COUNT()`, `AVG()`, `MAX()`
- `GROUP BY` to summarize data by team or country
- Conditional filtering using `HAVING`

---

## 📝 What I Learned
The difference between WHERE (row-level filter) and HAVING (group-level filter).
How to summarize and compare data across groups.
How SQL handles grouping when some values are NULL.

---

## 🧵 My Approach

I grouped players by their teams and countries to calculate how many players each team had. Then I filtered for top scorers and explored various statistics like average goals per team.

Example logic used:
```sql
SELECT team, COUNT(*) AS player_count
FROM players
GROUP BY team
HAVING COUNT(*) > 5;


