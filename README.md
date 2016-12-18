# Jobhun.com API

This document is here for Jobhun.com API users.  The document will cover list of API available, and data schema for all of API requests and responses.

##Before we begin.

Jobhun.com uses data management platform SEVENTH. You will need to register and obtain API token from SEVNETH.  Anyone with valid email address can register and use this API for free.  You can registere at here, [SEVENTH](http://7thdata.com/en-US/dev/).  

#The Simple Version

##Jobs
If you want to search for jobs.
```
GET: https://api.7thdata.com/JHN001/[Your Token]/Jobs/List/?culture=en-US&keywrods=engineer
```

If you want to get details of specific job.
```
GET: https://api.7thdata.com/JHN001/[Your Token]/Job/Get/?culture=en-US&jid=[Job ID]
```

##Companies
If you want to search for companies.
```
GET: https://api.7thdata.com/JHN001/[Your Token]/Companies/List/?culture=en-US&keywrods=engineer
```

If you want to get details of specific company.
```
GET: https://api.7thdata.com/JHN001/[Your Token]/Company/Get/?culture=en-US&jid=[Job ID]
```

#Job Seekers, Employers, and Developers

Jobhun.com is data management platform for job seekers, employers, and developers who are looking to create services with data at Jobhun.com. 

## Search For Jobs
End Point | Description
----------| -----------
/Jobs/List/ | Get list of Jobs
/Jobs/ListSaved/ | Get list of Jobs from saved list
/Job/Get/ | Get Specific Job

## Manage Jobs
End Point | Description
----------| -----------
/Jobs/MyJobs/ | Get list of editable Jobs
/Job/Upsert/ | Upsert specific job
/Job/Delete/ | Delete specific job
/Job/Analytics/ | Get analytic data of specific job

## Search For Companies
End Point | Description
----------| -----------
/Companies/List/ | Get list of Companies
/Companies/ListSaved/ | Get list of Companies from saved list
/Company/Get/ | Get Specific Company

## Manage Comapnies
End Point | Description
----------| -----------
/Companies/MyCompanies/ | Get list of editable Companies
/Company/Upsert/ | Upsert specific company
/Company/Delete/ | Delete specific company
/Company/Analytics/ | Get analytic data of specific company
