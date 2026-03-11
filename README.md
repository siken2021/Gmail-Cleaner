# Gmail-Cleaner
# 📧 Gmail Cleaner

A free Google Sheets tool to analyze and clean your Gmail inbox — no installs, no extensions, everything runs inside Google.

> Built by **Diego Valdivia Vargas** · Lima, Peru

---

## 🔗 Get started

👉 [Click here to make your own copy](https://docs.google.com/spreadsheets/d/1BY7AJEkYfQDsQAg-lgePcG0Ecst6nT0RqW4LpFtdvCM/copy)

Opening the link will create a personal copy in your Google Drive. No special permissions needed upfront.

---

## 🚀 First steps

1. **Make a copy** — Open the link above and confirm the copy to your Drive.
2. **Open the menu** — In your spreadsheet, go to the top menu: `Gmail Cleaner → Open Dashboard`.
3. **Authorize permissions** — The first time, Google will ask for Gmail access. This is required to read senders and move emails to trash.
4. **Start an analysis** — Click `Start Analysis` inside the dashboard and choose how many emails to scan.

---

## 🔒 About permissions

When Google shows the **"This app is not verified"** warning, click:

- `Advanced settings`
- `Go to Gmail Cleaner (unsafe)`
- `Allow`

This warning appears because the tool is not published on the official Google Marketplace. The code is fully open — you can review every line in this repository.

The tool only reads sender, subject, and date. **Message body is never accessed.**

---

## 🗂️ Dashboard tabs

**🏠 Home**
Main screen with your inbox summary and the full senders table. You can search in real time, quick-filter by count (+100, +50, +20, spam only), select senders and delete their emails, preview subjects, or export a PDF report.

**🔍 Filters**
Filter senders by name/email, minimum and maximum count, minimum size in KB, and sort order before deleting.

**📊 Report**
Summary stats: total emails, average per sender, and top 5 senders with the most emails.

**⏱️ Recently Deleted**
History of everything deleted during the current session. Select one or more groups and click `Restore selected` to move them back to your inbox. This history clears when you close the dashboard.

---

## 🗑️ How deletion works

Emails are **moved to Gmail trash, not permanently deleted**. You have 30 days to recover them from Gmail trash before they are automatically purged.

Steps:
1. Select one or more senders using the checkboxes.
2. Click `Delete selected`.
3. Wait for the estimated email count to appear — the confirm button activates only once the calculation finishes.
4. Click `Yes, delete` to confirm.

---

## 📊 Cumulative analysis

Each analysis **adds** results to existing ones rather than replacing them. This lets you scan your inbox in parts without losing previous data.

> 💡 If you have more than 3,000 emails, run several analyses of 500 instead of one large batch. Each Apps Script session has a 6-minute execution limit.

Every time you reopen the dashboard, the sheet clears automatically so you always start fresh with up-to-date data.

---

## ❓ FAQ

**Are my emails deleted forever?**
No. They are moved to the Gmail trash. You have 30 days to recover them.

**Does the tool read my email content?**
No. It only reads sender, subject, and date. Message body is never processed.

**Why did the analysis stop halfway?**
Apps Script has a 6-minute execution limit per session. Use smaller batches (300–500) and run multiple analyses.

**Can I use it on multiple devices?**
Yes. The spreadsheet lives in your Google Drive and is accessible from any device.

**Does it work with Google Workspace accounts?**
It depends on your organization's policies. Some admins restrict Apps Script or Gmail access from scripts.

---

## 📄 License

Free to use and open source. Code visible in the Apps Script editor after copying the spreadsheet.
