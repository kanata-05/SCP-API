# SCP API
Access information on SCPs through python and javascript! (note: currently being developed, isn't completely released)  
Currently limited from SCP-001 to SCP-5723, Some field may be broken (or just not exist) and may not have properly been copied (I apologize for that, I am constantly working on it.)  
Install using `pip install scpfetch`! (the name is scpfetch because pypi didn't like scp-api being close to a already existing package nc-scp-api)  
Import using `import scpfetch`  
https://pypi.org/project/scpfetch/0.1.1/

# How it works
We first scrapes (Reason why some field might've not been properly copied) the information off from the [SCP wikidot](https://scp-wiki.wikidot.com/) and stores it in a JSON format.  
We then upload the information up to our site, where the API pulls the data from, inorder to avoid putting load on the [SCP wikidot](https://scp-wiki.wikidot.com/)  

## Process
Create Scraper and get the information (Complete)  
Create the site and upload the files (Complete)  
Create the API (Testing)

### Documentation
  Functions that are currently available:  
    `get_info(scp, field, num)`  
    Where `scp` is the SCP number  
    `field` is one of the field you can access, [click here for the available field](#fields)  
    `num` is the list object number (of `field`) if the field is not a list, it will be ignored.

### Fields
  Fields that can be accessed:  
    `"URL"`: URL from where it was scraped  
    `"all_text"`: Complete text from the page  
    `"addendums"`: All addendums on the SCP  
    `"documents"`: All documents on the SCP  
    `"notes"`: Most of the time, it's about licensing stuff and who made it  
    `"containment_procedures"`: Containment Procedures for the SCP  
    `"description"`: Description of the SCP  
    `"title"`: Title of the tab
