# Business Case: Live Quizzes for the IT Department

## 1. Problem
The IT department currently relies on ad‑hoc tools (paper, PowerPoint, or third‑party quiz platforms) for formative assessments. Lecturers spend **≈ 1 hour per week** preparing and grading quizzes, totaling **≈ 10 hours/week** across 10 lecturers. Over a 30‑week academic year this equals **300 hours** of faculty time, valued at **$3,000** (assuming $10 USD/h). The lack of instant feedback reduces student engagement and slows the learning loop.

## 2. Options
| Option | Description | One‑off cost | Annual cost | Annual benefit |
|--------|-------------|--------------|-------------|----------------|
| A | Do nothing – continue with existing manual process. | 0 | 0 | 0 |
| B | Purchase a SaaS solution (e.g., Kahoot‑style) with a license fee. | $1,800 (setup) | $1,800 (annual licence) | Saves lecturer grading time (≈ $3,000) but incurs licence cost; net benefit **$1,200**.
| C | Build the Realtime Quiz platform in‑house. | $4,900 (student & PM effort) + $300 (hosting first year) = **$5,200** | $0 (no recurring licence) | Saves grading time ($3,000) + eliminates SaaS licence ($1,800) = **$4,800** net benefit; payback ≈ **1.08 years**. |

## 3. Comparison
| Option | Net annual benefit | Payback (years) | Sensitivity (‑2 lecturers) |
|--------|--------------------|-----------------|----------------------------|
| B | $1,200 | 1.5 | $0 (benefit unchanged, cost same) |
| C | $4,800 | 1.08 | $3,600 (benefit drops to $3,600 → payback 1.44 yr) |

## 4. Benefits Not Priced
- **Increased student engagement** – measured by higher attendance and participation scores (qualitative). 
- **Improved learning outcomes** – faster feedback loops lead to better knowledge retention (to be captured in post‑semester surveys).
- **Scalability for future courses** – the platform can be reused across departments without additional licence fees.

## 5. Risks Per Option
- **Option A**: Continued inefficiency, risk of errors in manual grading, low student satisfaction.
- **Option B**: Vendor lock‑in, limited customisation, data‑privacy concerns, licence cost may increase.
- **Option C**: Development effort risk (team inexperience with WebSocket), potential schedule slip affecting MVP demo (Week 7).

## 6. Recommendation and Review Gate
We recommend **Option C – building the Realtime Quiz platform** because it delivers the greatest net benefit, eliminates recurring licence fees, and provides a reusable asset for the department. A **Week‑7 MVP review gate** will assess whether core Must features are functional and on schedule; if the MVP is not demonstrable, we will reassess scope and consider a hybrid approach with a limited SaaS component.

---

### Business‑case CSV (summary of cost calculations)

```
option,line,quantity,unit_cost,per_year,amount,formula
B,SaaS licence,10,15,12,1800,=C2*D2*E2
C,Student and PM effort (one‑off),490,10,1,4900,=C3*D3
C,Hosting,12,25,1,300,=C4*D4*E4
B,Marking time saved,300,10,1,3000,=C5*D5
C,Marking time saved,300,10,1,3000,=C6*D6
C,SaaS fee avoided,1,1800,1,1800,=C7*D7
C,Net annual benefit,,,,4500,=F6+F7-F4
C,Payback years,,,,1.09,=F3/F8
```
