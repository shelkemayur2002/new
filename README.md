<a id="top"></a>

#  ERP(Enterprise Resource Planning) SYSTEM
---
##  Introduction

This document contains a comprehensive and structured list of defects identified across the four GTVL portals during exploratory testing. All bugs are organized module-wise to maintain clarity and ensure easy review. Shortcut navigation links are provided at the top of the file to allow reviewers to directly jump to each portal’s bug list. Every bug entry follows a standardized format to maintain consistency, improve readability, and help developers quickly understand the issue, its expected behavior, and supporting evidence.

---

##  Bug Fields Used

Each bug in this document is documented using the following fields:

- **Bug-id**  
- **Description**  
- **Expected**  
- **Actual**  
- **Category**  
- **Severity**  
- **Evidence**

---


**Click below to navigate directly to the bug list for each portal:-**

[1.Management Portal](#management-portal)

* The GTVL Management Portal serves as the administrative control center where SKUs, Stores, Supervisors, and Promodizers are managed.
* During testing, multiple functional validation issues, missing actions, and UI/UX inconsistencies were identified. Major problems include non-functional action icons, lack of input validation, duplicate data acceptance, and broken filtering controls.
* Overall, the portal requires improvements in form validations, interactive actions, and filter management to ensure a smooth administrative workflow.

| Bug-ID | Title |
|--------|--------|
| [P1-BG-1](#P1-BG-1) | SKU action icons not working |
| [P1-BG-2](#P1-BG-2) | No Clear Filters in SKU list |
| [P1-BG-3](#P1-BG-3) | Duplicate SKU code allowed |
| [P1-BG-4](#P1-BG-4) | ZIP field accepts alphabets |
| [P1-BG-5](#P1-BG-5) | Phone number cannot be deleted |
| [P1-BG-6](#P1-BG-6) | Store action icons unresponsive |
| [P1-BG-7](#P1-BG-7) | No Clear Filters in Store Directory |
| [P1-BG-8](#P1-BG-8) | Export button not working |
| [P1-BG-9](#P1-BG-9) | Supervisor name invalid validation |
| [P1-BG-10](#P1-BG-10) | Backspace blocked in supervisor phone |
| [P1-BG-11](#P1-BG-11) | Duplicate promodizer names allowed |
| [P1-BG-12](#P1-BG-12) | Create button shows loading early |
| [P1-BG-13](#P1-BG-13) | Phone validation blocks valid input |
| [P1-BG-14](#P1-BG-14) | Assigned Stores popup not closable |
| [P1-BG-15](#P1-BG-15) | Dashboard arrow icons not working |
| [P1-BG-16](#P1-BG-16) | Import SKUs button showing wrong icon |
| [P1-BG-17](#P1-BG-17) | Fix Error & Re-upload not functional |
| [P1-BG-18](#P1-BG-18) | Status label capitalization inconsistent |
| [P1-BG-19](#P1-BG-19) | Radio button shows unwanted square outline |
| [P1-BG-20](#P1-BG-20) | Sorting icons missing in Promodizer table |
| [P1-BG-21](#P1-BG-21) | No confirmation message after SKU deletion |
| [P1-BG-22](#P1-BG-22) | Missing labels in Supervisor filters |
| [P1-BG-23](#P1-BG-23) | Supervisor Back link placed inconsistently |

  
[2.Promodizer Portal](#promodizer-portal)

* The Sales Analytics Dashboard provides analytical insights into SKUs, stores, staff performance, and transaction history.
Significant defects were observed in filters, date selection, validation checks, and duplicate datasets. Many filters do not clear or reset properly, negative numeric inputs are accepted, and several table headers or UI components are misaligned. Duplicated store names and broken data retrieval also affect overall analytics accuracy.
The dashboard needs strong improvements in filter logic, validation, data loading, and UI consistency to function as a reliable analytics tool.

| Bug-ID | Title |
|--------|--------|
| [P2-BG-1](#P2-BG-1) | Home icon position inconsistent |
| [P2-BG-2](#P2-BG-2) | Sales Detail shows “Record Not Found” |
| [P2-BG-3](#P2-BG-3) | Attendance calendar misaligned |
| [P2-BG-4](#P2-BG-4) | My Profile layout unbalanced |
| [P2-BG-5](#P2-BG-5) | Sidebar highlight not updating |
| [P2-BG-6](#P2-BG-6) | Feedback form not submitting |
| [P2-BG-7](#P2-BG-7) | Manual barcode input restricted to 7 digits |
| [P2-BG-8](#P2-BG-8) | Sales Detail icons misaligned |
| [P2-BG-9](#P2-BG-9) | Sales Detail error message section misaligned |
| [P2-BG-10](#P2-BG-10) | Promodizer Portal GTVL icon color inconsistent |
| [P2-BG-11](#P2-BG-11) | Dashboard icons not following consistent theme |

[3.Sales Analytics Dashboard](#sales-analytics-portal)

The Sales Analytics Dashboard provides analytical insights into SKUs, stores, staff performance, and transaction history.
Significant defects were observed in filters, date selection, validation checks, and duplicate datasets. Many filters do not clear or reset properly, negative numeric inputs are accepted, and several table headers or UI components are misaligned. Duplicated store names and broken data retrieval also affect overall analytics accuracy.
The dashboard needs strong improvements in filter logic, validation, data loading, and UI consistency to function as a reliable analytics tool.

| Bug-ID | Title |
|--------|--------|
| [P3-BG-1](#P3-BG-1) | SKU filters alignment issue |
| [P3-BG-2](#P3-BG-2) | Clear filter (X) not working |
| [P3-BG-3](#P3-BG-3) | Status checkbox not resetting |
| [P3-BG-4](#P3-BG-4) | Custom date range not opening |
| [P3-BG-5](#P3-BG-5) | Negative values allowed in quantity |
| [P3-BG-6](#P3-BG-6) | “None Selected” blocks all SKUs |
| [P3-BG-7](#P3-BG-7) | Wrong status label shown |
| [P3-BG-8](#P3-BG-8) | Store Performance columns hidden |
| [P3-BG-9](#P3-BG-9) | Negative sales volume accepted |
| [P3-BG-10](#P3-BG-10) | Tag clear (X) not resetting filters |
| [P3-BG-11](#P3-BG-11) | Staff details show “Not Found” |
| [P3-BG-12](#P3-BG-12) | Role filter not clearing |
| [P3-BG-13](#P3-BG-13) | Store & Staff filters not clearing |
| [P3-BG-14](#P3-BG-14) | Negative quantity filter allowed |
| [P3-BG-15](#P3-BG-15) | Clear All button styling incorrect |
| [P3-BG-16](#P3-BG-16) | Table headers inconsistent |
| [P3-BG-17](#P3-BG-17) | Duplicate stores in list |
| [P3-BG-18](#P3-BG-18) | Filters not visible in mobile view |
| [P3-BG-19](#P3-BG-19) | Sales dropdown misaligned in mobile view |
| [P3-BG-20](#P3-BG-20) | Assignment Stores filter inconsistent |
| [P3-BG-21](#P3-BG-21) | Date & Time preferences not applied |
| [P3-BG-22](#P3-BG-22) | Dashboard preferences not applied |

[4.Supervisor Portal](#supervisor-portal)

The Supervisor Portal allows supervisors to manage promodizers, record sales, track attendance, and view team details.
Testing identified issues such as non-updating attendance, unresponsive pagination, misplaced UI elements, and missing essential features (e.g., no Clock Out option). Popups lack close buttons, Clear Filters do not reset fields, and summary cards lack interactive UI elements.
The portal requires enhancements in functional completeness, responsive UI, data consistency, and user-friendly interactions.

| Bug-ID | Title |
|--------|--------|
| [P4-BG-1](#P4-BG-1) | Dashboard attendance not updating |
| [P4-BG-2](#P4-BG-2) | Sidebar order mismatch |
| [P4-BG-3](#P4-BG-3) | No Clock Out option |
| [P4-BG-4](#P4-BG-4) | Submission ID opens “Record Not Found” |
| [P4-BG-5](#P4-BG-5) | No Add/Edit/Delete for promodizers |
| [P4-BG-6](#P4-BG-6) | Phone allows alphabets |
| [P4-BG-7](#P4-BG-7) | No Clear Filters in My Team |
| [P4-BG-8](#P4-BG-8) | Duplicate Cancel buttons |
| [P4-BG-9](#P4-BG-9) | Store dropdown not responsive |
| [P4-BG-10](#P4-BG-10) | Summary section lacks visuals |
| [P4-BG-11](#P4-BG-11) | Add to Store button misplaced |
| [P4-BG-12](#P4-BG-12) | No close button on success popup |
| [P4-BG-13](#P4-BG-13) | Clear Filters does not reset dates |
| [P4-BG-14](#P4-BG-14) | Pagination arrows not functional |
| [P4-BG-15](#P4-BG-15) | No labels in My Team filters |
| [P4-BG-16](#P4-BG-16) | Sorting icons missing in Sales History |
| [P4-BG-17](#P4-BG-17) | Page title font inconsistency |
| [P4-BG-18](#P4-BG-18) | Clear Filters button styling inconsistent |

---
<h1 align="center">⭐ Day-1 ⭐</h1>

## Create A Pull Request

------
<h1 align="center">⭐ Day-2 ⭐</h1>

#**GTVL Management Portal — Bug Report**
---
<a id="management-portal"></a>

## **Module 1 — SKUs**
---
<a id="P1-BG-1"></a>

### **Bug-id : P1-BG-1**

**Description:**  
1. In the SKU list, all action icons (View, Edit, Delete) are unresponsive.  
2. Clicking any icon does not trigger any navigation or action.

**Expected Result:** All SKU action icons should open the correct View, Edit, or Delete actions.  
**Actual Result:** None of the action icons perform any operation when clicked.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-1](ScreenShot/p1-ss-1.png)

[↩️](#top)

---
<a id="P1-BG-2"></a>

### **Bug-id : P1-BG-2**

**Description:**  
1. The SKU list does not include a Clear Filters button.  
2. Once a filter is applied, there is no way to reset the list to default view.

**Expected Result:** A Clear Filters option should reset all applied filters to default view.  
**Actual Result:** No clear/reset option is available; user must manually remove each filter.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p1-ss-2](ScreenShot/p1-ss-2.png)

[↩️](#top)

---
<a id="P1-BG-3"></a>

### **Bug-id : P1-BG-3**

**Description:**  
1. System allows creation of a new SKU even when the SKU Code already exists.  
2. No validation or warning is shown for duplicate SKU codes.

**Expected Result:** System should prevent creation of duplicate SKU codes and show a validation message.  
**Actual Result:** Duplicate SKU codes are accepted without any warning.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-3](ScreenShot/p1-ss-3.png)

[↩️](#top)

---

## **Module 2 — Stores**
---
<a id="P1-BG-4"></a>

### **Bug-id : P1-BG-4**

**Description:**  
1. ZIP/Postal Code field accepts alphabetic characters.  
2. No validation prevents the user from entering non-numeric data.

**Expected Result:** ZIP field should accept only numeric values.  
**Actual Result:** Alphabet characters are accepted without validation.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-4](ScreenShot/p1-ss-4.png)

[↩️](#top)

---
<a id="P1-BG-5"></a>

### **Bug-id : P1-BG-5**

**Description:**  
1. When entering a phone number in the Create Store form, the field does not allow deleting characters.  
2. Backspace and delete keys do not work once input is typed.  
3. User cannot correct or modify the phone number after typing.

**Expected Result:** Phone number field should support normal editing (delete/backspace).  
**Actual Result:** User is unable to delete or modify entered values.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-5](ScreenShot/p1-ss-5.png)

[↩️](#top)

---
<a id="P1-BG-6"></a>

### **Bug-id : P1-BG-6**

**Description:**  
1. All action icons (View, Edit, Delete) in the Store Directory do not work.  
2. Clicking any icon does not trigger any response.

**Expected Result:** Store action icons should open View, Edit, or Delete functions.  
**Actual Result:** Icons do not respond when clicked; no action is triggered.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-6](ScreenShot/p1-ss-6.png)

[↩️](#top)

---
<a id="P1-BG-7"></a>

### **Bug-id : P1-BG-7**

**Description:**  
1. The Store Directory page has filters but no Clear Filters or Reset button.  
2. Once filters are applied, the user cannot reset the view easily.

**Expected Result:** Clear Filters should reset status, assignment, and search filters.  
**Actual Result:** No such option exists; filters must be manually removed.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p1-ss-7](ScreenShot/p1-ss-7.png)

[↩️](#top)

---
<a id="P1-BG-8"></a>

### **Bug-id : P1-BG-8**

**Description:**  
1. The Export button on the Store Directory page is unresponsive.  
2. Clicking the button does not trigger any file download or popup.

**Expected Result:** Export should download a CSV/Excel file of Store Directory.  
**Actual Result:** No download or response occurs when clicking Export.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-8](ScreenShot/p1-ss-8.png)

[↩️](#top)

---
<a id="P1-BG-9"></a>

## **Module 3 — Supervisors**
---

### **Bug-id : P1-BG-9**

**Description:**  
1. The system allows creating multiple supervisors with the same name.  
2. The Name field also accepts numeric characters (e.g., “John123”).  
3. No validation exists to restrict the name field to alphabetic characters only.  
4. This results in inconsistent and incorrect supervisor records.

**Expected Result:** Name field should validate duplicates and block numeric characters.  
**Actual Result:** Duplicate names and number-containing names are accepted.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-9](ScreenShot/p1-ss-9.png)

[↩️](#top)

---
<a id="P1-BG-10"></a>

### **Bug-id : P1-BG-10**

**Description:**  
1. While creating a new supervisor, the phone number input field stops accepting backspace/delete after entering partial input (e.g., “(555)”).  
2. User cannot edit or remove characters once typed.  
3. Only page refresh resets the field.

**Expected Result:** Phone field should allow editing and deleting normally.  
**Actual Result:** Backspace/Delete do not work; field becomes locked.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-10](ScreenShot/p1-ss-10.png)

[↩️](#top)

---

## **Module 4 — Promodizers**

---

<a id="P1-BG-11"></a>

### **Bug-id : P1-BG-11**

**Description:**  
1. The system allows creating promodizers with duplicate names.  
2. The Name field accepts numeric characters (e.g., “Mayur123”).  
3. No validation enforces alphabet-only names.  
4. This results in incorrect and inconsistent employee records.

**Expected Result:** Promodizer names should be alphabetic-only and unique.  
**Actual Result:** Duplicate and numeric names are accepted.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-11](ScreenShot/p1-ss-11.png)

[↩️](#top)

---
<a id="P1-BG-12"></a>

### **Bug-id : P1-BG-12**

**Description:**  
1. The “Create Promodizer” button shows a loading state (“Creating…”) even before clicking.  
2. Invalid data (numbers in names, incorrect formats) still triggers the loading state.

**Expected Result:** Button should load only after clicking and only with valid data.  
**Actual Result:** Button shows loading state prematurely.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-12](ScreenShot/p1-ss-12.png)

[↩️](#top)

---
<a id="P1-BG-13"></a>

### **Bug-id : P1-BG-13**

**Description:**  
1. When editing a promodizer, the phone number field remains in an error state even when entering a valid format (e.g., `+1-555-0301`).  
2. The system incorrectly flags the input as invalid.  
3. The Update Promodizer button stays disabled, preventing any updates.  
4. User cannot save changes due to incorrect phone validation.

**Expected Result:** Valid phone numbers should remove the error state and allow updating.  
**Actual Result:** Field stays in error; update button stays disabled.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-13](ScreenShot/p1-ss-13.png)

[↩️](#top)

---
<a id="P1-BG-14"></a>

### **Bug-id : P1-BG-14**

**Description:**  
When clicking the “Assigned Stores” count for any promodizer, a popup appears showing the list of assigned stores.  
1. The external-link icon in each store card does not redirect to the store details page.  
2. The close (X) button on the popup is non-functional and does not close the popup.  
3. User is forced to refresh the page to exit the popup.

**Expected Result:** Clicking link should open store details; X button should close popup.  
**Actual Result:** Neither redirect nor close works; popup remains stuck.

**Category:**  Functional / UI  

**Severity:**  High  

**Evidence:**  [p1-ss-14](ScreenShot/p1-ss-14.png)

[↩️](#top)

---

## **Module 5 — Dashboard**

---
<a id="P1-BG-15"></a>

### **Bug-id : P1-BG-15**

**Description:**  
1. On the Management Dashboard, each module card contains a right-arrow icon intended for quick navigation.  
2. Clicking these arrows does nothing.  
3. No page navigation or action is triggered.

**Expected Result:** Clicking arrow should navigate to the module’s page.  
**Actual Result:** Arrow icons are unresponsive.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-15](ScreenShot/p1-ss-15.png)

[↩️](#top)

---
<a id="P1-BG-16"></a>

### **Bug-id : P1-BG-16**

**Description:**  
1. The **Import SKUs** button is using the **wrong icon**.  
2. The icon displayed represents an **Upload** action instead of an **Import/Download** action.  
3. This causes a UI inconsistency and may confuse users about the actual purpose of the button.

**Expected Result:**  
Import button should use the correct **import/download icon** matching the rest of the UI theme.

**Actual Result:**  
Import SKUs button shows an incorrect upload-style icon.

**Category:** UI / Consistency  

**Severity:** Low  

**Evidence:**  [p1-ss-16](ScreenShot/p1-ss-16.png)

[↩️](#top)

---
<a id="P1-BG-17"></a>

### **Bug-id : P1-BG-17**

**Description:**  
1. When a duplicate SKU is detected during import, the system displays a **“Fix Error & Re-upload”** option.  
2. The radio button is clickable, but **no functionality is triggered** after selecting it.  
3. The system does **not provide any way to correct errors**, nor does it allow re-uploading corrected SKU data.  
4. The **Import SKUs** button remains disabled, blocking the entire process.

**Expected Result:**  
- Selecting **Fix Error & Re-upload** should enable a workflow allowing users to correct invalid rows and re-upload the corrected file.  
- Import button should become active after selecting this option.

**Actual Result:**  
- Radio button does nothing.  
- No correction flow appears.  
- User cannot re-upload or continue with the import.

**Category:** Functional  

**Severity:** High  

**Evidence:**  
[p1-ss-17](ScreenShot/p1-ss-17.png)

[↩️](#top)

---
<a id="P1-BG-18"></a>

### **Bug-id : P1-BG-18**

**Description:**  
1. On the SKUs page, the status label appears as **“active”** (lowercase).  
2. On other pages in the system, the status label is displayed as **“Active”** (uppercase).  
3. This inconsistency creates a lack of uniformity across modules.

**Expected Result:**  
Status labels should follow a **consistent capitalization format** across all pages and modules.

**Actual Result:**  
Status label appears in lowercase on the SKUs page but uppercase elsewhere.

**Category:** UI / Consistency  

**Severity:** Low  

**Evidence:**  
[p1-ss-18](ScreenShot/p1-ss-18.png)

[↩️](#top)

---
<a id="P1-BG-19"></a>

### **Bug-id : P1-BG-19**

**Description:**  
1. On the Create Promodizer page, selecting the **Active** or **Inactive** radio button displays an additional **square box** around the radio button.  
2. The selection animation/overflow is not smooth and appears visually broken.  
3. This results in an inconsistent and distracting UI behavior.

**Expected Result:**  
Radio buttons should display a clean, smooth selection state without extra shapes or overflow artifacts.

**Actual Result:**  
A square box appears around the selected radio button, causing UI inconsistency.

**Category:** UI / Visual Bug  

**Severity:** Low  

**Evidence:**  
[p1-ss-19](ScreenShot/p1-ss-19.png)

[↩️](#top)

---
<a id="P1-BG-20"></a>

### **Bug-id : P1-BG-20**

**Description:**  
1. In the Promodizer List page, sorting works for columns such as **Employee ID, Name, Phone, Email, and Status**, but  
2. The **sorting icons (↑↓)** are missing from the column headers.  
3. Users cannot visually identify which fields are sortable, causing UI inconsistency.

**Expected Result:**  
All sortable columns should display sorting icons consistently across the table.

**Actual Result:**  
Sorting icons are missing even though sorting functionality is active.

**Category:** UI / Functional  

**Severity:** Medium  

**Evidence:**  
[p1-ss-20](ScreenShot/p1-ss-20.png)

[↩️](#top)

---
<a id="P1-BG-21"></a>

### **Bug-id : P1-BG-21**

**Description:**  
When deleting a SKU record, the system does not display any success confirmation message.  
The user receives no indication that the deletion was completed successfully.

**Expected Result:**  
A success confirmation (toast, popup, or alert) should appear after deleting a SKU.

**Actual Result:**  
No confirmation message appears after deletion.

**Category:** Functional / UX  

**Severity:** Medium  

**Evidence:**  
[p1-ss-21](ScreenShot/p1-ss-21.png)

[↩️](#top)

---
<a id="P1-BG-22"></a>

### **Bug-id : P1-BG-22 — Missing Labels in Supervisor Filters**

**Description:**  
In the **GTVL Management Portal → Supervisors** module, the following labels are missing in the filter section:

- The **Search** textbox has no label above it.  
- The **Status** dropdown also does not display a label.  

Other modules (SKUs, Stores, Promodizers) show proper labels for filters, creating inconsistency.

**Expected Result:**  
All filters should display clear and consistent labels across all modules (e.g., “Search”, “Status”).

**Actual Result:**  
Labels for the Search textbox and Status dropdown are missing in the Supervisor tab.

**Category:** UI / Consistency  

**Severity:** Medium  

**Evidence:**  
[p1-ss-22](ScreenShot/p1-ss-22.png)

[↩️](#top)

---
<a id="P1-BG-23"></a>

### **Bug-id : P1-BG-23 — Supervisor Back Link Poor UI Placement**

**Description:**  
In the Supervisor Detail window, the **“Back to Supervisors List”** navigation is placed only as a text link at the **bottom** of the page.  
However, in other modules such as **SKUs**, the Back option appears as a **button positioned at the top**, following standard UI/UX patterns.  
This inconsistency disrupts navigation flow and reduces visibility of the back action.

**Expected Result:**  
The Back navigation should follow a consistent UI pattern — preferably a button placed at the top of the detail page like other modules.

**Actual Result:**  
Back navigation appears only as a bottom text link, making it less visible and inconsistent with other module layouts.

**Category:** UI / Consistency  

**Severity:** Medium  

**Evidence:**  
[p1-ss-23](ScreenShot/p1-ss-23.png)

[↩️](#top)

---
<h1 align="center">⭐ Day-3 ⭐</h1>

---
<a id="promodizer-portal"></a>

# **GTVL Promodizer Portal — Bug Report**

---
## **Module 1 — Dashboard**

---
<a id="P2-BG-1"></a>
 
### **Bug-id : P2-BG-1**

**Description:**  
1. The Home button icon (top-right corner) is not fixed in a consistent position.  
2. Its placement shifts across different modules such as Record Sales, Sales History, and Attendance.  
3. This creates UI inconsistency and may confuse users.

**Expected Result:** Home icon should stay in a fixed, consistent position across all modules.  
**Actual Result:** Home icon shifts position on different screens, causing inconsistency.

**Category:** UI  

**Severity:** Medium  

**Evidence:**  [p2-ss-1](ScreenShot/p2-ss-1.jpg)

[↩️](#top)

---

## **Module 2 — Sales History**

---
<a id="P2-BG-2"></a>
 
### **Bug-id : P2-BG-2**

**Description:**  
1. After recording a sale successfully, the entry appears correctly in Sales History.  
2. When clicking any sales entry, the Sales Detail page opens but shows “Sales record not found”.  
3. The system fails to load the sale description even though the sale history card displays the sale information.

**Expected Result:** Clicking a sale entry should open its detailed Sales Record page with full information.  
**Actual Result:** Detail page shows “Sales record not found” even for valid records.

**Category:** Functional  

**Severity:** High  

**Evidence:**  [p2-ss-2](ScreenShot/p2-ss-2.png)

[↩️](#top)

---
## **Module 3 — Attendance History**

---
<a id="P2-BG-3"></a>
 
### **Bug-id : P2-BG-3**

**Description:**  
1. In the Attendance History Calendar View, all dates for the entire month are listed under the Sunday column.  
2. Other weekday columns (Mon–Sat) remain empty.  
3. The calendar grid fails to position dates according to correct weekdays.  
4. This makes the calendar view unusable and misleading.

**Expected Result:** Calendar should place each date under its correct weekday column.  
**Actual Result:** All dates appear under Sunday, with other columns empty.

**Category:** UI / Functional  

**Severity:** Medium  

**Evidence:**  [p2-ss-3](ScreenShot/p2-ss-3.png)

[↩️](#top)

---

## **Module 4 — My Profile**

---
<a id="P2-BG-4"></a>
 
### **Bug-id : P2-BG-4**

**Description:**  
1. The My Profile page displays user information only on the left portion of the page.  
2. A large empty space appears on the right side, making the layout look incomplete.  
3. Page content does not stretch to utilize available width.  
4. Overall UI looks unbalanced and visually unappealing.

**Expected Result:** My Profile layout should be balanced and use available page width effectively.  
**Actual Result:** Page content is left-aligned with empty space and unbalanced layout.

**Category:** UI  

**Severity:** Low  

**Evidence:**  [p2-ss-4](ScreenShot/p2-ss-4.png)

[↩️](#top)

---
<a id="P2-BG-5"></a>
 
### **Bug-id : P2-BG-5**

**Description:**  
The sidebar navigation in the Promodizer Portal does not correctly update the active state when moving between modules.  
This issue appears in two ways:

1. **Green Active Indicator Does Not Move**  
   - The small green light/backlight stays fixed on Dashboard.  
   - It does not follow the currently selected menu option.

2. **Sidebar Highlight Works Only for Some Items**  
   - Highlight appears correctly for Dashboard, Record Sales, My Stores, My Profile.  
   - Highlight does NOT appear for Sales History, Attendance, Attendance History.  

This makes the sidebar visually inconsistent and confusing.

**Expected Result:** Active state indicators should move correctly and highlight should appear for all menu items.  
**Actual Result:** Active indicator remains fixed; highlight shows only for some modules.

**Category:** UI / Functional  

**Severity:** Medium  

**Evidence:**  [p2-ss-5](ScreenShot/p2-ss-5.png)

[↩️](#top)

---
<a id="P2-BG-6"></a>
 
### **Bug-id : P2-BG-6**

**Description:**  
1. The feedback form does not successfully save or submit any feedback.  
2. Submission always fails, and no feedback is stored.

**Expected Result:** Feedback form should save and submit responses successfully.  
**Actual Result:** Feedback submission fails and nothing is stored.

**Category:** Functional  

**Severity:** High  

**Evidence:**  [p2-ss-6](ScreenShot/p2-ss-6.png)

[↩️](#top)

---
<a id="P2-BG-7"></a>

### **Bug-id : P2-BG-7**

**Description:**  
In the Promodizer Portal → Record Sales page, the manual barcode input field accepts **only up to 7 digits**.  
If the user tries to enter more digits, the field stops accepting input and immediately displays **“Barcode not recognized”**.  
Each attempt generates repeated pop-ups, even when the barcode entered is valid.

**Expected Result:**  
Manual barcode field should accept the full barcode length (typically 12–13 digits) and validate it correctly.

**Actual Result:**  
Input is restricted to 7 digits, and multiple “barcode not recognized” pop-ups appear unnecessarily.

**Category:** Functional / Validation  

**Severity:** High  

**Evidence:**  
[p2-ss-7](ScreenShot/p2-ss-7.png)

[↩️](#top)

---
<a id="P2-BG-8"></a>

### **Bug-id : P2-BG-8**

**Description:**  
On the Sales Detail page, both the **Back** icon and the **Home** icon are not positioned correctly within the title bar.  
They appear **misaligned** and placed **outside the main header div**, breaking the visual structure of the page.

**Expected Result:**  
Icons should be aligned properly inside the header/title bar with consistent spacing and correct placement.

**Actual Result:**  
Back and Home icons appear outside the header area, causing UI misalignment.

**Category:** UI / Layout  

**Severity:** Medium  

**Evidence:**  
[p2-ss-8](ScreenShot/p2-ss-8.png)

[↩️](#top)

---
<a id="P2-BG-9"></a>

### **Bug-id : P2-BG-9**

**Description:**  
The Sales Detail error section is visually misaligned.  
The alert icon, message (“Sales record not found or may have been deleted”), and the **Back to Sales History** link are not aligned properly within the container, resulting in an uneven and unbalanced layout.

**Expected Result:**  
The error icon, message text, and back link should be properly aligned within the same visual structure for a clean, balanced UI.

**Actual Result:**  
Elements appear misaligned and uneven, making the error box look unstructured.

**Category:** UI / Layout  

**Severity:** Low  

**Evidence:**  
[p2-ss-9](ScreenShot/p2-ss-9.png)

[↩️](#top)

---
<a id="P2-BG-10"></a>

### **Bug-id : P2-BG-10**

**Description:**  
The GTVL icon displayed in the *Promodizer Portal* uses a different color compared to the icons shown in the Management, Supervisor, and Sales Analytics portals.  
This color inconsistency breaks the uniform branding and creates a visually disconnected experience.

**Expected Result:**  
GTVL icon should follow a consistent color scheme across all portals.

**Actual Result:**  
Promodizer Portal displays the icon in a different color while other portals use a uniform color.

**Category:** UI / Branding  

**Severity:** Low  

**Evidence:**  
[p2-ss-10](ScreenShot/p2-ss-10.png)

[↩️](#top)

---
<a id="P2-BG-11"></a>

### **Bug-id : P2-BG-**

**Description:**  
Dashboard action icons in the Promodizer Portal use inconsistent color themes.  
The *Record Sales* icon appears in green, while other icons use different colors and styles.  
On hover, some icons turn grey, breaking the visual theme and creating inconsistency across the dashboard UI.

**Expected Result:**  
All dashboard icons should follow a unified color theme and consistent hover behavior.

**Actual Result:**  
Icons appear in different colors, and hover states differ across tiles, resulting in mismatched UI elements.

**Category:** UI / Design Consistency  

**Severity:** Low  

**Evidence:**  
[p2-ss-11](ScreenShot/p2-ss-11.png)

[↩️](#top)


---

<a id="sales-analytics-portal"></a>

# **GTVL Sales Analytics Dashboard — Bug Report**

---

## **Module 1 — SKU Performance**

---
<a id="P3-BG-1"></a>
 
### **Bug-id : P3-BG-1**

**Description:**  
The **SKU Performance Analysis** screen contains multiple UI alignment issues:  
1. The **Filters panel** is not aligned properly with the SKU table header section.  
2. The **Total Quantity Sold (Min–Max)** input fields are uneven and visually misaligned.  
These inconsistencies affect UI clarity and overall user experience.

**Expected Result:** Filters and input fields should be aligned consistently with the table layout.  
**Actual Result:** Filters and Min–Max fields appear misaligned and visually inconsistent.

**Category:**  UI  

**Severity:**  Low  

**Evidence:**  [p3-ss-1](ScreenShot/p3-ss-1.png)

[↩️](#top)

---
<a id="P3-BG-2"></a>
 
### **Bug-id : P3-BG-2**

**Description:**  
1. When a search input is applied in the SKU Performance module, a filter tag appears with a clear (X) button.  
2. Clicking the **X** does not remove the applied search filter.  
3. The search field also does not reset, and the results remain unchanged.

**Expected Result:** Clicking the X should remove the search filter and reset the results.  
**Actual Result:** X button does nothing; filter stays applied and results do not reset.

**Category:**  Functional  

**Severity:**  Low  

**Evidence:**  [p3-ss-2](ScreenShot/p3-ss-2.png)

[↩️](#top)

---
<a id="P3-BG-3"></a>
 
### **Bug-id : P3-BG-3**

**Description:**  
1. The **Clear All** button in the Filters panel does not reset the **Status** checkboxes.  
2. Even after clicking **Clear All**, the **Active** checkbox remains selected.  
3. Other filters may reset, but the status filter does not clear.

**Expected Result:** Clear All should uncheck all status checkboxes.  
**Actual Result:** Active checkbox remains checked even after Clear All.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-3](ScreenShot/p3-ss-3.png)

[↩️](#top)

---
<a id="P3-BG-4"></a>
 
### **Bug-id : P3-BG-4**

**Description:**  
1. When selecting **Custom Range** from the Date Range dropdown, no date picker or calendar modal opens.  
2. User cannot select a start date or end date.  
3. The Custom Range option becomes unusable and does not filter SKU data.

**Expected Result:** A date picker should open allowing selection of From and To dates.  
**Actual Result:** No date picker opens, preventing custom date selection.

**Category:**  Functional / UI 

**Severity:**  Medium  

**Evidence:**  [p3-ss-4](ScreenShot/p3-ss-4.png)

[↩️](#top)

---
<a id="P3-BG-5"></a>
 
### **Bug-id : P3-BG-5**

**Description:**  
1. The **Total Quantity Sold** filter allows users to enter negative numbers (e.g., -55 to -60).  
2. Negative quantities make no logical sense in sales analytics.  
3. System applies the filter and displays results with negative range.

**Expected Result:** Total Quantity Sold fields should not accept negative values.  
**Actual Result:** System accepts and applies filters with negative input.

**Category:**  Functional / Validation 

**Severity:**  Medium  

**Evidence:**  [p3-ss-5](ScreenShot/p3-ss-5.png)

[↩️](#top)

---
<a id="P3-BG-6"></a>
 
### **Bug-id : P3-BG-6**

**Description:**  
1. When both **Active** and **Inactive** checkboxes are unchecked in the Status filter, the system shows a tag **“Status: None Selected”**.  
2. System treats this as a filter condition instead of removing all filtering.  
3. As a result, SKU table displays **“No SKUs Found”**, even though SKUs exist.

**Expected Result:** If no status is selected, system should display all SKUs by default.  
**Actual Result:** System applies “None Selected” as a filter and hides all SKUs.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-6](ScreenShot/p3-ss-6.png)

[↩️](#top)

---
<a id="P3-BG-7"></a>
 
### **Bug-id : P3-BG-7**

**Description:**  
1. When both Status options (Active + Inactive) are selected, the filter tag incorrectly shows: **“Status: Inactive Only”**.  
2. This misrepresents the actual filter condition and causes confusion.

**Expected Result:** Filter tag should show “Active & Inactive” or “All”.  
**Actual Result:** Tag displays “Inactive Only” even when both options are selected.

**Category:**  Functional / UI  

**Severity:**  Medium  

**Evidence:**  [p3-ss-7](ScreenShot/p3-ss-7.png)

[↩️](#top)

---
## **Module 2 — Store Performance**

---
<a id="P3-BG-8"></a>
 
### **Bug-id : P3-BG-8**

**Description:**  
1. In the **Store Performance** module, some table columns are **not visible in desktop view** due to horizontal overflow.  
2. Right-side columns like **SKUs Sold**, **Active Staff**, **Last Sale Date** become hidden.  
3. All columns are visible only in mobile view (verified).

**Expected Result:** All columns should be visible normally in desktop view.  
**Actual Result:** Several right-side columns are clipped or hidden in desktop layout.

**Category:**  UI / Layout  

**Severity:**  Medium  

**Evidence:**  [p3-ss-8](ScreenShot/p3-ss-8.png)

[↩️](#top)

---
<a id="P3-BG-9"></a>
 
### **Bug-id : P3-BG-9**

**Description:**  
1. The **Sales Volume** filter accepts negative values in Min and Max fields.  
2. Negative sales volume is logically invalid.  
3. System still applies the filter and shows values like **Sales: -55 – 55**.

**Expected Result:** Sales Volume filter should allow only non-negative values.  
**Actual Result:** Negative values are accepted and applied without validation.

**Category:**  Functional / Validation  

**Severity:**  Medium  

**Evidence:**  [p3-ss-9](ScreenShot/p3-ss-9.png)

[↩️](#top)

---

## **Module 3 — Staff Performance**

---
<a id="P3-BG-10"></a>
 
### **Bug-id : P3-BG-10**

**Description:**  
1. Filter tags in Staff Performance show an **X** button to clear each filter.  
2. Clicking the **X** does nothing.  
3. Filters remain applied and table does not refresh.

**Expected Result:** Clicking X should remove that filter and refresh data.  
**Actual Result:** X button does nothing and filter remains active.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-10](ScreenShot/p3-ss-10.png)

[↩️](#top)

---
<a id="P3-BG-11"></a>
 
### **Bug-id : P3-BG-11**

**Description:**  
1. Clicking any employee row should open employee details.  
2. Instead, page shows **“Staff Not Found”** with empty fields.  
3. No employee data loads even when valid employees are selected.

**Expected Result:** Employee Detail page should load with real employee data.  
**Actual Result:** Page shows “Staff Not Found” and loads no data.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p3-ss-11](ScreenShot/p3-ss-11.png)

[↩️](#top)

---
<a id="P3-BG-12"></a>
 
### **Bug-id : P3-BG-12**

**Description:**  
1. In Staff Performance, both Role checkboxes (Promodizer & Supervisor) are auto-checked.  
2. Clicking **Clear All Filters** does **not** uncheck these boxes.  
3. Role filter remains active and cannot be fully reset.

**Expected Result:** Clear All should reset all filters including role checkboxes.  
**Actual Result:** Promodizer & Supervisor remain selected after Clear All.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-12](ScreenShot/p3-ss-12.png)

[↩️](#top)

---

## **Module 4 — Transaction History**

---
<a id="P3-BG-13"></a>
 
### **Bug-id : P3-BG-13**

**Description:**  
1. In Transaction History, **Store** and **Staff** checkbox filters do NOT reset after clicking **Clear All**.  
2. All values remain checked.  
3. Filter state cannot be reset without manually unchecking every entry.

**Expected Result:** Clear All should uncheck Store & Staff checkboxes.  
**Actual Result:** All checkboxes remain checked after Clear All.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-13](ScreenShot/p3-ss-13.png)

[↩️](#top)

---
<a id="P3-BG-14"></a>
 

### **Bug-id : P3-BG-14**

**Description:**  
1. The Total Quantity Range filter in Transaction History allows negative numbers (e.g., -555, -66).  
2. System accepts and applies these invalid values when filtering.

**Expected Result:** Total Quantity Range should not accept negative values.  
**Actual Result:** System accepts negative values and applies the filter.

**Category:**  Functional / Validation  

**Severity:**  Medium  

**Evidence:**  [p3-ss-14](ScreenShot/p3-ss-14.png)

[↩️](#top)

---
<a id="P3-BG-15"></a>
 
### **Bug-id : P3-BG-15**

**Description:**  
1. The **Clear All** text appears without any button styling or visible button structure.  
2. Its position is incorrect — it is placed at the top instead of below the **Apply Filters** button.

**Expected Result:** Clear All should be a styled button placed below Apply Filters.  
**Actual Result:** Clear All appears as plain text at the top.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p3-ss-15](ScreenShot/p3-ss-15.png)

[↩️](#top)

---
<a id="P3-BG-16"></a>
 
### **Bug-id : P3-BG-16**

**Description:**  
1. The table headers **Role** and **Submission ID** have a different text style compared to other table headers.  
2. The **sorting arrows (up/down)** seen on other columns are missing for these two headers.  
3. This causes UI inconsistency within the Transaction History table.

**Expected Result:** Role & Submission ID headers should match other headers and show sorting arrows.  
**Actual Result:** Headers are styled differently and sorting arrows are missing.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p3-ss-16](ScreenShot/p3-ss-16.png)

[↩️](#top)

---
<a id="P3-BG-17"></a>

### **Bug-id : P3-BG-17**

**Description:**  
1. The **Stores** multi-select filter in Transaction History displays **multiple duplicate entries** for several stores.  
2. Stores like **Beverly Hills Grocery**, **Downtown Market NYC**, and **Lincoln Park Superstore** appear repeatedly in the dropdown list.  
3. The list becomes unnecessarily long and confusing due to repeated values.

**Expected Result:**  
Store filter should display a **unique list of store names**, with no repeated entries.

**Actual Result:**  
Same store appears multiple times in the dropdown:
- Beverly Hills Grocery (3 times)  
- Downtown Market NYC (7+ times)  
- Lincoln Park Superstore (3 times)  
- Others also repeated  

**Category:** Functional / Data Issue  

**Severity:** Medium  

**Evidence:**  
[p3-ss-17](ScreenShot/p3-ss-17.png)

[↩️](#top)

---
<a id="P3-BG-18"></a>

### **Bug-id : P3-BG-18**

**Description:**  
The filters panel in the **SKU Performance** module is not visible in mobile view.  
Users cannot access Category, Status, Total Quantity Sold, or Date Range filters when viewing the page on mobile screens.  
Only the table appears, making the filter section inaccessible.

**Expected Result:**  
Filters should be fully visible and accessible in mobile view with responsive layout adjustments or collapsible panels.

**Actual Result:**  
Filters disappear entirely in mobile view, leaving no option for filtering SKU data.

**Category:** UI / Responsive Design  

**Severity:** Medium  

**Evidence:**  
[p3-ss-18](ScreenShot/p3-ss-18.png)

[↩️](#top)

---
<a id="P3-BG-19"></a>

### **Bug-id : P3-BG-19**

**Description:**  
In the Store Performance module, the **Sales dropdown is not aligned properly in mobile view**.  
The dropdown expands **outside the visible container**, causing layout overflow.  
UI placement breaks, making the filter difficult to read and interact with.

**Expected Result:**  
Dropdown should stay within its container and maintain proper alignment in all screen sizes.

**Actual Result:**  
Dropdown overflows the div and appears outside the layout in mobile view.

**Category:** UI / Responsive Design  

**Severity:** Medium  

**Evidence:**  
[p3-ss-19](ScreenShot/p3-ss-19.png)

[↩️](#top)

---
<a id="P3-BG-20"></a>

### **Bug-id : P3-BG-20**

**Description:**  
In the Staff Performance module, the **Assignment Stores** section shows UI inconsistencies:

1. The store list does **not contain checkboxes**, unlike all other filter sections in the Analytics Dashboard.  
2. The **search bar above the table has no label**, making it unclear what the input field is meant for.  
3. This breaks the theme consistency, as every other filter section uses labeled fields and checkbox-based selection.

**Expected Result:**  
- Assignment Stores should use the same checkbox UI theme as other filter sections.  
- The search bar should include a clear label above it (e.g., "Search Stores").  

**Actual Result:**  
- Checkboxes are missing.  
- Search bar appears unlabeled, reducing usability and visual consistency.

**Category:** UI / Consistency  

**Severity:** Medium  

**Evidence:**  
[p3-ss-20](ScreenShot/p3-ss-20.png)

[↩️](#top)

---
<a id="P3-BG-21"></a>

### **Bug-id : P3-BG-21 — Date & Time Preference Changes Not Applied**

**Description:**  
In the *Settings → Date Range Defaults* section of the Sales Analytics Dashboard, changes made to the default date range, date format, or time format are not reflected in the actual dashboard views.  
Even after selecting new options and saving preferences, the previous default settings continue to display.

**Expected Result:**  
Updated date range, date display format, and time display format should immediately apply across all modules where date/time is displayed.

**Actual Result:**  
The dashboard continues to show old date range and time formats, ignoring the saved preference changes.

**Category:** Functional  

**Severity:** Medium  

**Evidence:**  
[p3-ss-21](ScreenShot/p3-ss-21.png)

[↩️](#top)

---
<a id="P3-BG-22"></a>

### **Bug-id : P3-BG-22 — Dashboard Preferences Not Applied**

**Description:**  
In the *Settings → Dashboard Preferences* section, updating options such as **Default Landing Page**, **Default Chart Type**, and KPI visibility saves successfully and displays a “Changes saved successfully” message.  
However, these updated preferences do **not** reflect on the actual dashboard view.  
The dashboard continues to show the old landing page and chart type.

**Expected Result:**  
After saving preferences, the dashboard should automatically reflect the new default landing page and selected chart type, along with updated KPI card visibility.

**Actual Result:**  
Dashboard loads with previous settings. None of the saved changes are applied.

**Category:** Functional  

**Severity:** Medium  

**Evidence:**  
[p3-ss-22](ScreenShot/p3-ss-22.png)

[↩️](#top)

---
<h1 align="center">⭐ Day-4 ⭐</h1>
<a id="supervisor-portal"></a>

# **gtvl-supervisor-portal — Bug Report**

---
<a id="P4-BG-1"></a>
 
### **Bug-id : P4-BG-1**

**Description:**  
1. Even after marking attendance as **Present** in Attendance Management,  
2. The Dashboard still shows **Not Marked** for Today’s Attendance.  
3. System does not update dashboard status after marking attendance.

**Expected Result:** Dashboard should display **Present** once attendance is marked.  
**Actual Result:** Dashboard continues showing **Not Marked** even after attendance is recorded.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p4-ss-1](ScreenShot/p4-ss-1.png)

[↩️](#top)

---
<a id="P4-BG-2"></a>
 
### **Bug-id : P4-BG-2**

**Description:**  
1. The order of menu items in the **left sidebar** does not match the order of items shown in the **Quick Actions** section.  
2. Sidebar: Dashboard → Record Sales → Sales History → Attendance → My Team → Add Promodizer → My Profile  
3. Quick Actions: Record Sales → Mark Attendance → View Team → Sales History  
4. The mismatch creates UI inconsistency and confusion about navigation hierarchy.

**Expected Result:**  
Sidebar order and Quick Actions order should follow a consistent logical sequence.

**Actual Result:**  
Sidebar and Quick Actions display items in different, unaligned orders.

**Category:**  UI  

**Severity:**  Low  

**Evidence:**  [p4-ss-2](ScreenShot/p4-ss-2.png)

[↩️](#top)

---
<a id="P4-BG-3"></a>
 
### **Bug-id : P4-BG-3**

**Description:**  
1. In the Attendance module, users can only **Mark Attendance (Clock In)** but there is **no option to Clock Out**.  
2. As a result, the **Clock Out Time** field always displays a dash (-).  
3. This prevents recording full attendance data for the day.

**Expected Result:** User should be able to Clock Out, and the Clock Out Time should be recorded properly.

**Actual Result:** No Clock Out feature exists, and Clock Out Time remains blank.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p4-ss-3](ScreenShot/p4-ss-3.png)

[↩️](#top)

---
<a id="P4-BG-4"></a>
 
### **Bug-id : P4-BG-4**

**Description:**  
1. Clicking any Submission ID in Sales History should open the detailed sales record.  
2. Instead, clicking redirects to a "Record Not Found" page.  
3. The system does not pass the submission ID in the URL, causing the detail page to fail.

**Expected Result:** Sales Record Detail page should open and show full submission details.  
**Actual Result:** Page shows “Record Not Found — No submission ID provided in the URL.”

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p4-ss-4](ScreenShot/p4-ss-4.png)

[↩️](#top)

---
<a id="P4-BG-5"></a>
 
### **Bug-id : P4-BG-5**

**Description:**  
1. After adding a promodizer, the Supervisor cannot perform any management actions.  
2. No options/buttons are available to **Add**, **Edit**, or **Delete** a promodizer.  
3. The My Team page only displays promodizer cards without any action controls.

**Expected Result:** Supervisor should see options to Add, Edit, or Delete promodizers on the My Team page.  
**Actual Result:** No management options are visible; supervisor cannot modify promodizers.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p4-ss-5](ScreenShot/p4-ss-5.png)

[↩️](#top)

---
<a id="P4-BG-6"></a>
 
### **Bug-id : P4-BG-6**

**Description:**  
1. The Phone Number field on the Add Promodizer page accepts alphabetic characters.  
2. User can enter letters (e.g., "Mayur") instead of digits.  
3. No validation is applied to restrict input to numeric phone number format.

**Expected Result:** Phone Number field should accept only numeric values and follow a valid phone format.  
**Actual Result:** Field allows alphabetic characters without validation.

**Category:**  Functional / Validation  

**Severity:**  High  

**Evidence:**  [p4-ss-6](ScreenShot/p4-ss-6.png)

[↩️](#top)

---
<a id="P4-BG-7"></a>
 
### **Bug-id : P4-BG-7**

**Description:**  
1. In the My Team module, store and status filters can be applied but cannot be cleared.  
2. There is **no Clear Filters button** to reset selections.  
3. User must manually change dropdowns each time, causing poor usability.

**Expected Result:** A Clear Filters option should reset store and status filters to default.  
**Actual Result:** No Clear Filters option is available; filters stay applied until manually changed.

**Category:**  Functional / UI  

**Severity:**  Medium  

**Evidence:**  [p4-ss-7](ScreenShot/p4-ss-7.png)

[↩️](#top)

---
<a id="P4-BG-8"></a>
 
### **Bug-id : P4-BG-8**

**Description:**  
1. The **Add New Promodizer** page displays **two Cancel buttons** —  
   one at the top-right corner and another inside the form.  
2. Having duplicate Cancel buttons is unnecessary and creates UI redundancy.  
3. This may confuse users about which Cancel action to use.

**Expected Result:** Only one clearly placed Cancel button should be displayed.  
**Actual Result:** Two Cancel buttons appear on the same page.

**Category:** UI  

**Severity:** Low  

**Evidence:**  [p4-ss-8](ScreenShot/p4-ss-8.png)

[↩️](#top)

---
<a id="P4-BG-9"></a>
 
### **Bug-id : P4-BG-9**

**Description:**  
1. The **Store dropdown** in the Sales History module is **not responsive** on iPad or tablet-sized screens.  
2. The dropdown expands outside the visible screen area and does not adjust to the layout width.  
3. This causes selection difficulty and breaks responsive UI behavior on medium-sized devices.

**Expected Result:** Dropdown should resize and reposition properly on iPad/tablet view.  
**Actual Result:** Dropdown overflows the screen and becomes unusable on tablet resolutions.

**Category:** UI / Responsive Design  

**Severity:** Medium  

**Evidence:**  [p4-ss-9](ScreenShot/p4-ss-9.png)

[↩️](#top)

---
<a id="P4-BG-10"></a>
 
### **Bug-id : P4-BG-10**

**Description:**  
1. The **My Team summary section** (Total Promodizers, Active Promodizers, Stores) appears visually plain and inconsistent compared to other modules.  
2. Cards do **not have hover backlight or hover effects**, making them less interactive.  
3. No **icons** are displayed inside the cards, unlike similar summary cards in other portals/modules.  
4. The cards lack a proper **color theme or visual hierarchy**, causing them to look incomplete and less engaging.

**Expected Result:** Summary cards should include icons, hover effects, and consistent color styling similar to other modules.  
**Actual Result:** Cards appear plain, without icons, hover effects, or a consistent color scheme.

**Category:** UI / Visual Design  

**Severity:** Low  

**Evidence:**  [p4-ss-10](ScreenShot/p4-ss-10.png)

[↩️](#top)

---
<a id="P4-BG-11"></a>
 
### **Bug-id : P4-BG-11**

**Description:**  
The **Add to Store** button in the My Team module is placed incorrectly on the far right side, making it appear disconnected from the section.  
Its position creates UI inconsistency and may confuse users about its purpose.

**Expected Result:**  
The Add to Store button should be placed near the store header or within a consistent actionable area for better UI clarity.

**Actual Result:**  
Button appears improperly placed on the right side, visually detached from relevant elements.

**Category:** UI  

**Severity:** Medium  

**Evidence:**  [p4-ss-11](ScreenShot/p4-ss-11.png)

[↩️](#top)

---
<a id="P4-BG-12"></a>
 
### **Bug-id : P4-BG-12**

**Description:**  
1. The “Sales Recorded Successfully” popup does **not show any close (X) button** on the top-right corner.  
2. User is unable to dismiss the popup without clicking one of the action buttons.

**Expected Result:** Popup should include a clear **close (X)** icon to manually exit the popup.  
**Actual Result:** No close option is provided; popup stays until an action button is pressed.

**Category:** UI / Functional  

**Severity:** Medium  

**Evidence:** [p4-ss-12](ScreenShot/p4-ss-12.png)

[↩️](#top)

---
<a id="P4-BG-13"></a>
 
### **Bug-id : P4-BG-13**

**Description:**  
1. The **Clear Filters** button in the Sales History module is not styled consistently with other buttons.  
2. Its design looks plain, unaligned, and visually weaker compared to adjacent buttons like **Apply Filters** and **Export CSV**.  
3. **Clicking the Clear Filters button does NOT reset the From Date and To Date fields.**  
4. Both date boxes remain unchanged even after clicking Clear Filters, requiring manual clearing.

**Expected Result:**  
- Clear Filters button should have consistent styling — proper padding, border, hover effect, and alignment matching other action buttons.  
- Clicking Clear Filters should **reset all filters**, including *From Date* and *To Date* fields.

**Actual Result:**  
- Button appears minimally styled, lacks proper formatting, and visually breaks UI consistency.  
- **Date fields do not reset** after clicking Clear Filters.

**Category:** UI / Functional / Design  

**Severity:** Medium  

**Evidence:**  
[p4-ss-13](ScreenShot/p4-ss-13.png)

[↩️](#top)


---
<a id="P4-BG-14"></a>
 
### **Bug-id : P4-BG-14**

**Description:**  
1. The pagination arrows (**<** and **>**) at the bottom of the Sales History table are not functional.  
2. Clicking them does not change the page or load additional records.

**Expected Result:**  
Pagination arrows should navigate between pages (Next/Previous) and load the correct records.

**Actual Result:**  
Pagination controls do nothing when clicked; user remains on the same page.

**Category:** Functional  

**Severity:** Medium  

**Evidence:**  [p4-ss-14](ScreenShot/p4-ss-14.png)

[↩️](#top)

---
<a id="P4-BG-15"></a>

### **Bug-id : P4-BG-15**

**Description:**  
On the *Supervisor Portal → My Team* page, the filter section contains:  
- Search textbox  
- Store dropdown  
- Status dropdown  

However, **none of these fields display labels**, unlike other modules where each filter input is clearly labeled.  
This leads to inconsistency and reduces clarity for users.

**Expected Result:**  
All filter inputs (Search, Store, Status) should include visible labels to maintain UI consistency and improve usability.

**Actual Result:**  
Filter inputs appear without labels, making the UI inconsistent with other sections.

**Category:** UI / Consistency  

**Severity:** Medium  

**Evidence:**  
[p4-ss-15](ScreenShot/p4-ss-15.png)

[↩️](#top)

---
<a id="P4-BG-16"></a>

### **Bug-id : P4-BG-16**

**Description:**  
On the *Supervisor Portal → Sales History* page, the table headers (Submission ID, Date & Time, Store, Items, Status) do **not display sorting icons**, unlike other modules.  
Users cannot sort the Sales History records by any column.

**Expected Result:**  
Sorting icons should appear beside each table column header, allowing users to sort data (ascending/descending).

**Actual Result:**  
No sorting icons are present, and the table cannot be sorted.

**Category:** Functional / UI  

**Severity:** Medium  

**Evidence:**  
[p4-ss-16](ScreenShot/p4-ss-16.png)

[↩️](#top)

---
<a id="P4-BG-17"></a>

### **Bug-id : P4-BG-17**

**Description:**  
The page titles in the *GTVL Management Portal* and *GTVL Supervisor Portal* use different typography styles.  
Font weight, size, and spacing differ between portals, causing inconsistent UI hierarchy and branding.

**Expected Result:**  
All portal page titles should follow a standardized font weight, size, and spacing to maintain consistent visual design.

**Actual Result:**  
Management Portal and Supervisor Portal display titles with different typography styles, breaking UI uniformity.

**Category:** UI / Design Consistency  

**Severity:** Low  

**Evidence:**  
[p4-ss-17](ScreenShot/p4-ss-17.png)

[↩️](#top)

---
<a id="P4-BG-18"></a>

### **Bug-id : P4-BG-18**

**Description:**  
The **Clear Filters** button on the Supervisor Portal’s *Sales History* page does not follow the standard button styling used across the application.  
Its color, padding, and background styling differ from other action buttons, resulting in inconsistent UI/UX.

**Expected Result:**  
Clear Filters button should match the global button styling — consistent background, border radius, padding, and hover effects.

**Actual Result:**  
Button appears with a different style, breaking design consistency across the portal.

**Category:** UI / Design  

**Severity:** Low  

**Evidence:**  
[p4-ss-18](ScreenShot/p4-ss-18.png)

[↩️](#top)

---

