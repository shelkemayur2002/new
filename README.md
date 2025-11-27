# ERP SYSTEM
---
<h1 align="center"> Day-1 </h1>

# Create Pull request
---
<h1 align="center"> Day-2 </h1>

[ Back to Top](#gvtl-sales-analytics-dashboard--bug-report)

---
# **GTVL Management Portal — Bug Report**
* This document contains a consolidated list of UI and Functional defects identified during manual testing of the GTVL Management Portal.
* The portal includes four modules: SKUs, Stores, Supervisors, and Promodizers.
* The objective of this assignment was to test all modules thoroughly and document every issue clearly for developers.
---
## **Module 1 — SKUs**
---
### **Bug-id : P1-BG-1**

**Title:** SKU Actions Not Working

**Description:**  
1. In the SKU list, all action icons (View, Edit, Delete) are unresponsive.  
2. Clicking any icon does not trigger any navigation or action.

**Category:** Functional  
**Severity:** High  
**Priority:** P1

**Precondition:**  
User must be on the SKUs List page in the GTVL Management Portal.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Go to SKUs  
3. Locate the Actions column  
4. Click View, Edit, or Delete

**Expected Result:**  
1. View → Should open SKU details  
2. Edit → Should navigate to edit form  
3. Delete → Should show confirmation and delete SKU

**Actual Result:**  
1. None of the action buttons work  
2. No navigation or popup appears

**Screenshot Reference:**  [p1-ss-1](ScreenShot/p1-ss-1.png)

---

### **Bug-id : P1-BG-2**

**Title:** Clear Filters Missing

**Description:**  
1. The SKU list does not include a **Clear Filters** button.  
2. Once a filter is applied, there is no way to reset the list to default view.

**Category:** UI  
**Severity:** Medium  
**Priority:** P2

**Precondition:**  
At least one search filter or field value must be applied in the SKUs list.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to SKUs  
3. Apply any filter or search  
4. Try to find a Clear / Reset button

**Expected Result:**  
1. A visible **Clear Filters** button should be available  
2. Clicking it should reset search and filters

**Actual Result:**  
1. No clear/reset option exists  
2. User must manually remove each filter

**Screenshot Reference:**  [p1-ss-2](ScreenShot/p1-ss-2.png)

---
### **Bug-id : P1-BG-3**

**Title:** Duplicate SKU Codes Allowed

**Description:**  
1. System allows creation of a new SKU even when the SKU Code already exists.  
2. No validation or warning is shown for duplicate SKU codes.

**Category:** Functional  
**Severity:** High  
**Priority:** P1

**Precondition:**  
At least one SKU must already exist with a valid SKU Code.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to SKUs  
3. Click on Add New SKU  
4. Enter an existing SKU Code  
5. Save the form

**Expected Result:**  
1. System should prevent duplicate SKU codes  
2. A validation message should appear (“SKU Code already exists”)

**Actual Result:**  
1. SKU is created with a duplicate code  
2. No validation or warning is displayed

**Screenshot Reference:**  [p1-ss-3](ScreenShot/p1-ss-3.png)

---
## **Module 2 — Stores**

---
### **Bug-id : P1-BG-4**

**Title:** Zip Code Accepts Letters

**Description:**  
1. ZIP/Postal Code field accepts alphabetic characters.  
2. No validation prevents the user from entering non-numeric data.

**Category:** Functional  
**Severity:** High  
**Priority:** P1

**Precondition:**  
User must be on the **Add New Store** form.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to Stores  
3. Click **Add New Store**  
4. Enter letters into the Zip/Postal Code field

**Expected Result:**  
1. Field should only allow numeric input  
2. Validation error should appear if letters are entered

**Actual Result:**  
1. Letters are accepted  
2. Store can be submitted with invalid ZIP code

**Screenshot Reference:**  [p1-ss-4](ScreenShot/p1-ss-4.png)

---
### **Bug-id : P1-BG-5**

**Title:** Phone Number Field Does Not Allow Deletion or Backspace

**Description:**  
1. When entering a phone number in the Create Store form, the field does not allow deleting characters.  
2. Backspace and delete keys do not work once input is typed.  
3. User cannot correct or modify the phone number after typing.

**Category:** Functional  
**Severity:** High  
**Priority:** P1

**Precondition:**  
User must be on the **Add New Store** page with input typed in the phone number field.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Stores → Add New Store**  
3. Enter a phone number in the Phone Number field  
4. Try to press Backspace or Delete  

**Expected Result:**  
1. User should be able to delete or edit phone number characters  
2. Field should support normal text editing behavior  

**Actual Result:**  
1. Backspace/Delete does not work  
2. User is forced to refresh or reopen the form to correct the number  

**Screenshot Reference:**  [p1-ss-5](ScreenShot/p1-ss-5.png)

---
### **Bug-id : P1-BG-6**

**Title:** Store Actions Not Working

**Description:**  
1. All action icons (View, Edit, Delete) in the Store Directory do not work.  
2. Clicking any icon does not trigger any response.

**Category:** Functional  
**Severity:** High  
**Priority:** P1

**Precondition:**  
Store records must be visible in the Store Directory table.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Stores**  
3. Scroll to the **Store Directory** section  
4. Click any action icon (View, Edit, Delete)

**Expected Result:**  
1. View → Should open Store details  
2. Edit → Should open Edit Store page  
3. Delete → Should show confirmation popup  

**Actual Result:**  
1. No action is performed  
2. No popup or navigation occurs  

**Screenshot Reference:**  [p1-ss-6](ScreenShot/p1-ss-6.png)

---
### **Bug-id : P1-BG-7**

**Title:** Clear Filters Missing in Store Directory

**Description:**  
1. The Store Directory page has filters but no Clear Filters or Reset button.  
2. Once filters are applied, the user cannot reset the view easily.

**Category:** UI  
**Severity:** Medium  
**Priority:** P2

**Precondition:**  
At least one filter (Status, Assignment, or Search) must be applied in the Store Directory.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Stores**  
3. Apply any filter (Status, Assignment, Search)  
4. Try to reset the filters

**Expected Result:**  
1. A Clear Filters button should be visible  
2. Clicking it should reset all applied filters

**Actual Result:**  
1. No option exists to clear filters  
2. User must manually remove each filter

**Screenshot Reference:**  [p1-ss-7](ScreenShot/p1-ss-7.png)

---
### **Bug-id : P1-BG-8**

**Title:** Export Button Not Functional

**Description:**  
1. The Export button on the Store Directory page is unresponsive.  
2. Clicking the button does not trigger any file download or popup.

**Category:** Functional  
**Severity:** Medium  
**Priority:** P2

**Precondition:**  
Store Directory page must be loaded with store records visible.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Stores**  
3. Locate the **Export** button (top-right of Store Directory)  
4. Click the Export button

**Expected Result:**  
1. A CSV or Excel file should start downloading  
2. Exported store data should be delivered

**Actual Result:**  
1. Nothing happens when the button is clicked  
2. No download, popup, or system feedback

**Screenshot Reference:**  [p1-ss-8](ScreenShot/p1-ss-8.png)

---
## **Module 3 — Supervisors**

---
### **Bug-id : P1-BG-9**

**Title:** Supervisor Name Field Allows Duplicates and Numbers

**Description:**  
1. The system allows creating multiple supervisors with the same name.  
2. The Name field also accepts numeric characters (e.g., “John123”).  
3. No validation exists to restrict the name field to alphabetic characters only.  
4. This results in inconsistent and incorrect supervisor records.

**Category:** Functional  
**Severity:** Medium  
**Priority:** P2

**Precondition:**  
At least one supervisor record should already exist for duplication to occur.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Supervisors → Add New Supervisor**  
3. Enter a duplicate name or a name containing numeric characters  
4. Save the record

**Expected Result:**  
1. System should prevent duplicate supervisor names  
2. Name field should not accept numeric characters  
3. Validation message should appear for invalid inputs

**Actual Result:**  
1. Duplicate supervisor names are created  
2. System accepts names containing numbers without any warning

**Screenshot Reference:**  [p1-ss-9](ScreenShot/p1-ss-9.png)

---
### **Bug-id : P1-BG-10**

**Title:** Phone Number Field Does Not Allow Backspace or Deletion

**Description:**  
1. While creating a new supervisor, the phone number input field stops accepting backspace/delete after entering partial input (e.g., `(555)`).  
2. User cannot edit or remove characters once typed.  
3. Only page refresh resets the field.

**Category:** Functional  
**Severity:** High  
**Priority:** P1

**Precondition:**  
User must be on the **Add New Supervisor** page with some characters already entered in the phone field.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Supervisors → Add New Supervisor**  
3. Start typing in the Phone Number field (e.g., `(555)`)  
4. Try pressing Backspace or Delete

**Expected Result:**  
1. Backspace/Delete should allow removing characters  
2. User should be able to freely edit the phone number

**Actual Result:**  
1. Field becomes locked  
2. Backspace/Delete do not work  
3. User cannot correct the phone number

**Screenshot Reference:**  [p1-ss-10](ScreenShot/p1-ss-10.png)

---
## **Module 4 — Promodizers**

---
### **Bug-id : P1-BG-11**

**Title:** Promodizer Name Field Allows Duplicates and Numbers

**Description:**  
1. The system allows creating promodizers with duplicate names.  
2. The Name field accepts numeric characters (e.g., “Mayur123”).  
3. No validation enforces alphabet-only names.  
4. This results in incorrect and inconsistent employee records.

**Category:** Functional  
**Severity:** Medium  
**Priority:** P2

**Precondition:**  
At least one promodizer with the same name should already exist in the system.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Promodizers → Add New Promodizer**  
3. Enter an existing promodizer name or a name containing numbers  
4. Save the form

**Expected Result:**  
1. System should block duplicate names  
2. Name field should accept only alphabetical characters  
3. Proper validation messages should appear

**Actual Result:**  
1. Duplicate promodizer names are created  
2. Numeric characters in the name field are accepted without warnings

**Screenshot Reference:**  [p1-ss-11](ScreenShot/p1-ss-11.png)

---
### **Bug-id : P1-BG-12**

**Title:** Create Promodizer Button Stuck on “Creating…”.

**Description:**  
1. The “Create Promodizer” button shows a loading state (“Creating…”) even before clicking.  
2. Invalid data (numbers in names, incorrect formats) still triggers the loading state.

**Category:** Functional  
**Severity:** High  
**Priority:** P1

**Precondition:**  
User must be on the **Add New Promodizer** form with incomplete or invalid inputs entered.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Promodizers → Add New Promodizer**  
3. Enter incomplete or invalid input values (e.g., invalid name, wrong email format)  
4. Notice the button showing “Creating…” even before clicking  
5. Click **Create Promodizer**

**Expected Result:**  
1. Button should remain in normal state until valid data is entered  

**Actual Result:**  
1. Button shows “Creating…” in advance  

**Screenshot Reference:**  [p1-ss-12](ScreenShot/p1-ss-12.png)

---
### **Bug-id : P1-BG-13**

**Title:** Cannot Update Promodizer Even With Valid Phone Number Format

**Description:**  
1. When editing a promodizer, the phone number field remains in an error state even when entering a valid format (e.g., `+1-555-0301`).  
2. The system incorrectly flags the input as invalid.  
3. The **Update Promodizer** button stays disabled, preventing any updates.  
4. User cannot save changes due to incorrect phone validation.

**Category:** Functional  
**Severity:** High  
**Priority:** P1

**Precondition:**  
User must open the **Edit Promodizer** form for any existing promodizer.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Promodizers → Select any Promodizer → Edit**  
3. Enter a valid phone number format (e.g., `+1-555-0301`)  
4. Observe that the field still shows an error  
5. Try clicking **Update Promodizer**

**Expected Result:**  
1. Valid phone number should be accepted  
2. Error border should disappear  
3. Update button should enable  
4. Promodizer details should save successfully

**Actual Result:**  
1. Phone number is marked invalid  
2. Error message remains  
3. Update button stays disabled  
4. User is unable to update promodizer details

**Screenshot Reference:**  [p1-ss-13](ScreenShot/p1-ss-13.png)

---
### **Bug-id : P1-BG-14**

**Title:** Assigned Stores Popup — Redirect & Close Button Not Working

**Description:**  
When clicking the “Assigned Stores” count for any promodizer, a popup appears showing the list of assigned stores.  
1. The external-link icon in each store card does not redirect to the store details page.  
2. The close (X) button on the popup is non-functional and does not close the popup.  
3. User is forced to refresh the page to exit the popup.

**Category:** Functional / UI  
**Severity:** High  
**Priority:** P1

**Precondition:**  
A promodizer must have at least one assigned store to display the popup.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Promodizers** module  
3. Click the “X stores” link under the **Assigned Stores** column  
4. Popup appears  
5. Click the **external link icon**  
6. Click the **close (X)** button

**Expected Result:**  
1. External link should redirect to the respective store details page  
2. Close (X) button should close the popup

**Actual Result:**  
1. External link does nothing  
2. Close button does nothing  
3. Popup remains stuck on the screen until page refresh

**Screenshot Reference:**  [p1-ss-14](ScreenShot/p1-ss-14.png)

---
## **Module 5 — Dashboard**

---
### **Bug-id : P1-BG-15**

**Title:** Dashboard Navigation Arrows Not Working

**Description:**  
1. On the Management Dashboard, each module card (SKUs, Stores, Supervisors, Promodizers) contains a right-arrow icon intended for quick navigation.  
2. Clicking these arrows does nothing.  
3. No page navigation or action is triggered.

**Category:** Functional  
**Severity:** Medium  
**Priority:** P2

**Precondition:**  
User must be on the **Dashboard** page of the GTVL Management Portal.

**Steps to Reproduce:**  
1. Open GTVL Management Portal  
2. Navigate to **Dashboard**  
3. Click the right-arrow icon on:  
   - SKU Management  
   - Store Management  
   - Supervisors  
   - Promodizers  
4. Observe the behavior

**Expected Result:**  
Clicking the arrow should navigate to the respective module page:  
1. SKU Management → SKUs List  
2. Store Management → Stores List  
3. Supervisors → Supervisor List  
4. Promodizers → Promodizer List

**Actual Result:**  
1. No navigation happens  
2. Arrows are completely unresponsive

**Screenshot Reference:**  [p1-ss-15](ScreenShot/p1-ss-15.png)

---
<h1 align="center"> Day-3 </h1>

---
# **GTVL Promodizer Portal — Bug Report**

---
## **Module 1 — Dashboard**

---
### **Bug-id : P2-BG-1**

**Title:** Home Button Icon Position Not Consistent Across Pages

**Description:**  
1. The Home button icon (top-right corner) is not fixed in a consistent position.  
2. Its placement shifts across different modules such as **Record Sales**, **Sales History**, and **Attendance**.  
3. This creates UI inconsistency and may confuse users.

**Category:** UI  

**Severity:** Medium  
**Priority:** P2  

**Precondition:**  
User must be logged into the **GTVL Promodizer Portal**.

**Steps to Reproduce:**  
1. Open GTVL Promodizer Portal  
2. Navigate to **Record Sales**  
3. Observe the position of the Home icon  
4. Navigate to **Sales History**  
5. Navigate to **Attendance**  
6. Compare Home icon placement across screens  

**Expected Result:**  
The Home icon should remain in a **fixed and consistent** position across all screens.

**Actual Result:**  
The Home icon **changes position** in different sections, breaking UI alignment.

**Screenshot Reference:**  [p2-ss-1](ScreenShot/p2-ss-1.jpg)

---
## **Module 2 — Sales History**

---
### **Bug-id : P2-BG-2**

**Title:** Sales Description Page Not Loading After Recording Sales

**Description:**  
1. After recording a sale successfully, the entry appears correctly in **Sales History**.  
2. When clicking any sales entry, the **Sales Detail** page opens but shows “Sales record not found”.  
3. The system fails to load the sale description even though the sale history card displays the sale information.

**Category:** Functional  
**Severity:** High  
**Priority:** P1  

**Precondition:**  
A sales entry must already be recorded in the **Record Sales** module.

**Steps to Reproduce:**  
1. Open **GTVL Promodizer Portal**  
2. Navigate to **Record Sales**  
3. Select a store → Click **Start Scanning** → Record a sale  
4. After successful submission, go to **Sales History**  
5. Click on the newly recorded sale entry  
6. Observe the behavior on the **Sales Detail** page

**Expected Result:**  
1. Sales Detail page should display full sale information  
   - Item details  
   - Batch number  
   - Store  
   - Submission timestamp  
2. Page should load without errors

**Actual Result:**  
1. Sales Detail page shows:  
   **“Sales record not found — The requested sales submission could not be found or may have been deleted.”**  
2. No sale description is displayed  
3. User cannot view recorded sale details  

**Screenshot Reference:**  [p2-ss-2](ScreenShot/p2-ss-2.png)

------
## **Module 3 — Attendance History**

---
### **Bug-id : P2-BG-3**

**Title:** Calendar View Not Aligned — All Dates Displayed Under Sunday Only

**Description:**  
1. In the Attendance History **Calendar View**, all dates for the entire month are listed under the **Sunday** column.  
2. Other weekday columns (Mon–Sat) remain empty.  
3. The calendar grid fails to position dates according to correct weekdays.  
4. This makes the calendar view unusable and misleading.

**Category:** UI / Functional  
**Severity:** Medium  
**Priority:** P2  

**Precondition:**  
User must navigate to **Attendance History → Calendar View** in the Promodizer Portal.

**Steps to Reproduce:**  
1. Open **GTVL Promodizer Portal**  
2. Navigate to **Attendance History**  
3. Switch to **Calendar View**  
4. Scroll through the month view  
5. Observe how all dates appear only under the **Sunday** column  

**Expected Result:**  
1. Dates should be positioned correctly based on actual weekdays  
   - Example: If 1 November 2025 is a Saturday, it should appear under **SAT**  
2. Calendar grid should reflect an accurate month layout

**Actual Result:**  
1. All dates (1–30/31) are shown only under the **SUN** column  
2. Monday–Saturday columns remain empty  
3. Calendar structure is invalid and confusing  

**Screenshot Reference:**  [p2-ss-3](ScreenShot/p2-ss-3.png)

---
## **Module 4 — My Profile**

---
### **Bug-id : P2-BG-4**

**Title:** My Profile Layout Has Excessive Empty Space on Right Side

**Description:**  
1. The **My Profile** page displays user information only on the left portion of the page.  
2. A large empty space appears on the right side, making the layout look incomplete.  
3. Page content does not stretch to utilize available width.  
4. Overall UI looks unbalanced and visually unappealing.

**Category:** UI  
**Severity:** Low  
**Priority:** P3  

**Precondition:**  
User must be logged into the **GTVL Promodizer Portal** and navigate to **My Profile**.

**Steps to Reproduce:**  
1. Open **GTVL Promodizer Portal**  
2. Navigate to **My Profile** from left sidebar  
3. Observe the layout structure  

**Expected Result:**  
1. Profile content should be centered or properly expanded to fill available screen width.  
2. Layout should look visually balanced and polished.  

**Actual Result:**  
1. Significant unused empty space appears on the right side.  
2. Page looks unoptimized and visually incomplete.  

**Screenshot Reference:**  
[p2-ss-4](ScreenShot/p2-ss-4.png)

---
### **Bug-id : P2-BG-5**

**Title:** Sidebar Active State Not Updating Consistently (Highlight & Green Indicator Issues)

**Description:**  
The sidebar navigation in the Promodizer Portal does not correctly update the active state when moving between modules.  
This issue appears in two ways:

**1. Green Active Indicator Does Not Move**  
- The small green light/backlight stays fixed on **Dashboard**.  
- It does not follow the currently selected menu option.

**2. Sidebar Highlight (Background Selection) Works Only for Some Items**  
- Highlight appears correctly for:  
  - Dashboard  
  - Record Sales  
  - My Stores  
  - My Profile  
- Highlight does **NOT** appear for:  
  - Sales History  
  - Attendance  
  - Attendance History  
This makes the sidebar visually inconsistent and confusing for the user.

**Category:** UI / Functional  
**Severity:** Medium  
**Priority:** P2  

**Precondition:**  
User must be logged into the **GTVL Promodizer Portal**.

**Steps to Reproduce:**  
1. Open **GTVL Promodizer Portal**  
2. Observe sidebar highlight & green indicator on **Dashboard**  
3. Navigate to different modules like:  
   - Sales History  
   - Attendance  
   - Attendance History  
4. Observe sidebar behavior  
5. Notice that  
   - Green indicator does not move  
   - Highlight is missing for several modules

**Expected Result:**  
1. The green active-indicator should always move to the menu item currently opened.  
2. Sidebar highlight should be consistently applied to **every** active menu item.  
3. All modules should correctly reflect which page is currently selected.

**Actual Result:**  
1. Green indicator stays fixed on Dashboard.  
2. Highlight appears only for some menus and is missing on others.  
3. Sidebar does not visually update based on navigation.

**Screenshot Reference:**  [p2-ss-5](ScreenShot/p2-ss-5.png)

---
### **Bug-id : P2-BG-6**

**Title:** Feedback Submission Not Saved

**Description:**  
The feedback form does not successfully save or submit any feedback.  
Submission always fails, and no feedback is stored.

**Category:** Functional  

**Severity:** High  

**Priority:** P2  

**Steps to Reproduce:**  
1. Open **GTVL Promodizer Portal**  
2. Click the **Feedback** button  
3. Fill in all required fields  
4. Click **Submit**

**Expected Result:**  
Feedback should be saved and a success message should appear.

**Actual Result:**  
An error message appears and the feedback is **not saved**.

**Screenshot Reference:**  [p2-ss-6](ScreenShot/p2-ss-6.png)

---
# **GTVL Sales Analytics Dashboard — Bug Report**

---
## **Module 1 — SKU Performance**

---
### **Bug-id : P3-BG-1**

**Title:** Filters Panel & Min–Max Input Fields Misaligned in SKU Performance Module

**Description:**  
The **SKU Performance Analysis** screen contains multiple UI alignment issues:
1. The **Filters panel** is not aligned properly with the SKU table header section.  
2. The **Total Quantity Sold (Min–Max)** input fields are uneven and visually misaligned.  
These inconsistencies affect UI clarity and overall user experience.

**Category:** UI  
**Severity:** Low  
**Priority:** P3  

**Precondition:**  
User must be on the **SKU Performance** page in the Sales Analytics Dashboard.

**Steps to Reproduce:**  
1. Open **Sales Analytics Dashboard**  
2. Navigate to **SKU Performance**  
3. Observe the alignment between:  
   - The Filters panel  
   - The main table header  
   - The Min–Max input fields  
4. Notice misalignment on both areas.

**Expected Result:**  
1. Filters panel should align consistently with the main content and table header.  
2. Min–Max input fields should have equal height, spacing, and alignment.

**Actual Result:**  
1. Filters panel appears shifted and does not align with the overall layout.  
2. Min–Max input boxes are uneven and misaligned.

**Screenshot Reference:**  [p3-ss-1](ScreenShot/p3-ss-1.png)

---
### **Bug-id : P3-BG-2**

**Title:** Search Filter Clear (X) Button Not Working

**Description:**  
1. When a search input is applied in the SKU Performance module, a filter tag appears with a clear (X) button.  
2. Clicking the **X** does not remove the applied search filter.  
3. The search field also does not reset, and the results remain unchanged.

**Category:** Functional  
**Severity:** Low  
**Priority:** P3  

**Precondition:**  
A SKU search must be applied using the search bar.

**Steps to Reproduce:**  
1. Open **Sales Analytics Dashboard**  
2. Navigate to **SKU Performance**  
3. Enter any SKU code in the search bar (e.g., `GTVL-BEV-001`)  
4. Press Enter → Search tag appears  
5. Click the **X** button on the search tag  

**Expected Result:**  
- The search tag should disappear  
- Search filter should be cleared  
- Results should reset to the full SKU list  
- Search bar should become empty  

**Actual Result:**  
- Clicking the **X** does nothing  
- Search filter remains applied  
- Results do not reset  

**Screenshot Reference:**  [p3-ss-2](ScreenShot/p3-ss-2.png)

---
### **Bug-id : P3-BG-3**

**Title:** “Clear All” Button Does Not Reset Status Filters (Active Checkbox Remains Checked)

**Description:**  
1. The **Clear All** button in the Filters panel does not reset the **Status** checkboxes.  
2. Even after clicking **Clear All**, the **Active** checkbox remains selected.  
3. Other filters may reset, but the status filter does not clear.

**Category:** Functional  
**Severity:** Medium  
**Priority:** P3  

**Precondition:**  
At least one filter (Active/Inactive) must be applied in the SKU Performance page.

**Steps to Reproduce:**  
1. Open **Sales Analytics Dashboard**  
2. Navigate to **SKU Performance**  
3. Check the **Active** status checkbox  
4. Click the **Clear All** button  
5. Observe the status filter section  

**Expected Result:**  
- All filters should reset  
- All checkboxes should be unchecked  
- No filters should remain selected  

**Actual Result:**  
- **Active** checkbox remains checked  
- Filter is not fully cleared  
- User must manually uncheck the checkbox  

**Screenshot Reference:**  [p3-ss-3](ScreenShot/p3-ss-3.png)

---
### **Bug-id : P3-BG-4**

**Title:** Custom Date Range Option Does Not Open Any Date Picker

**Description:**  
1. When selecting **Custom Range** from the Date Range dropdown, no date picker or calendar modal opens.  
2. User cannot select a start date or end date.  
3. The Custom Range option becomes unusable and does not filter SKU data.

**Category:** Functional / UI  
**Severity:** Medium  
**Priority:** P3  

**Precondition:**  
User must be on the **SKU Performance** page of the Sales Analytics Dashboard.

**Steps to Reproduce:**  
1. Open **Sales Analytics Dashboard**  
2. Navigate to **SKU Performance**  
3. Click the **Date Range** dropdown  
4. Select **Custom Range**  
5. Observe that nothing appears after selection

**Expected Result:**  
- A **calendar date picker** should appear  
- User should be able to select **From Date** and **To Date**  
- Data should refresh based on selected range  

**Actual Result:**  
- No date picker appears  
- User cannot choose custom dates  
- Custom range filtering is impossible  

**Screenshot Reference:**  [p3-ss-4](ScreenShot/p3-ss-4.png)

---
### **Bug-id : P3-BG-5**

**Title:** Total Quantity Sold Filter Accepts Negative Values

**Description:**  
1. The **Total Quantity Sold** filter allows users to enter negative numbers (e.g., -55 to -60).  
2. Negative quantities make no logical sense in sales analytics.  
3. System applies the filter and displays results with negative range even though sales quantity cannot be negative.  

**Category:** Functional / Validation  
**Severity:** Medium  
**Priority:** P3  

**Precondition:**  
User must be on the **SKU Performance Analysis** page.

**Steps to Reproduce:**  
1. Open **Sales Analytics Dashboard**  
2. Navigate to **SKU Performance**  
3. Scroll down to **Filters → Total Quantity Sold**  
4. Enter negative values in Min and Max fields  
5. Click **Apply Filters**

**Expected Result:**  
1. Total Quantity Sold field should **not** accept negative values.  
2. Input validation should restrict values to `0` or greater.  
3. Error message or red border should appear for invalid input.

**Actual Result:**  
1. Negative values are accepted.  
2. Filter applies successfully with invalid numeric range.  
3. Tag shows invalid input: `Quantity: -55 - ∞`.

**Screenshot Reference:**  [p3-ss-5](ScreenShot/p3-ss-5.png)

---
### **Bug-id : P3-BG-6**

**Title:** Status Filter Misbehavior — Shows “No SKUs Found” When No Option Is Selected

**Description:**  
1. When both **Active** and **Inactive** checkboxes are unchecked in the Status filter, the system shows a tag **“Status: None Selected”**.  
2. Instead of showing all SKUs, the system treats it as a filter condition.  
3. This results in the SKU table displaying **“No SKUs Found”**, even though SKUs exist.  
4. “No selection” should mean **no filter applied**, not “empty status”.

**Category:** Functional  
**Severity:** Medium  
**Priority:** P3  

**Precondition:**  
User must be on **SKU Performance Analysis** page.

**Steps to Reproduce:**  
1. Open **Sales Analytics Dashboard**  
2. Go to **SKU Performance**  
3. Under **Status**, uncheck both:  
   - Active  
   - Inactive  
4. Click **Apply Filters**

**Expected Result:**  
- When no checkbox is selected, the system should display **all SKUs**, regardless of status.  
- No filter tag should be shown because no filtering condition is set.

**Actual Result:**  
- A tag appears: **“Status: None Selected”**  
- SKU list becomes empty and shows **“No SKUs Found”**, incorrectly applying a filter.

**Screenshot Reference:**  [p3-ss-6](ScreenShot/p3-ss-6.png)

---
### **Bug-id : P3-BG-7**

**Title:** Status Filter Incorrectly Shows “Inactive Only” Even When Both Active & Inactive Are Selected

**Description:**  
1. When **both** Status checkboxes (Active + Inactive) are checked, the applied filter tag incorrectly displays:  
   **“Status: Inactive Only”**  
2. The system applies the wrong label even though both statuses are selected.  
3. This creates confusion and gives the impression that Active SKUs are not included.

**Category:** Functional / UI  
**Severity:** Medium  
**Priority:** P3  

**Precondition:**  
User must be on **SKU Performance Analysis** page.

**Steps to Reproduce:**  
1. Open **Sales Analytics Dashboard**  
2. Navigate to **SKU Performance**  
3. Under **Status**, check:  
   - Active  
   - Inactive  
4. Click **Apply Filters**  
5. Observe the filter summary tag above the table.

**Expected Result:**  
- If both options are selected, filter tag should show:  
  **“Status: Active & Inactive”**  
  OR  
  **“Status: All”**  
- Behavior should clearly indicate that no restriction is applied on status.

**Actual Result:**  
- Filter summary incorrectly shows:  
  **“Status: Inactive Only”**  
- This misrepresents the applied filter and creates confusion.

**Screenshot Reference:**  [p3-ss-7](ScreenShot/p3-ss-7.png)

