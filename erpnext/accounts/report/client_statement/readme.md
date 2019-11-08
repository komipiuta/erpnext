# Erpnext Client Statement

Erpnext Script Report to generate a Client Statement
The code used is initially derived from the General Ledger Script Report, but may deviate in future.

**CONSIDER THIS CODE AS BUGGY AND NOT SUITABLE FOR PRODUCTION USE.**


### Installation

**Read notes below before embarking on an installation.

The recommended way to install this is using git.

- Enable developer mode for your site
- Log in as an administrator
- Navigate to the "New Report" menu.
- Create a new scipt report
- Pull the branch. You can do this by
   - adding this repository as a remote repository, 
```
git remote add myfork https://github.com/pradeshc/erpnext.git
git fetch myfork
git checkout client_statement
# ...or...
git  merge client_statement
```
      or
   -  fetching the branch directly from the repository using the URL (see url in references)
- Merge into your current development branch


# Notes

- Beware the customer ageing report. It is potentially buggy
- The customer selection in the dropdown must be converted to a single company selection
- Need to find a way to export the ageing report to the Excel export
- The code in installed inside an exiting module
   erpnext/accounts/report/client_statement
  You may not be comfortable with messing with this
 

###References

https://mirrors.edge.kernel.org/pub/software/scm/git/docs/git-fetch.html
https://stackoverflow.com/questions/6368987/how-do-i-fetch-only-one-branch-of-a-remote-git-repository/26270966

###End