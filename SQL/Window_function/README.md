# Window Functions — ROW_NUMBER, RANK, DENSE_RANK, NTILE

## What I learned
- When to use RANK vs DENSE_RANK vs ROW_NUMBER
- How PARTITION BY scopes the window
- NTILE for bucketing (quartiles, deciles)

## Key pattern
```sql
RANK() OVER (PARTITION BY group_col ORDER BY metric DESC)
```

## Problems solved (10/10)
| # | Problem | Platform | Difficulty | Key Function |
|---|---------|----------|------------|--------------|
| 1 | Highest-Grossing Items | DataLemur | Medium | RANK() |
| 2 | Top Fans Rank | DataLemur | Easy | DENSE_RANK() |
| ... | | | | |