# Input data

The notebook reads these files from the directory it runs in. None are committed to this repository.

| File | Contents | Source |
|---|---|---|
| `MasterData.parquet` | Monthly CRSP/Compustat stock panel. Columns used: `permno`, `ldate` (month), `ret`, `daret` (delisting-adjusted return), `me`, `me_lagged`, `vol`, `at`, `revt`, `cogs`, `profitA`, plus the Fama-French factors `rf`, `mktrf`, `smb`, `hml`, `rmw`, `cma`, `umd` merged by month | CRSP and Compustat via [WRDS](https://wrds-www.wharton.upenn.edu/) (licensed, cannot be redistributed); factors from the [Ken French Data Library](https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html) |
| `US_Policy_Uncertainty_Data.xlsx` | Monthly U.S. Economic Policy Uncertainty index (columns: Year, Month, EPU) | [policyuncertainty.com](https://www.policyuncertainty.com/us_monthly.html) |

`FFData.parquet` is written by the notebook itself from `MasterData.parquet`.
