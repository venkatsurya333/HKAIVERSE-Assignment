# AI Exercise 3 — Subject: Database Management Systems (CS206)

**Model:** Gemini (Educational Account)
**Date:** 23 October 2026
**Task type:** SQL query writing with explanation

---

## Task Given to AI
Write a SQL query to find the top 3 highest-paid employees from a table called 'employees' with columns: emp_id, name, department, salary. Explain each part of the query.

## Exact Prompt Used
"Write a SQL query to find the top 3 highest-paid employees from a table called 'employees' with columns: emp_id, name, department, salary. Explain each part of the query."

## AI Output

```sql
SELECT emp_id, name, department, salary
FROM employees
ORDER BY salary DESC
LIMIT 3;
```

**Explanation of each part:**
- `SELECT emp_id, name, department, salary` — retrieves the specified columns
- `FROM employees` — identifies the source table
- `ORDER BY salary DESC` — sorts rows by salary in descending order (highest first)
- `LIMIT 3` — restricts output to only the top 3 rows after sorting

**Dialect note from AI:**
- MySQL / PostgreSQL / SQLite → use `LIMIT 3`
- SQL Server → `SELECT TOP 3 ...`
- Oracle → `FETCH FIRST 3 ROWS ONLY`

## My Verification

| Check | Result |
|-------|--------|
| SELECT clause includes all required columns | ✅ Correct |
| FROM clause names correct table | ✅ Correct |
| ORDER BY salary DESC sorts highest first | ✅ Correct |
| LIMIT 3 restricts to top 3 | ✅ Correct |
| SQL Server and Oracle dialect alternatives are accurate | ✅ Correct |
| Query would execute correctly on MySQL / PostgreSQL | ✅ Verified by manual trace |

**Error found:** No errors found. The query is syntactically and logically correct for standard SQL.

## What the AI Did Well
- Query was minimal and clean — no unnecessary complexity
- Proactively mentioned dialect differences (LIMIT vs TOP vs FETCH FIRST) which is practically useful
- Explanation was line-by-line, matching how CS206 teaches query breakdown

## What Human Checking Was Still Needed
- Considered edge case: if two employees share the 3rd-highest salary, LIMIT 3 returns only one of them arbitrarily. A more precise query would use RANK() or DENSE_RANK() window functions. The AI's answer is correct for the basic prompt but does not address ties — this was a limitation I identified myself.
- Confirmed the ORDER BY + LIMIT pattern is the standard approach taught in CS206

## Additional Insight (Human-Added)
A more robust version handling ties:
```sql
SELECT emp_id, name, department, salary
FROM (
    SELECT *, DENSE_RANK() OVER (ORDER BY salary DESC) AS rnk
    FROM employees
) ranked
WHERE rnk <= 3;
```
This ensures all employees with a tied 3rd-highest salary are included.
