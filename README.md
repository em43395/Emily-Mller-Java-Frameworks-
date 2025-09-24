# WESTERN GOVERNORS UNIVERSITY 
#JAVA FRAMEWORKS

## Task C: Customize Main page
- File: `mainscreen.html`
  - Line 14: Changed `<title>` to `Em’s Craft Store`
    - ![img_5.png](img_5.png)
  - Line 19: Changed `<h1>` to `Em's Craft Store`
    - ![img_6.png](img_6.png)
  - Line 21: Changed `<h2>` to `Craft Supplies`
    - ![img_4.png](img_4.png)
  - Line 53: Changed `<h2>` to `Craft Kits`
    - ![img_2.png](img_2.png)
## Task D: Add about page
- File: `about.html`
  - Line 6: Set the `<title>` to "About Em's Craft Store"
    - ![img_7.png](img_7.png)
  - Lines 9-15: Added an `<h1>` heading, a store description, and included a "Back to inventory" link
    - ![img_8.png](img_8.png)
- File: `MainScreenControllerr.java`
  - Line 56-59: Created a new `aboutPage()` method with `@GetMapping("/about")` 
    - ![img.png](img.png)
- File: `mainscreen.html`
  - Line 20: Inserted an "about" button so users can navigate to the About page
    - ![img_1.png](img_1.png)

## Task E: Add Sample Inventory
- File: `BootStrapData.java`
  -Lines 44-105: Created 5 parts and 5 products 
  - ![img_9.png](img_9.png)
  - ![img_3.png](img_3.png)
  - ![img_10.png](img_10.png)
## Task F: Add "buy Now" Button
- File: `mainscreen.html`
  - Lines 90: added "Buy Now" button to mainscreen
    - ![img_11.png](img_11.png)
- File: `AddProductController.java`
  - Lines 177-194: Created the BuyProduct method
    - ![img_12.png](img_12.png)
- File: `Failure.html`
  - Created failure page when inventory is lower than 1
    - ![img_13.png](img_13.png)
- File: `Success.html`
  - Created success page when a product is successfully purchased
    - ![img_14.png](img_14.png)
  
## Task G: Add Min/Max Inventory Fields
- File: `Part.java`
  - Lines 33-36: created min and max inventory variables
    - ![img_15.png](img_15.png)
  - Lines 91-103: created min and max inventory getters and setters
    - ![img_16.png](img_16.png)
  - Line 23: added annotation for new ValidInventory interface
    - ![img_17.png](img_17.png)
- File: `mainscreen.html`
  - Lines 49-50: added min and max inventory fields to parts table
    - ![img_18.png](img_18.png)
- File: `BootStrapData.java`
  - Lines 52-93: added min and max inventory to parts
    - ![img_9.png](img_9.png)
    - ![img_3.png](img_3.png)
-File: `application.properties`
  -Line 6: changed the file name the persistent storage is saved to
    - ![img_19.png](img_19.png)
- File: `InhousePartForm.html`
  - Line 26-30: added min and max inventory fields to form
    - ![img_20.png](img_20.png)
- File: `OutsourcedPartForm.html`
  - Line 26-30: added min and max inventory fields to form
    - ![img_22.png](img_22.png)
- File `InventoryValidator.java` and File `ValidInventory.java`
  - created Inventory validator class to enforce `minInv <= inv <= maxInv`
    - ![img_24.png](img_24.png)

  
## Task H: Add Validation Messages
- File `InventoryValidator.java`
  - Used previously created validator class
    - ![img_25.png](img_25.png)
- File: `InhousePartForm.html`
  - Line 33-37: added error message field
    - ![img_21.png](img_21.png)
- File `OutsourcedPartForm.html`
  - Line 34-38: added error message field
    - ![img_23.png](img_23.png)
- File `EnufPartsValidator.java`
  - checks to see if associated parts will fall below min when updating or adding a product
    - ![img_26.png](img_26.png)
- File `ValidEnufParts.java`
    - ![img_27.png](img_27.png)

## Task I: Unit Tests for Inventory Bounds
- File `PartTest.java`
  - Lines 159-174: Added two unit tests for the minimum and maximum fields
    - ![img_28.png](img_28.png)

## Task J: Remove Unused Validators
- File `DeletePartValidator`
  - Removed file
- File `ValidDeletePart`
  - removed file
- File `Part.Java`
  - Line 2: removed "import com.example.demo.validators.ValidDeletePart;"
  - Line 19: removed "@ValidDeletePart"

## What do I get in each kit?
- I'm Glad you asked! With our "My First Crochet Project" kit you'll receive the Red Heart brand yarn, one of MeMaw's Best Hooks, and a beginner-friendly Em's Original Pattern that explains all the stitches you'll need to know! 
- With our "My First Cross Stitch Project" kit, you'll receive DMC embroidery floss, a DMC embroidery needle, and one of Em's Original Patterns!
- We know crafting can get intense! That's why we've created our "Supply Run" line of kits! With our "Crochet Supply Run" kit, we've put together your choice of Red Heart yarn, and your choice of one of MeMaw's Best Hooks!
- For our busy bee Cross stitch folks, we have our "Cross Stitch Supply Run" kit that includes your choice of DMC Embroidery Floss and a DMC Embroidery Needle. 
- If you're new to crafting and you'd like to dive in head first? We reccommend our "I'll take one of each please" kit! As the kit says, you'll get to take home one of each of our fine supply collection!
