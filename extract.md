[db-e help home](/index.md)

# Operation manual

## Extract

The extract entry list is the main table where are all your extract definition are maintained. All other processes like transform, delta merge are referencing to this list. Only talbe which active (Status = 1) are beeing processed.


### Extract entry list (required)

| Status | Connection | DatabaseType | Database | DatabaseSchema | TableSQL | TableSave | TableSaveLocation | PrimaryKey | PrimaryKeyName | FullLoad | NoRecords |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 = Active 0 = Inactive | Name of the Connection in QMC | MSSql ODBC XLS SAP SAPBW Oracle | Database Name | Table name in the database | Database schema e.g. MSSql = .dbo | Name of the QVD table to be saved | Folder Name where to QVD should be saved | definition of the primary key* | Name of the Primary Key** | 1 = Full Load 0 = Delta Load | No. of records to be loaded. Set to 999999999999 of all shall be loaded | 


- *Qlik script syntax have to be used
- **Recommended naming convention e.g. %Account_Key

### Extract entry list (optional)

| Filter | DeltaDateField | DeltaKey | DeltaType | 
| --- | --- | --- | --- | 
| filter criteria e.g. where Year=2017  | Date field to be used for delta load e.d. modified_date | Primary Key of the table | 2 = SCD Type 2, 1 = SCD Type 1** |


- *database script syntax have to be used
- **SCD Type 1 = .... SCD Type 2 = ......

### Extract entry list (information only)

| TableInfo | TableNoRowsFull | TableLoadingTime_Full |
| --- | --- | --- | 
| Descriptive information about the table  | Number of total rows of the table | Duration for a full load |



