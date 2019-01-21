## Welcome to data/\bridge engine Help Page

# Installation
## Qlik Deplyoment Framework (QDF)

The data/\bridge engine (db-e) is based on the Qlik Deployment Framework.
Please download and install it using the following link.

https://github.com/databridge-engine/Qlik-Deployment-Framework

To assure that that db-e is working with QDF following prerequisites are required:
1. Name QDF Container Folder e.g. 03.CRM, 04.SAP, 05.CallCenter
2. Folder Connection setup in Qlik Management Console (QMC) need to have the same Name which are pointing to these QDF-Contaners
3. ETL Apps linked to the QDF Container need the same naming convention:
```markdown  
    Container: 03.CRM:
      03.CRM-10.Extract
      03.CRM-11.Delta Transform
      03.CRM-20.Transform
      03.CRM-30.DataModel
```
## data/\bridge engine (db-e) installation

The db-e sctips (extract, transform, datamart, etc) have to store in the subfolder of each QDF Container: \3.Include\3.Custom

### Server name Info

On each Qlik Server a "Server info" file has to be stored.
This helps to identify the server where your are on, especially in a multi-node environment.
```markdown  
- ServerInfo.txt to be stored in the QDF Root directory containing your Server Name
```

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/databridge-engine/help/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
