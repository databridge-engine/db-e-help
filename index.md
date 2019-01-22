## Welcome to data/\bridge engine Help Page

# Installation
## Qlik Deplyoment Framework (QDF)

The data/\bridge engine (db-e) is based on the **Qlik Deployment Framework**.
Please download and install it using the following link.

[github Qlik Deployment Framework QDF](https://github.com/databridge-engine/Qlik-Deployment-Framework)

To assure that that db-e is working with QDF following prerequisites are required:
```markdown
1. Name QDF Container Folder e.g. 03.CRM, 04.SAP, 05.CallCenter
2. Folder Connection setup in Qlik Management Console (QMC) need to have the **same Name** which are pointing to these QDF-Containers
3. ETL Apps linked to the QDF Container need the **same naming convention**:
  
    Container: 03.CRM:
      03.CRM-10.Extract
      03.CRM-11.Delta merge
      03.CRM-20.Transform
      03.CRM-30.DataModel
```
## data/\bridge engine (db-e) installation
```markdown  
- The db-e sctips (extract, transform, datamart, etc) have to be stored in the subfolder of **share** QDF Container: **\3.Include\3.Custom**
- The custom pre- and post-scripts have to be stored in each individual QDF Container under **\3.Include\3.Custom**
```
### Server name Info

On each Qlik Server a "Server info" file has to be stored.
This helps to identify the server where your are on, especially in a multi-node environment.
```markdown  
- ServerInfo.txt to be stored in the QDF Root directory containing your Server Name
```

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
