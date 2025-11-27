# ERP SYSTEM
---
<h1 align="center"> Day-1 </h1>
# **GTVL Management Portal — Bug Report**
* This document contains a consolidated list of UI and Functional defects identified during manual testing of the GTVL Management Portal.
* The portal includes four modules: SKUs, Stores, Supervisors, and Promodizers.
* The objective of this assignment was to test all modules thoroughly and document every issue clearly for developers.

## **Module 1 — SKUs**

### **Bug-id : BG-1**

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

**Screenshot Reference:**  [ss-1](ScreenShot/ss-1.png)

### **Bug-id : BG-2**

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

**Screenshot Reference:**  [ss-2](ScreenShot/ss-2.png)


### **Bug-id : BG-3**

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

**Screenshot Reference:**  [ss-3](ScreenShot/ss-3.png)

## **Module 2 — Stores**

### **Bug-id : BG-4**

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

**Screenshot Reference:**  [ss-4](ScreenShot/ss-4.png)

### **Bug-id : BG-5**

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

**Screenshot Reference:**  [ss-5](ScreenShot/ss-5.png)

### **Bug-id : BG-6**

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

**Screenshot Reference:**  [ss-6](ScreenShot/ss-6.png)

### **Bug-id : BG-7**

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

**Screenshot Reference:**  [ss-7](ScreenShot/ss-7.png)

### **Bug-id : BG-8**

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

**Screenshot Reference:**  [ss-8](ScreenShot/ss-8.png)

## **Module 3 — Supervisors**

### **Bug-id : BG-9**

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

**Screenshot Reference:**  [ss-9](ScreenShot/ss-9.png)

### **Bug-id : BG-10**

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

**Screenshot Reference:**  [ss-10](ScreenShot/ss-10.png)

## **Module 4 — Promodizers**

### **Bug-id : BG-11**

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

**Screenshot Reference:**  [ss-11](ScreenShot/ss-11.png)

### **Bug-id : BG-12**

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

**Screenshot Reference:**  [ss-12](ScreenShot/ss-12.png)

### **Bug-id : BG-13**

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

**Screenshot Reference:**  [ss-13](ScreenShot/ss-13.png)

### **Bug-id : BG-14**

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

**Screenshot Reference:**  [ss-14](ScreenShot/ss-14.png)

## **Module 5 — Dashboard**

### **Bug-id : BG-15**

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

**Screenshot Reference:**  [ss-15](ScreenShot/ss-15.png)

# **GTVL Management Portal — Bug Report**
