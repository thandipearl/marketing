# Output Results 

This section highlights the **before vs after outputs** from the data cleaning process and what each result means.

---

## Dataset Overview Output
- **Rows:** 2,240  
- **Columns:** 12  

This confirms that the dataset is large enough for meaningful analysis and reflects a real-world scenario.

---

## Column Cleaning Output

### Before:
- Column names contained:
  - Extra spaces  
  - Inconsistent capitalization  
  - Irregular formatting  

### After:
- Column names are:
  - Lowercase  
  - Clean (no extra spaces)  
  - Separated using underscores  

This output confirms that column names are standardized and easier to work with.

---

## Spend Column Output

### Before:
- Values included symbols like:
  - `$500`
  - `$1200`

### After:
- Values converted to numeric:
  - `500`
  - `1200`

The output confirms that the column is now fully numeric and ready for calculations such as averages and totals.

---

## Channel Column Output

### Before:
- Inconsistent categories such as:
  - `Facebok`
  - `Insta_gram`
  - `Tik_Tok`
  - `Gogle`

### After:
- Standardized categories:
  - `Facebook`
  - `Instagram`
  - `TikTok`
  - `Google Ads`
  - `Email`

The output shows that all categorical values are now consistent and grouped correctly.

---

## Active Column Output

### Before:
- Mixed values:
  - `Yes`, `Y`, `1`
  - `No`, `0`

### After:
- Clean boolean values:
  - `True`
  - `False`

This confirms that the column is now properly formatted for logical operations and filtering.

---

## Date Conversion Output

### Before:
- `start_date` was of type:
  - `object` (string)

### After:
- `start_date` converted to:
  - `datetime`

This output confirms that the dates are now in a proper format for time-based analysis.

---

## Clicks vs Impressions Output

### Before Fix:
- Error occurred due to:
  - Duplicate column (`clicks`)

### After Fix:
- Output returned:
  - **Empty DataFrame**

This confirms:
- No cases where clicks exceed impressions  
- The dataset passes logical validation checks  

---

## Start Date vs End Date Output

### Before:
- Some rows had:
  - End date earlier than start date ❌  

### After:
- End dates corrected:
  - `start_date + 30 days`

The output confirms that all campaigns now follow a logical timeline.

---

## 📈 Outliers in Spend Output

### Before:
- Some spend values were extremely high (outliers)

### After:
- Outliers capped at a defined upper limit (≈ 8603)

This confirms that extreme values were controlled without removing data.

---

## Feature Extraction Output

### Before:
- Campaign name example:
  - `Q4_summer_campaign`

### After:
- New column created:
  - `season = summer`

The output confirms successful feature engineering, adding useful information for analysis.

---

## Final Output

- Cleaned dataset with:
  - No formatting issues  
  - No logical errors  
  - Standardized values  
- New features added for deeper analysis  

The final dataset is:
✔ Analysis-ready  
✔ Clean and consistent  
✔ Suitable for visualization and modeling  
