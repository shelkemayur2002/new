### Bug-id : P1-BG-1
#**Description:**  
1. In the SKU list, all action icons (View, Edit, Delete) are unresponsive.  
2. Clicking any icon does not trigger any navigation or action.
#**Severity:** High  
#**Evidence:**  p1-ss-1

---

### Bug-id : P1-BG-2

**Description:**  
1. The SKU list does not include a Clear Filters button.  
2. Once a filter is applied, there is no way to reset the list to default view.

**Severity:** Medium  

**Evidence:**  
p1-ss-2

---

### Bug-id : P1-BG-3

**Description:**  
1. System allows creation of a new SKU even when the SKU Code already exists.  
2. No validation or warning is shown for duplicate SKU codes.

**Severity:** High  

**Evidence:**  
p1-ss-3

---

### Bug-id : P1-BG-4

**Description:**  
1. ZIP/Postal Code field accepts alphabetic characters.  
2. No validation prevents the user from entering non-numeric data.

**Severity:** High  

**Evidence:**  
p1-ss-4

---

### Bug-id : P1-BG-5

**Description:**  
1. When entering a phone number in the Create Store form, the field does not allow deleting characters.  
2. Backspace and delete keys do not work once input is typed.  
3. User cannot correct or modify the phone number after typing.

**Severity:** High  

**Evidence:**  
p1-ss-5

---

### Bug-id : P1-BG-6

**Description:**  
1. All action icons (View, Edit, Delete) in the Store Directory do not work.  
2. Clicking any icon does not trigger any response.

**Severity:** High  

**Evidence:**  
p1-ss-6

---

### Bug-id : P1-BG-7

**Description:**  
1. The Store Directory page has filters but no Clear Filters or Reset button.  
2. Once filters are applied, the user cannot reset the view easily.

**Severity:** Medium  

**Evidence:**  
p1-ss-7

---

### Bug-id : P1-BG-8

**Description:**  
1. The Export button on the Store Directory page is unresponsive.  
2. Clicking the button does not trigger any file download or popup.

**Severity:** Medium  

**Evidence:**  
p1-ss-8

---

### Bug-id : P1-BG-9

**Description:**  
1. The system allows creating multiple supervisors with the same name.  
2. The Name field also accepts numeric characters (e.g., “John123”).  
3. No validation exists to restrict the name field to alphabetic characters only.  
4. This results in inconsistent and incorrect supervisor records.

**Severity:** Medium  

**Evidence:**  
p1-ss-9

---

### Bug-id : P1-BG-10

**Description:**  
1. While creating a new supervisor, the phone number input field stops accepting backspace/delete after entering partial input (e.g., `(555)`).  
2. User cannot edit or remove characters once typed.  
3. Only page refresh resets the field.

**Severity:** High  

**Evidence:**  
p1-ss-10

---

### Bug-id : P1-BG-11

**Description:**  
1. The system allows creating promodizers with duplicate names.  
2. The Name field accepts numeric characters (e.g., “Mayur123”).  
3. No validation enforces alphabet-only names.  
4. This results in incorrect and inconsistent employee records.

**Severity:** Medium  

**Evidence:**  
p1-ss-11

---

### Bug-id : P1-BG-12

**Description:**  
1. The “Create Promodizer” button shows a loading state (“Creating…”) even before clicking.  
2. Invalid data (numbers in names, incorrect formats) still triggers the loading state.

**Severity:** High  

**Evidence:**  
p1-ss-12

---

### Bug-id : P1-BG-13

**Description:**  
1. When editing a promodizer, the phone number field remains in an error state even when entering a valid format (e.g., `+1-555-0301`).  
2. The system incorrectly flags the input as invalid.  
3. The Update Promodizer button stays disabled, preventing any updates.  
4. User cannot save changes due to incorrect phone validation.

**Severity:** High  

**Evidence:**  
p1-ss-13

---

### Bug-id : P1-BG-14

**Description:**  
1. The external-link icon in Assigned Stores popup does not redirect to the store details page.  
2. The close (X) button on the popup is non-functional.  
3. User is forced to refresh the page to exit the popup.

**Severity:** High  

**Evidence:**  
p1-ss-14

---

### Bug-id : P1-BG-15

**Description:**  
1. On the Dashboard, each module card contains a right-arrow icon intended for quick navigation.  
2. Clicking these arrows does nothing.  
3. No page navigation or action is triggered.

**Severity:** Medium  

**Evidence:**  
p1-ss-15
