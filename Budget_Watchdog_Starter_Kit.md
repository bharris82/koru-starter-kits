# 💰 Budget Watchdog Starter Kit

**Goal:** Track overspending privately with YNAB or spreadsheets.

## What you need
- Open WebUI or AnythingLLM
- YNAB API key (or a local CSV/Google Sheet of expenses)

## Steps
1. **Connect YNAB or CSV**

   YNAB Example config:
   ```yaml
   tools:
     - name: "ynab_api"
       type: "rest"
       config:
         api_key: "YOUR_YNAB_API_KEY"
   ```

   For CSV/Google Sheets: load the file into LlamaIndex or a pgvector DB.

2. **Import a Starter Prompt**

   ```
   You are my Budget Watchdog.
   - Check my spending categories.
   - If I overspent in one, suggest a category to move money from.
   - Provide a daily summary in 3–4 bullet points.
   ```

3. **Run your first check**
   Ask: *"How is my budget today? Did I overspend anywhere?"*

## Next Step
Connect to a daily email or chat notification.
