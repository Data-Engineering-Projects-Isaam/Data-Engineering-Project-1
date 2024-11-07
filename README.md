# Project: How to Monitor AWS CloudTrail Logs using AWS Glue, PySpark, and Save on Datadog Subscription

## Steps:

1. **Extract CloudTrail Data**  
   - Call the CloudTrail API to retrieve events, which return nested JSON data.

2. **Flatten the Data**  
   - Use `StructType` to flatten the JSON structure and focus on specific data points of interest.

3. **Extract Table Access Details**  
   - Modify the extraction logic to specifically retrieve details about tables accessed, including:
     - **Database Name**
     - **Table Name**
     - **User Name**
