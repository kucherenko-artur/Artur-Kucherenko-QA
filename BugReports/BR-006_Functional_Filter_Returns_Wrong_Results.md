# BR-006 — Category Filter Returns Incorrect Results

**Severity:** High  
**Severity Justification:** Incorrect filtering logic returns irrelevant products across multiple categories, breaking navigation and trust.  
**Priority:** High  
**Status:** Open  
**Component:** Catalog / Filters / Relevance  
**Environment:**  
- Platform: Web  
- Browser: Chrome  
- Device: Windows 11  
- Site Type: E-commerce test environment  

---

## Summary
Category and search filters return unrelated items across multiple product categories.  
Issue appears systemic and reproducible in **Laptops**, **Stands**, **Keyboards**, **Tablets**, **Monitors**, and **Mouse** sections.

---

## Description
Filtering and search relevance logic frequently display items completely unrelated to the selected category.  
Observed incorrect results include furniture, automotive camera systems, compressors, USB hubs, KVM switches, desktop PCs, and household accessories.

This indicates broken category mapping, inconsistent relevance scoring, or recommendation overrides interfering with category integrity.

---

## Steps to Reproduce
1. Open the e-commerce catalog.  
2. Navigate to any category (Laptops, Stands, Monitors, Keyboards, Tablets, Mouse).  
3. Scroll through the product list.  
4. Observe unrelated items appearing inside category-specific results.

---

## Expected Result
Only products matching the selected category or logically related items should appear.

---

## Actual Result
Unrelated products appear in category lists, including:
- furniture (tables, nightstands)  
- car backup camera systems  
- compressors / air dusters  
- DIY controller boards  
- USB hubs, KVM switches  
- full desktop computers  
- generic household items  

---

## Impact Analysis
**User Impact:**  
- Users cannot reliably find products  
- Increased confusion and mistrust  
- Higher abandonment rates  

**Business Impact:**  
- Lower conversion  
- Disrupted product discovery flow  
- Category integrity compromised  

**Technical Impact:**  
- Relevance ranking incorrect  
- Category mapping inconsistent  
- Recommendation logic overrides filter constraints  

---

## Evidence

![Evidence 01](./BR-006_Wrong_Category_Filter_Evidence_01.png)
![Evidence 02](./BR-006_Wrong_Category_Filter_Evidence_02.png)
![Evidence 03](./BR-006_Wrong_Category_Filter_Evidence_03.png)
![Evidence 04](./BR-006_Wrong_Category_Filter_Evidence_04.png)
![Evidence 05](./BR-006_Wrong_Category_Filter_Evidence_05.png)
![Evidence 06](./BR-006_Wrong_Category_Filter_Evidence_06.png)
![Evidence 07](./BR-006_Wrong_Category_Filter_Evidence_07.png)
![Evidence 08](./BR-006_Wrong_Category_Filter_Evidence_08.png)
![Evidence 09](./BR-006_Wrong_Category_Filter_Evidence_09.png)
![Evidence 10](./BR-006_Wrong_Category_Filter_Evidence_10.png)

---

## Conclusion
Filtering and relevance logic produce incorrect product sets across multiple categories.  
Defect is systemic and affects navigation, discoverability, and consistency of search and catalog behavior.
