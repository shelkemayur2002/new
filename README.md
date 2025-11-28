# 🏢 ERP(Enterprise Resource Planning) SYSTEM
---
## 📘 Introduction

This document contains a comprehensive and structured list of defects identified across the four GTVL portals during exploratory testing. All bugs are organized module-wise to maintain clarity and ensure easy review. Shortcut navigation links are provided at the top of the file to allow reviewers to directly jump to each portal’s bug list. Every bug entry follows a standardized format to maintain consistency, improve readability, and help developers quickly understand the issue, its expected behavior, and supporting evidence.

---

## 📝 Bug Fields Used

Each bug in this document is documented using the following fields:

- **Bug-id**  
- **Description**  
- **Expected**  
- **Actual**  
- **Category**  
- **Severity**  
- **Evidence**

---


**Click below to navigate directly to the bug list for each portal:**

[Management Portal](#management-portal)
  
[Promodizer Portal](#promodizer-portal)

[Sales Analytics Dashboard](#sales-analytics-portal)

[Supervisor Portal](#supervisor-portal)

---
<h1 align="center">⭐ Day-1 ⭐</h1>

## Generate A Pull Request

------
<h1 align="center">⭐ Day-2 ⭐</h1>

---
<a id="management-portal"></a>

# **GTVL Management Portal — Bug Report**

---
## **Module 1 — SKUs**
---

### **🐞Bug-id : P1-BG-1**

**Description:**  
1. In the SKU list, all action icons (View, Edit, Delete) are unresponsive.  
2. Clicking any icon does not trigger any navigation or action.

**Expected Result:** All SKU action buttons should work properly.  
**Actual Result:** View/Edit/Delete do not respond when clicked.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-1](ScreenShot/p1-ss-1.png)

---

### **🐞Bug-id : P1-BG-2**

**Description:**  
1. The SKU list does not include a Clear Filters button.  
2. Once a filter is applied, there is no way to reset the list to default view.

**Expected Result:** Clear Filters button should reset the applied filters.  
**Actual Result:** No option to clear filters; user must manually remove each filter.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p1-ss-2](ScreenShot/p1-ss-2.png)

---

### **🐞Bug-id : P1-BG-3**

**Description:**  
1. System allows creation of a new SKU even when the SKU Code already exists.  
2. No validation or warning is shown for duplicate SKU codes.

**Expected Result:** System should not allow duplicate SKU codes.  
**Actual Result:** Duplicate SKUs are created without any validation message.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-3](ScreenShot/p1-ss-3.png)

---

## **Module 2 — Stores**
---

### **🐞Bug-id : P1-BG-4**

**Description:**  
1. ZIP/Postal Code field accepts alphabetic characters.  
2. No validation prevents the user from entering non-numeric data.

**Expected Result:** ZIP code field should allow only numeric values.  
**Actual Result:** Alphabetic characters are accepted.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-4](ScreenShot/p1-ss-4.png)

---

### **🐞Bug-id : P1-BG-5**

**Description:**  
1. When entering a phone number in the Create Store form, the field does not allow deleting characters.  
2. Backspace and delete keys do not work once input is typed.  
3. User cannot correct or modify the phone number after typing.

**Expected Result:** User should be able to edit/delete phone number normally.  
**Actual Result:** Backspace/Delete do not work; phone cannot be edited.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-5](ScreenShot/p1-ss-5.png)

---

### **🐞Bug-id : P1-BG-6**

**Description:**  
1. All action icons (View, Edit, Delete) in the Store Directory do not work.  
2. Clicking any icon does not trigger any response.

**Expected Result:** Store actions should open details/edit/delete as expected.  
**Actual Result:** Icons do nothing when clicked.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-6](ScreenShot/p1-ss-6.png)

---

### **🐞Bug-id : P1-BG-7**

**Description:**  
1. The Store Directory page has filters but no Clear Filters or Reset button.  
2. Once filters are applied, the user cannot reset the view easily.

**Expected Result:** Clear Filters button should reset all applied filters.  
**Actual Result:** No option available to clear filters.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p1-ss-7](ScreenShot/p1-ss-7.png)

---

### **🐞Bug-id : P1-BG-8**

**Description:**  
1. The Export button on the Store Directory page is unresponsive.  
2. Clicking the button does not trigger any file download or popup.

**Expected Result:** Export button should download CSV/Excel file.  
**Actual Result:** No response when clicking Export.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-8](ScreenShot/p1-ss-8.png)

---

## **Module 3 — Supervisors**
---

### **🐞Bug-id : P1-BG-9**

**Description:**  
1. The system allows creating multiple supervisors with the same name.  
2. The Name field also accepts numeric characters (e.g., “John123”).  
3. No validation exists to restrict the name field to alphabetic characters only.

**Expected Result:** Name should not allow numbers or duplicates.  
**Actual Result:** System accepts numeric/duplicate names without validation.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-9](ScreenShot/p1-ss-9.png)

---

### **🐞Bug-id : P1-BG-10**

**Description:**  
1. While creating a new supervisor, the phone number input field stops accepting backspace/delete after entering partial input (e.g., “(555)”).  
2. User cannot edit or remove characters once typed.

**Expected Result:** Backspace/Delete should work normally.  
**Actual Result:** Phone field becomes locked after partial entry.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-10](ScreenShot/p1-ss-10.png)

---

## **Module 4 — Promodizers**
---

### **🐞Bug-id : P1-BG-11**

**Description:**  
1. The system allows creating promodizers with duplicate names.  
2. The Name field accepts numeric characters (e.g., “Mayur123”).  
3. No validation enforces alphabet-only names.

**Expected Result:** No duplicates; no numeric characters allowed.  
**Actual Result:** System accepts duplicates and numbers.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-11](ScreenShot/p1-ss-11.png)

---

### **🐞Bug-id : P1-BG-12**

**Description:**  
1. The “Create Promodizer” button shows a loading state (“Creating…”) even before clicking.  
2. Invalid data still triggers the loading state.

**Expected Result:** Button should load only after clicking with valid data.  
**Actual Result:** Button shows loading even before action.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-12](ScreenShot/p1-ss-12.png)

---

### **🐞Bug-id : P1-BG-13**

**Description:**  
1. When editing a promodizer, the phone number field remains in an error state even when entering a valid format (e.g., +1-555-0301).  
2. The Update Promodizer button stays disabled.

**Expected Result:** Valid phone numbers should be accepted; update enabled.  
**Actual Result:** Shows error & disables update button.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-13](ScreenShot/p1-ss-13.png)

---

### **🐞Bug-id : P1-BG-14**

**Description:**  
1. Assigned Stores popup external-link does not redirect to store details.  
2. Close (X) button does not close the popup.

**Expected Result:** External link should open store details; close should work.  
**Actual Result:** Neither redirect nor close works.

**Category:**  Functional / UI  

**Severity:**  High  

**Evidence:**  [p1-ss-14](ScreenShot/p1-ss-14.png)

---

## **Module 5 — Dashboard**
---

### **🐞Bug-id : P1-BG-15**

**Description:**  
1. Dashboard module cards contain right-arrow icon for quick navigation.  
2. Clicking these arrows does nothing.

**Expected Result:** Should navigate to respective module pages.  
**Actual Result:** Arrow icons are unresponsive.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-15](ScreenShot/p1-ss-15.png)

---
<h1 align="center">⭐ Day-3 ⭐</h1>

---
<a id="promodizer-portal"></a>

# **GTVL Promodizer Portal — Bug Report**

---
## **Module 1 — Dashboard**
---

### **🐞Bug-id : P2-BG-1**

**Description:**  
1. The Home button icon is not fixed in a consistent position.  
2. It shifts across different modules such as Record Sales, Sales History, and Attendance.

**Expected Result:** Home icon should stay in a fixed consistent position.  
**Actual Result:** Home icon changes position across pages.

**Category:** UI  

**Severity:** Medium  

**Evidence:**  [p2-ss-1](ScreenShot/p2-ss-1.jpg)

---

## **Module 2 — Sales History**
---

### **🐞Bug-id : P2-BG-2**

**Description:**  
1. After recording a sale, the entry appears in Sales History.  
2. Clicking the sale shows “Sales record not found”.

**Expected Result:** Sales details should load correctly.  
**Actual Result:** Sales Detail page shows “record not found”.

**Category:** Functional  

**Severity:** High  

**Evidence:**  [p2-ss-2](ScreenShot/p2-ss-2.png)

---

## **Module 3 — Attendance History**
---

### **🐞Bug-id : P2-BG-3**

**Description:**  
1. Calendar View shows all dates under Sunday column.  
2. Monday–Saturday columns remain empty.

**Expected Result:** Dates should align correctly with weekdays.  
**Actual Result:** All dates appear under Sunday only.

**Category:** UI / Functional  

**Severity:** Medium  

**Evidence:**  [p2-ss-3](ScreenShot/p2-ss-3.png)

---

## **Module 4 — My Profile**
---

### **🐞Bug-id : P2-BG-4**

**Description:**  
1. My Profile page uses only the left area of the screen.  
2. Right side has a large empty space.

**Expected Result:** Layout should be centered and properly spaced.  
**Actual Result:** Large empty right space makes layout unbalanced.

**Category:** UI  

**Severity:** Low  

**Evidence:**  [p2-ss-4](ScreenShot/p2-ss-4.png)

---

### **🐞Bug-id : P2-BG-5**

**Description:**  
Sidebar navigation does not update active state correctly.

**Expected Result:** Green indicator & highlight should move with active item.  
**Actual Result:** Green light stays on Dashboard; highlight missing for several items.

**Category:** UI / Functional  

**Severity:** Medium  

**Evidence:**  [p2-ss-5](ScreenShot/p2-ss-5.png)

---

### **🐞Bug-id : P2-BG-6**

**Description:**  
Feedback form does not successfully submit any feedback.

**Expected Result:** Feedback should save & show success message.  
**Actual Result:** Error message appears; feedback not saved.

**Category:** Functional  

**Severity:** High  

**Evidence:**  [p2-ss-6](ScreenShot/p2-ss-6.png)

---

<a id="sales-analytics-portal"></a>

# **GTVL Sales Analytics Dashboard — Bug Report**

---

## **Module 1 — SKU Performance**
---

### **🐞Bug-id : P3-BG-1**

**Description:**  
Filters panel and Min–Max input fields are misaligned.

**Expected Result:** Filters panel and inputs should align consistently.  
**Actual Result:** Both appear uneven and misaligned.

**Category:**  UI  

**Severity:**  Low  

**Evidence:**  [p3-ss-1](ScreenShot/p3-ss-1.png)

---

### **🐞Bug-id : P3-BG-2**

**Description:**  
Search filter clear (X) button does not remove applied filter.

**Expected Result:** X should clear search and reset results.  
**Actual Result:** Clicking X does nothing.

**Category:**  Functional  

**Severity:**  Low  

**Evidence:**  [p3-ss-2](ScreenShot/p3-ss-2.png)

---

### **🐞Bug-id : P3-BG-3**

**Description:**  
Clear All button does not reset Status filters (Active remains checked).

**Expected Result:** All filters including Status should reset.  
**Actual Result:** Active checkbox remains checked.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-3](ScreenShot/p3-ss-3.png)

---

### **🐞Bug-id : P3-BG-4**

**Description:**  
Custom Range does not open a date picker.

**Expected Result:** Date picker should open for selecting range.  
**Actual Result:** Nothing appears when Custom Range is selected.

**Category:**  Functional / UI 

**Severity:**  Medium  

**Evidence:**  [p3-ss-4](ScreenShot/p3-ss-4.png)

---

### **🐞Bug-id : P3-BG-5**

**Description:**  
Total Quantity Sold filter accepts negative values.

**Expected Result:** Negative values should not be accepted.  
**Actual Result:** System accepts and applies negative range.

**Category:**  Functional / Validation 

**Severity:**  Medium  

**Evidence:**  [p3-ss-5](ScreenShot/p3-ss-5.png)

---

### **🐞Bug-id : P3-BG-6**

**Description:**  
When both Active & Inactive are unchecked, system shows “Status: None Selected” and returns no results.

**Expected Result:** Should show all SKUs if nothing is selected.  
**Actual Result:** Shows empty list with “None Selected”.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-6](ScreenShot/p3-ss-6.png)

---

### **🐞Bug-id : P3-BG-7**

**Description:**  
When both statuses are selected, tag incorrectly shows “Inactive Only”.

**Expected Result:** Should show “Active & Inactive” or “All”.  
**Actual Result:** Shows “Inactive Only”.

**Category:**  Functional / UI 

**Severity:**  Medium  

**Evidence:**  [p3-ss-7](ScreenShot/p3-ss-7.png)

---

## **Module 2 — Store Performance**
---

### **🐞Bug-id : P3-BG-8**

**Description:**  
Some table columns are not visible in desktop view due to overflow.

**Expected Result:** All columns should be visible with scrolling.  
**Actual Result:** Columns on the right are clipped/hidden.

**Category:**  UI / Layout  

**Severity:**  Medium  

**Evidence:**  [p3-ss-8](ScreenShot/p3-ss-8.png)

---

### **🐞Bug-id : P3-BG-9**

**Description:**  
Sales Volume filter accepts negative values.

**Expected Result:** Only non-negative values should be accepted.  
**Actual Result:** Negative values are applied successfully.

**Category:**  Functional / Validation  

**Severity:**  Medium  

**Evidence:**  [p3-ss-9](ScreenShot/p3-ss-9.png)

---

## **Module 3 — Staff Performance**
---

### **🐞Bug-id : P3-BG-10**

**Description:**  
Filter tag X button does not remove filters.

**Expected Result:** X should remove filter and refresh data.  
**Actual Result:** Tag remains; filter stays applied.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-10](ScreenShot/p3-ss-10.png)

---

### **🐞Bug-id : P3-BG-11**

**Description:**  
Employee detail page shows “Staff Not Found”.

**Expected Result:** Employee details should load correctly.  
**Actual Result:** Empty page with “Not Found”.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p3-ss-11](ScreenShot/p3-ss-11.png)

---

### **🐞Bug-id : P3-BG-12**

**Description:**  
Clear All does not reset Role filters.

**Expected Result:** Role checkboxes should uncheck when clearing filters.  
**Actual Result:** Both checkboxes remain checked.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-12](ScreenShot/p3-ss-12.png)

---

## **Module 4 — Transaction History**
---

### **🐞Bug-id : P3-BG-13**

**Description:**  
Store and Staff checkbox filters do not reset when Clear All is clicked.

**Expected Result:** Clear All should uncheck Store & Staff checkboxes.  
**Actual Result:** All checkboxes remain checked after Clear All.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-13](ScreenShot/p3-ss-13.png)

---

### **🐞Bug-id : P3-BG-14** 

**Description:**  
Total Quantity Range filter allows negative inputs.

**Expected Result:** Only non-negative quantity should be allowed.  
**Actual Result:** System accepts negative values.

**Category:**  Functional / Validation  

**Severity:**  Medium  

**Evidence:**  [p3-ss-14](ScreenShot/p3-ss-14.png)

---

### **🐞Bug-id : P3-BG-15** 

**Description:**  
Clear All text appears without button structure.

**Expected Result:** Clear All should appear as a styled button in correct place.  
**Actual Result:** Plain text, placed incorrectly at the top.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p3-ss-15](ScreenShot/p3-ss-15.png)

---

### **🐞Bug-id : P3-BG-16** 

**Description:**  
Role & Submission ID headers have different styling and missing sorting arrows.

**Expected Result:** Headers should match others & show sort arrows.  
**Actual Result:** Different style + no sorting arrows.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p3-ss-16](ScreenShot/p3-ss-16.png)

---
<h1 align="center">⭐ Day-4 ⭐</h1>
<a id="supervisor-portal"></a>

# **gtvl-supervisor-portal — Bug Report**

---

### **🐞Bug-id : P4-BG-1**

**Description:**  
1. Even after marking attendance as **Present** in Attendance Management,  
2. The Dashboard still shows **Not Marked** for Today’s Attendance.  
3. System does not update dashboard status after marking attendance.

**Expected Result:** Dashboard should display **Present** once attendance is marked.  
**Actual Result:** Dashboard continues showing **Not Marked** even after attendance is recorded.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p4-ss-1](ScreenShot/p4-ss-1.png)

---
### **🐞Bug-id : P4-BG-2**

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

---
### **🐞Bug-id : P4-BG-3**

**Description:**  
1. In the Attendance module, users can only **Mark Attendance (Clock In)** but there is **no option to Clock Out**.  
2. As a result, the **Clock Out Time** field always displays a dash (-).  
3. This prevents recording full attendance data for the day.

**Expected Result:** User should be able to Clock Out, and the Clock Out Time should be recorded properly.

**Actual Result:** No Clock Out feature exists, and Clock Out Time remains blank.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p4-ss-3](ScreenShot/p4-ss-3.png)

---
### **🐞Bug-id : P4-BG-4**

**Description:**  
1. Clicking any Submission ID in Sales History should open the detailed sales record.  
2. Instead, clicking redirects to a "Record Not Found" page.  
3. The system does not pass the submission ID in the URL, causing the detail page to fail.

**Expected Result:** Sales Record Detail page should open and show full submission details.  
**Actual Result:** Page shows “Record Not Found — No submission ID provided in the URL.”

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p4-ss-4](ScreenShot/p4-ss-4.png)

---
### **🐞Bug-id : P4-BG-5**

**Description:**  
1. After adding a promodizer, the Supervisor cannot perform any management actions.  
2. No options/buttons are available to **Add**, **Edit**, or **Delete** a promodizer.  
3. The My Team page only displays promodizer cards without any action controls.

**Expected Result:** Supervisor should see options to Add, Edit, or Delete promodizers on the My Team page.  
**Actual Result:** No management options are visible; supervisor cannot modify promodizers.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p4-ss-5](ScreenShot/p4-ss-5.png)

---
### **🐞Bug-id : P4-BG-6**

**Description:**  
1. The Phone Number field on the Add Promodizer page accepts alphabetic characters.  
2. User can enter letters (e.g., "Mayur") instead of digits.  
3. No validation is applied to restrict input to numeric phone number format.

**Expected Result:** Phone Number field should accept only numeric values and follow a valid phone format.  
**Actual Result:** Field allows alphabetic characters without validation.

**Category:**  Functional / Validation  

**Severity:**  High  

**Evidence:**  [p4-ss-6](ScreenShot/p4-ss-6.png)

---
### **🐞Bug-id : P4-BG-7**

**Description:**  
1. In the My Team module, store and status filters can be applied but cannot be cleared.  
2. There is **no Clear Filters button** to reset selections.  
3. User must manually change dropdowns each time, causing poor usability.

**Expected Result:** A Clear Filters option should reset store and status filters to default.  
**Actual Result:** No Clear Filters option is available; filters stay applied until manually changed.

**Category:**  Functional / UI  

**Severity:**  Medium  

**Evidence:**  [p4-ss-7](ScreenShot/p4-ss-7.png)

---
