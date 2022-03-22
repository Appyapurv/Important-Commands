# Important-Commands
Some important commands/querys

**Azure commands--**
1. Az-login 
2. Install-Module -Name Az -AllowClobber  -Scope CurrentUser
3. C:/home/CLI2/wbin/az.cmd login --service-principal -u 'xxxxxx' -p 'xxxxxx' --tenant 'xxxxxx' | Write-Host



**NPM commands--**
1. brew install openss
2. brew install librdkafka
3. brew install openssl
4. brew install zstd
5. brew upgrade openssl
6. brew install glib-openssl
7. npm install
8. npm intall @azure/functions



**SQL Commands--**


select DISTINCT (FileName) from stix.DocumentImages di

select COUNT(*)   from stix.DocumentImages di

Select COUNT(DISTINCT FileName) AS "Number" From stix.DocumentImages di 


select FileName from stix.DocumentImages  where stix.DocumentImages di=(stix.DocumentImages) and column_name like 'a%';


SELECT COUNT(DISTINCT FileName)
FROM stix.DocumentImages
WHERE  FileName LIKE '.%'

SELECT  FileName
FROM stix.DocumentImages
WHERE  FileName LIKE '.'

select PARSENAME(replace(FileName,'.',''),1) as FileName  
from stix.DocumentImages

//filterout column into 2 parts 
select DISTINCT 
     case CHARINDEX('.', FileName) when 0 then FileName
       else SUBSTRING(FileName, CHARINDEX('.', FileName) + 1, LEN(FileName)) end Apurv 
from stix.DocumentImages 


Select COUNT(*)  from stix.DocumentImages di WHERE  di.FileName LIKE '%.jpg'

