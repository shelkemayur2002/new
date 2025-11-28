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

<a id="management-portal"></a>

# **GTVL Management Portal — Bug Report**

---
## **Module 1 — SKUs**
---

### **Bug-id : P1-BG-1**

**Description:**  
1. In the SKU list, all action icons (View, Edit, Delete) are unresponsive.  
2. Clicking any icon does not trigger any navigation or action.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-1](ScreenShot/p1-ss-1.png)

---

### **Bug-id : P1-BG-2**

**Description:**  
1. The SKU list does not include a Clear Filters button.  
2. Once a filter is applied, there is no way to reset the list to default view.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p1-ss-2](ScreenShot/p1-ss-2.png)

---

### **Bug-id : P1-BG-3**

**Description:**  
1. System allows creation of a new SKU even when the SKU Code already exists.  
2. No validation or warning is shown for duplicate SKU codes.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-3](ScreenShot/p1-ss-3.png)

---

## **Module 2 — Stores**
---

### **Bug-id : P1-BG-4**

**Description:**  
1. ZIP/Postal Code field accepts alphabetic characters.  
2. No validation prevents the user from entering non-numeric data.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-4](ScreenShot/p1-ss-4.png)

---

### **Bug-id : P1-BG-5**

**Description:**  
1. When entering a phone number in the Create Store form, the field does not allow deleting characters.  
2. Backspace and delete keys do not work once input is typed.  
3. User cannot correct or modify the phone number after typing.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-5](ScreenShot/p1-ss-5.png)

---

### **Bug-id : P1-BG-6**

**Description:**  
1. All action icons (View, Edit, Delete) in the Store Directory do not work.  
2. Clicking any icon does not trigger any response.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-6](ScreenShot/p1-ss-6.png)

---

### **Bug-id : P1-BG-7**

**Description:**  
1. The Store Directory page has filters but no Clear Filters or Reset button.  
2. Once filters are applied, the user cannot reset the view easily.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p1-ss-7](ScreenShot/p1-ss-7.png)

---

### **Bug-id : P1-BG-8**

**Description:**  
1. The Export button on the Store Directory page is unresponsive.  
2. Clicking the button does not trigger any file download or popup.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-8](ScreenShot/p1-ss-8.png)

---

## **Module 3 — Supervisors**
---

### **Bug-id : P1-BG-9**

**Description:**  
1. The system allows creating multiple supervisors with the same name.  
2. The Name field also accepts numeric characters (e.g., “John123”).  
3. No validation exists to restrict the name field to alphabetic characters only.  
4. This results in inconsistent and incorrect supervisor records.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-9](ScreenShot/p1-ss-9.png)

---

### **Bug-id : P1-BG-10**

**Description:**  
1. While creating a new supervisor, the phone number input field stops accepting backspace/delete after entering partial input (e.g., “(555)”).  
2. User cannot edit or remove characters once typed.  
3. Only page refresh resets the field.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-10](ScreenShot/p1-ss-10.png)

---

## **Module 4 — Promodizers**
---

### **Bug-id : P1-BG-11**

**Description:**  
1. The system allows creating promodizers with duplicate names.  
2. The Name field accepts numeric characters (e.g., “Mayur123”).  
3. No validation enforces alphabet-only names.  
4. This results in incorrect and inconsistent employee records.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p1-ss-11](ScreenShot/p1-ss-11.png)

---

### **Bug-id : P1-BG-12**

**Description:**  
1. The “Create Promodizer” button shows a loading state (“Creating…”) even before clicking.  
2. Invalid data still triggers the loading state.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-12](ScreenShot/p1-ss-12.png)

---

### **Bug-id : P1-BG-13**

**Description:**  
1. When editing a promodizer, the phone number field remains in an error state even when entering a valid format (e.g., +1-555-0301).  
2. The system incorrectly flags the input as invalid.  
3. The Update Promodizer button stays disabled, preventing any updates.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p1-ss-13](ScreenShot/p1-ss-13.png)

---

### **Bug-id : P1-BG-14**

**Description:**  
1. The external-link icon in each store card does not redirect to the store details page.  
2. The close (X) button on the popup is non-functional.  
3. User is forced to refresh the page to exit the popup.

**Category:**  Functional / UI  

**Severity:**  High  

**Evidence:**  [p1-ss-14](ScreenShot/p1-ss-14.png)

---

## **Module 5 — Dashboard**
---

### **Bug-id : P1-BG-15**

**Description:**  
1. On the Management Dashboard, each module card contains a right-arrow icon intended for quick navigation.  
2. Clicking these arrows does nothing.  
3. No page navigation or action is triggered.

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

### **Bug-id : P2-BG-1**

**Description:**  
1. The Home button icon (top-right corner) is not fixed in a consistent position.  
2. Its placement shifts across different modules such as Record Sales, Sales History, and Attendance.  
3. This creates UI inconsistency and may confuse users.

**Category:** UI  

**Severity:** Medium  

**Evidence:**  [p2-ss-1](ScreenShot/p2-ss-1.jpg)

---

## **Module 2 — Sales History**
---

### **Bug-id : P2-BG-2**

**Description:**  
1. After recording a sale successfully, the entry appears correctly in Sales History.  
2. When clicking any sales entry, the Sales Detail page opens but shows “Sales record not found”.  
3. The system fails to load the sale description even though the sale history card displays the sale information.

**Category:** Functional  

**Severity:** High  

**Evidence:**  [p2-ss-2](ScreenShot/p2-ss-2.png)

---

## **Module 3 — Attendance History**
---

### **Bug-id : P2-BG-3**

**Description:**  
1. In the Attendance History Calendar View, all dates for the entire month are listed under the Sunday column.  
2. Other weekday columns (Mon–Sat) remain empty.  
3. The calendar grid fails to position dates according to correct weekdays.  
4. This makes the calendar view unusable and misleading.

**Category:** UI / Functional  

**Severity:** Medium  

**Evidence:**  [p2-ss-3](ScreenShot/p2-ss-3.png)

---

## **Module 4 — My Profile**
---

### **Bug-id : P2-BG-4**

**Description:**  
1. The My Profile page displays user information only on the left portion of the page.  
2. A large empty space appears on the right side, making the layout look incomplete.  
3. Page content does not stretch to utilize available width.  
4. Overall UI looks unbalanced and visually unappealing.

**Category:** UI  

**Severity:** Low  

**Evidence:**  [p2-ss-4](ScreenShot/p2-ss-4.png)

---

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

**Category:** UI / Functional  

**Severity:** Medium  

**Evidence:**  [p2-ss-5](ScreenShot/p2-ss-5.png)

---

### **Bug-id : P2-BG-6**

**Description:**  
The feedback form does not successfully save or submit any feedback.  
Submission always fails, and no feedback is stored.

**Category:** Functional  

**Severity:** High  

**Evidence:**  [p2-ss-6](ScreenShot/p2-ss-6.png)

---
<a id="sales-analytics-portal"></a>

# **GTVL Sales Analytics Dashboard — Bug Report**


---

## **Module 1 — SKU Performance**

---

### **Bug-id : P3-BG-1**

**Description:**  
The **SKU Performance Analysis** screen contains multiple UI alignment issues:  
1. The **Filters panel** is not aligned properly with the SKU table header section.  
2. The **Total Quantity Sold (Min–Max)** input fields are uneven and visually misaligned.  
These inconsistencies affect UI clarity and overall user experience.

**Category:**  UI  

**Severity:**  Low  

**Evidence:**  [p3-ss-1](ScreenShot/p3-ss-1.png)

---

### **Bug-id : P3-BG-2**

**Description:**  
1. When a search input is applied in the SKU Performance module, a filter tag appears with a clear (X) button.  
2. Clicking the **X** does not remove the applied search filter.  
3. The search field also does not reset, and the results remain unchanged.

**Category:**  Functional  

**Severity:**  Low  

**Evidence:**  [p3-ss-2](ScreenShot/p3-ss-2.png)

---

### **Bug-id : P3-BG-3**

**Description:**  
1. The **Clear All** button in the Filters panel does not reset the **Status** checkboxes.  
2. Even after clicking **Clear All**, the **Active** checkbox remains selected.  
3. Other filters may reset, but the status filter does not clear.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-3](ScreenShot/p3-ss-3.png)

---

### **Bug-id : P3-BG-4**

**Description:**  
1. When selecting **Custom Range** from the Date Range dropdown, no date picker or calendar modal opens.  
2. User cannot select a start date or end date.  
3. The Custom Range option becomes unusable and does not filter SKU data.

**Category:**  Functional / UI 

**Severity:**  Medium  

**Evidence:**  [p3-ss-4](ScreenShot/p3-ss-4.png)

---

### **Bug-id : P3-BG-5**

**Description:**  
1. The **Total Quantity Sold** filter allows users to enter negative numbers (e.g., -55 to -60).  
2. Negative quantities make no logical sense in sales analytics.  
3. System applies the filter and displays results with negative range.

**Category:**  Functional / Validation 

**Severity:**  Medium  

**Evidence:**  [p3-ss-5](ScreenShot/p3-ss-5.png)

---

### **Bug-id : P3-BG-6**

**Description:**  
1. When both **Active** and **Inactive** checkboxes are unchecked in the Status filter, the system shows a tag **“Status: None Selected”**.  
2. System treats this as a filter condition instead of removing all filtering.  
3. As a result, SKU table displays **“No SKUs Found”**, even though SKUs exist.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-6](ScreenShot/p3-ss-6.png)

---

### **Bug-id : P3-BG-7**

**Description:**  
1. When both Status options (Active + Inactive) are selected, the filter tag incorrectly shows: **“Status: Inactive Only”**.  
2. This misrepresents the actual filter condition and causes confusion.

**Category:**  Functional / UI 

**Severity:**  Medium  

**Evidence:**  [p3-ss-7](ScreenShot/p3-ss-7.png)

---

## **Module 2 — Store Performance**

---

### **Bug-id : P3-BG-8**

**Description:**  
1. In the **Store Performance** module, some table columns are **not visible in desktop view** due to horizontal overflow.  
2. Right-side columns like **SKUs Sold**, **Active Staff**, **Last Sale Date** become hidden.  
3. All columns are visible only in mobile view (verified).

**Category:**  UI / Layout  

**Severity:**  Medium  

**Evidence:**  [p3-ss-8](ScreenShot/p3-ss-8.png)

---

### **Bug-id : P3-BG-9**

**Description:**  
1. The **Sales Volume** filter accepts negative values in Min and Max fields.  
2. Negative sales volume is logically invalid.  
3. System still applies the filter and shows values like **Sales: -55 – 55**.

**Category:**  Functional / Validation  

**Severity:**  Medium  

**Evidence:**  [p3-ss-9](ScreenShot/p3-ss-9.png)

---

## **Module 3 — Staff Performance**

---

### **Bug-id : P3-BG-10**

**Description:**  
1. Filter tags in Staff Performance show an **X** button to clear each filter.  
2. Clicking the **X** does nothing.  
3. Filters remain applied and table does not refresh.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-10](ScreenShot/p3-ss-10.png)

---

### **Bug-id : P3-BG-11**

**Description:**  
1. Clicking any employee row should open employee details.  
2. Instead, page shows **“Staff Not Found”** with empty fields.  
3. No employee data loads even when valid employees are selected.

**Category:**  Functional  

**Severity:**  High  

**Evidence:**  [p3-ss-11](ScreenShot/p3-ss-11.png)

---

### **Bug-id : P3-BG-12**

**Description:**  
1. In Staff Performance, both Role checkboxes (Promodizer & Supervisor) are auto-checked.  
2. Clicking **Clear All Filters** does **not** uncheck these boxes.  
3. Role filter remains active and cannot be fully reset.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-12](ScreenShot/p3-ss-12.png)

---

## **Module 4 — Transaction History**

---

### **Bug-id : P3-BG-13**

**Description:**  
1. In Transaction History, **Store** and **Staff** checkbox filters do NOT reset after clicking **Clear All**.  
2. All values remain checked.  
3. Filter state cannot be reset without manually unchecking every entry.

**Category:**  Functional  

**Severity:**  Medium  

**Evidence:**  [p3-ss-13](ScreenShot/p3-ss-13.png)

---
### **Bug-id : P3-BG-14** 

**Description:**  
1. The Total Quantity Range filter in Transaction History allows negative numbers (e.g., -555, -66).  
2. System accepts and applies these invalid values when filtering.

**Expected Result:** Total Quantity Range should not accept negative values.  
**Actual Result:** System accepts negative values and applies the filter.

**Category:**  Functional / Validation  

**Severity:**  Medium  

**Evidence:**  [p3-ss-14](ScreenShot/p3-ss-14.png)

---
### **Bug-id : P3-BG-15** 

**Description:**  
1. The **Clear All** text appears without any button styling or visible button structure.  
2. Its position is incorrect — it is placed at the top instead of below the **Apply Filters** button.

**Expected Result:** Clear All should appear as a properly styled button placed below Apply Filters.  
**Actual Result:** Clear All appears as plain text and is positioned incorrectly at the top.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p3-ss-15](ScreenShot/p3-ss-15.png)

---
### **Bug-id : P3-BG-16** 

**Description:**  
1. The table headers **Role** and **Submission ID** have a different text style compared to other table headers.  
2. The **sorting arrows (up/down)** seen on other columns are missing for these two headers.  
3. This causes UI inconsistency within the Transaction History table.

**Expected Result:** Role and Submission ID headers should match other headers and show sorting arrows.  
**Actual Result:** Headers have different styling and no sorting arrows are displayed.

**Category:**  UI  

**Severity:**  Medium  

**Evidence:**  [p3-ss-16](ScreenShot/p3-ss-16.png)

---
<a id="supervisor-portal"></a>

# **gtvl-supervisor-portal — Bug Report**

---

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

---
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

---
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

---
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

---
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

---
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

---
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

---
