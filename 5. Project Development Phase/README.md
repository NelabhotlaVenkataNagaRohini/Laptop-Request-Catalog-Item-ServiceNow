# Project Development Phase

##  Implementation Details

### 1. Update Set Creation
Created a Local Update Set named "Laptop Request Project" and made it current.

### 2. Service Catalog Item
Created a Catalog Item under the Hardware category.

### 3. Variables Added
- Laptop Model (Single Line Text)
- Justification (Multi Line Text)
- Additional Accessories (Checkbox)
- Accessories Details (Multi Line Text)

### 4. Catalog UI Policy
Condition:
Additional Accessories is true

Action:
- Accessories Details → Visible
- Accessories Details → Mandatory
- Reverse if false enabled

### 5. UI Action (Reset Form)
Table: Shopping Cart (sc_cart)
Client-side script:

function resetForm() {
    g_form.clearForm();
    alert("The form has been reset.");
}

### 6. Update Set Export & Import
Exported the update set as XML.
Imported and committed in target instance.

Screenshots and XML files are included in this folder as proof of implementation.
