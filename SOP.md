# Standard Operating Procedures (SOP)

## Daily Job Collection SOP

1. Scheduler runs at 08:00 AM (UTC+6)
2. Collect max 20 jobs per LinkedIn query
3. Collect from remote APIs
4. Store raw job data
5. Trigger AI scoring
6. Save scoring result
7. Send daily summary email

---

## Error Handling SOP

- If scraper fails → retry once
- If AI fails → mark job as "pending scoring"
- If email fails → retry twice
- All errors must be logged

---

## Manual Review SOP

- Review moderate matches (70–79)
- Manually apply where relevant
- Update application status
