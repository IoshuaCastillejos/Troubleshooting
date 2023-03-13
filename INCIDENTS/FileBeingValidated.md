# The user is reporting ArcStatus: FileBeingValidated

## STEPS: 
1) Start by identifying the region where the user belongs to. This information can be obtained from the incident details.
2) Obtain the EngagementID from the Incident Details shared by the user.
3) Once you have identified the database server, connect to the database using appropriate credentials and SQL Server Management Studio.
4) Execute the following query to obtain the ArchiveID  with the previously obtained EngagementID:

    #### Universal DB Query

    Select archivelogid,EngagementStatusID, * from Engagement where engagementid = "Insert EngagementID"     

    select * from engagementstatus
    
    ![image](https://user-images.githubusercontent.com/127347943/224826547-dd88feeb-31ed-4ba1-883a-b54c6e78be6b.png)
    
    Note: Here you can validate that Engagement has the EngagementStatus of 9 that means archive error.

5) 
