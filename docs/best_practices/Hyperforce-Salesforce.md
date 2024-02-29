---
sidebar_position: 4
---

# Hyperforce Salesforce

The migration to Hyperforce Salesforce represents a significant step for Salesforce customers, promising an enhanced cloud infrastructure offering improved security, scalability, and regional compliance. Here is a summary of key information, potential impacts, and recommended actions to prepare your Salesforce instance for this migration.

## **Advantages of Hyperforce**

   - Scalability: Hyperforce allows unlimited growth for your business.

   - Security and Privacy: Data is encrypted both at rest and in transit, ensuring enhanced security.

   - Flexibility: Operates across global public clouds, enabling better management of data residency.

https://www.grazitti.com/blog/elevate-your-digital-endeavors-with-salesforce-hyperforce/.

## **Impacts and Preparations**

1. Migration of Production Instance Only:

   - Only production instances are migrated to Hyperforce. If you have sandbox instances, you will need to recreate or refresh them after the migration.

2. Read-Only Access:

   - During the migration, your Salesforce organization will be in read-only mode. It is advised to pause all Salesforce integrations during this period.

3. Update URLs and IP Ranges:

   - It is essential to remove any hardcoded instance references in your code and update the allowed IP ranges to accommodate the new Hyperforce cloud ranges.

4. Use of My Domain:

   - Activating My Domain in your organization is crucial for the migration. This helps to avoid hardcoded references and facilitates API integrations.

5. Impact Analysis:

   - Before the migration, assess how it will affect your organization. Use Hyperforce Assistant for this analysis.

6. Technical Preparation:

   - Use the Hyperforce Assistant to guide you throughout the migration. This includes removing hardcoded instance references and updating IP whitelist.

## **Business Advantages of Hyperforce**

- Data Localization Choice:
   - Hyperforce allows you to choose where your data is stored, making compliance with local regulations easier.
- Enhanced Security:
   - With advanced features such as data encryption, your information is more secure.
- Improved Performance:
   - Hyperforce optimizes performance, allowing developers to work more efficiently.

## **In summary**

Migration to Hyperforce requires careful preparation, including updating hardcoded URLs, managing IP ranges, and using My Domain. The benefits of Hyperforce, such as improved security, geographical flexibility, and performance optimization, make this transition advantageous for Salesforce customers. To ensure a successful migration, become familiar with the tools and resources provided by Salesforce, such as Hyperforce Assistant, and plan accordingly to minimize impact on your daily operations.


## **Manual Actions to Take:**

- Prepare the production org to check for any elements that need modification in the organization. The verification process sends a report at each step if there are any issues in the organization.
- Remove all hardcoded code in Salesforce (URLs, tokens, IP addresses, etc.).
- Stop all batch jobs during the migration.





## 1. Step:

Translate to English: "In the quick find, search for the term 'Hyperforce Assistant'.

![Hyperforce-Assistant](./img/Hyperforce-Assistant.JPG)

## 2. Step:

![Capture0](./img/Capture0.JPG)

## 3. Step:

Click on "Not Allowed" to change to "Allowed".
Click on the "Verify" button.

![Capture111](./img/Capture111.JPG)

![Capture1](./img/Capture1.JPG)

![Capture01](./img/Capture01.JPG)

## 4. Step:

Click on the "Verify" button.

![Capture4](./img/Capture4.JPG)

## 5. Step:

Click on the "Verify" button.

![Capture5](./img/Capture5.JPG)

![Capture6](./img/Capture6.JPG)

## 6. Step:

Click on "Complete".
Click on the "Verify" button.

![Capture7](./img/Capture7.JPG)

![Capture8](./img/Capture8.JPG)



## 7. Step:

Click on "Complete".
Click on the "Verify" button.

![Capture9](./img/Capture9.JPG)

![Capture10](./img/Capture10.JPG)

## 8. Step:

Click on "Complete".
Click on the "Verify" button.

![Capture11](./img/Capture11.JPG)

![Capture12](./img/Capture12.JPG)

Otherwise, in case of issues during verification, you can click on the 'Get Help' button.

![CaptureSupport](./img/CaptureSupport.JPG)

If everything goes well, you will receive an email confirming the status: Verified.

![CaptureFin](./img/CaptureFin.JPG)

In the quick find, search for the term 'Optimizer'.

Click on the 'Open Optimizer' button.

![Capture001](./img/Capture001.JPG)

Click on the 'Run Optimizer' button.

![CaptureRun](./img/CaptureRun.JPG)

![CaptureOptimizer](./img/CaptureOptimizer.JPG)



You will receive an email "Your Salesforce Optimization results are ready."

![emailOrg](./img/emailOrg.JPG)

In our sandbox, there are 5 features to fix:

These items are not blockers for the migration.

![listFeature](./img/listFeature.JPG)
