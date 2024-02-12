# Golden Rules: TOP 10



1. Follow the **PascalCase naming convention** (example: TotalAverageAmount) for API names and avoid special characters in API names as well as Page Layout names.
    1. Naming convention for Flows (TypeFlow_Object_Number_Description).
    2. API names for technical fields on an object should have the suffix "Tech".

2. Any configuration outside of pre/post deployment actions is prohibited on all environments (INT, UAT, etc.). Changes should be pushed to the repository through the SFDX deployment process.

3. Configuration documentation: Always fill in the description fields with the Jira number.

4. All picklists should be global picklists.

5. Avoid using Salesforce identifiers "hardcoded" (record type, report, user, etc.) in the configuration, reports: they vary from one environment to another. Use Custom Labels and Static Resources if possible.

6. Following best practices for [Flow Builder](https://admin.salesforce.com/blog/2021/the-ultimate-guide-to-flow-best-practices-and-standards) implementation includes:

    1. Always enable Auto-Layout.
    2. Aim for one Record Trigger flow per object if possible.
    3. Report each significant modification in the description field. 
7. Create the minimum necessary profiles starting from the Minimum Access standard profile, then add permission sets on top. Profiles should only contain:

    1. layoutAssignments

    2. recordTypeVisibilities

    3. applicationVisibilities

    4. pageAccesses

    5. LoginIpRanges

8. "Bypass" of automations (Flow, Trigger, Apex, etc.): Any rule/automation should be easily disabled without modification (by simply modifying a custom permission, custom settings, or custom metadata type).

9. Always consider Salesforce Governor Limits: Pay attention to target volumes and list executions.
10. Use the VS Code extension "chuckjonas.apex-pmd" to validate each Apex file through this [PMD](https://docs.pmd-code.org/latest/pmd_rules_apex.html) and following [best practices](https://apexstepbystep.com/apex-best-practices/) ([test classes](https://developer.salesforce.com/docs/atlas.en-us.apexcode.meta/apexcode/apex_testing_best_practices.htm#!); [triggers and bulk](https://developer.salesforce.com/docs/atlas.en-us.apexcode.meta/apexcode/apex_triggers_bestpract.htm#!); [functions](https://developer.salesforce.com/docs/platform/functions/guide/patterns-and-practices#patterns-for-apex-developers); [the 15 apex commandments](https://developer.salesforce.com/blogs/developer-relations/2015/01/apex-best-practices-15-apex-commandments)). [Flow Naming Conventions](https://wiki.sfxd.org/books/best-practices/page/flow-naming-conventions)

##  **Exemples :**
| Field Label      | Name API              | Description              |
| ------------------------------------ | ------------------ |------------------ |
|Type of Establishment                   | TypeEstablishment__c|The establishment type of an account|
| Number of secondary establishments attached| NumberOfSecondaryEstablishmentsAttached__c|The number of secondary establishments attached to the account|
| Number of company contacts | NumberOfCompanyContactsTech__c                      |The number of company contacts attached to the account                      |

| Field type      | Prefix       | Suffix              |
| ------------------------------------ | ------------------ |------------------ |
|Boolean | Est ou A ou Peut|            | 
| Automatically populated technical field||Tech|

| Type      | Name API       |Description  |
| ------------------------------------ | ------------------ |------------------ |
|Screen Flow | FL01_AddQuoteLines |            | 
| Autolaunched Flow |AFL01_AppelApex |     |
| Scheduled Flow  |BFL01_SendBirthdayEmails  |     |
| Before Update Flow, on Account |RTFL01_ACC_BeforeUpdate  |     |
| After Update Flow, on Account  |RTFL02_ACC_AfterUpdate  |     |
| Record-triggered Email-sending Flow, on Account.  |EFL01_AccountEmails  |     |