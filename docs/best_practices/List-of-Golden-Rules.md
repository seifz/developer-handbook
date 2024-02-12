---
sidebar_position: 1
---

# List of Golden Rules

## 1. **KISS:**
   - "keep it simple, stupid" → Think about the next developer during implementation & long-term maintenance.

## 2. **Applying naming conventions:**
   - They will facilitate the search and identification of metadata in a highly complex system in the long run.

## 3. **Code documentation:**
   - Use the description field if available; otherwise, adhere to the documentation header. Include the User Story number.

## 4. **Factorizing code + Cleaning up dead code:**
   - Aim to limit the number of code characters by factorizing whenever possible; do not hesitate to use SObjects to avoid typing a method.

## 5. **Bulkifying processes:**
   - Always think that you need to handle a "Collection of records" and not a single record. The number of SOQL queries and DML operations should never change based on the number of records processed.

## 6. **Consolidating Triggers:**
   - One trigger per object & no business logic in triggers.

## 7. **Escaping/Bypassing automations:**
   - Any rule/automation should be easily disabled without modification (by simply modifying a Parameter).

## 8. **hardcoded:**
   - No Salesforce identifiers "hardcoded" in the code (record type, report, user...).

## 9. **Always consider Salesforce Governor Limits:**
   - Pay attention to target volumes and list executions.

## 10. **Pooling :**
   - needs (Interface, Class, ...) by playing with Design Patterns and avoiding duplicates.





