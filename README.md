# Logger-project
Aero Maint Logger
A lightweight, mobile‑friendly logging tool for aircraft maintenance tasks.
Built to streamline daily task entry, support partial work orders, and provide fast recall of past IAW references.

Overview
Aero Maint Logger is a simple web app designed for aviation technicians who need to quickly record maintenance actions without fighting spreadsheets on a phone. It preserves the exact column order of your existing maintenance log while adding quality‑of‑life improvements:Fast mobile formOptional NO/WO and IAW fieldsSmart IAW recall based on past tasksSupport for aircraft, engines, and off‑aircraft componentsInspector field for the signing authorityAutomatic timestampsClean JSON submission to a Google Apps Script backend

Features
Task logging with autosuggestNO/WO optional entryAsset selection (aircraft, engines, components)IAW recall from previous entriesInspector dropdown for signing authorityHours quick buttons + custom inputGoogle Apps Script backend for writing rows directly into a Google SheetPending tasks workflow for entries missing NO/WO or IAW

Structure
Logger-project/
│
├── index.html      # Frontend form and logic
├── LICENSE         # MIT License
└── README.md       # Project documentation 

Backend
The backend is a Google Apps Script web service that receives JSON from the frontend and appends rows to a Google Sheet in the exact order:DateTaskNO/WOAssetTemplateIAWInspectorHoursBackend setup instructions are included in the script comments.

Deployment
This project is designed to run on GitHub Pages:Push index.html to the root of the repoEnable GitHub Pages in Settings → PagesUse the generated URL to access the logger on any device

License
This project is licensed under the MIT License, allowing free use, modification, and distribution.






