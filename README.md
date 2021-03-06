# Automatically Apply to Jobs Web Crawler

Application for Automatically Applying to jobs using a Web Crawler (i.e. using Selenium API). This is a simple .Net Console application for demonstrative purposes only. 

# What You Will Need

1. Suggested Operating Systems: Windows 7 or 10
2. (Required) Microsoft SQL-Server Database (Express edition is free)
3. (Required) API Key from https://www.indeed.com/publisher (Free to signup and use)
4. (Optional) Visual Studio (VS 2017 Community is Free)

# Getting Started

1. Create a Sql Server Database either locally or in a cloud of your choosing which is a bit easier (e.g. AWS RDS, Azure, etc.)
2. Open and Run the SQL commands as defined in file "Create Database.sql"
3. Open Configuration file found in "AutoApply/config.json" and alter the following json object properties:
	* "sql": Connection String to your SQL Server CrossMyLoss Database
	* "indeed-api": Publisher API key as received from https://www.indeed.com/publisher (requires signup)
	* "locations": Array
		* "country-code": [Full List Available Country Codes](https://github.com/hadjimylos/AutoApplyWebCrawler/blob/master/All%20Country%20Codes.txt "Available values")
		* "city": Enter a location (e.g. New York) or leave as an empty string apply everywhere
	* "terms": Array of search words to apply to (e.g. Software Developer, Accounting, Salesman, etc.)
	* "user": Object that stores all of your information, used for creating and sending the application
		* "email": Your Email (required)
		* "full-name": Your Full Name (required)
		* "phone-num": Your Phone Number (required)
		* "resume-path": C:\\\\FullPath\\\\To\\\\SampleResume.pdf (required)
		* "supporting-file1": C:\\\\FullPath\\\\To\\\\SomeFile.pdf (optional)
		* "supporting-file2": C:\\\\FullPath\\\\To\\\\SomeFile.pdf (optional)
		* "supporting-file3": C:\\\\FullPath\\\\To\\\\SomeFile.pdf (optional)
		* "supporting-file4": C:\\\\FullPath\\\\To\\\\SomeFile.pdf (optional)
		* "supporting-file5": C:\\\\FullPath\\\\To\\\\SomeFile.pdf (optional)
		* "cover-letter": C:\\\\FullPath\\\\To\\\\CoverLetter.txt


>**Please Note**: 
>
>In JSON, file paths should use 2 backslashes, not 1. 
>
>Therefore 
>
>>* C:\\FullPath\\To\\CoverLetter.txt
>
>Should be entered as:
>
>>* C:\\\\FullPath\\\\To\\\\CoverLetter.txt
>
>To the "cover-letter" property of the config.json file. 

# Getting Finished

Run the application by doing any of the following:

1. Open the solution in Visual Studio (.sln file) and hit f5/run
2. Navigate to and double click "AutoApply/bin/Debug/AutoApply.exe"
3. Navigate to and double click "AutoApply/bin/Release/AutoApply.exe"

If you have any questions or require assistance, please feel free to 

get in touch. My email is chris.hadjimylos@bitbytebuffer.com

**Enjoy** :) !!
