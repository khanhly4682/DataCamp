# 1. Importing non-flat files from the web

* import pandas as pd
url = 'http://s3.amazonaws.com/assets.datacamp.com/course/importing_data_into_r/latitude.xls'
xls = pd.read_excel(url,sheet_name=None)
print(xls.keys()) #Print the sheetnames to the shell
print(xls['1700'])##Print the head of the first sheet (using its name, NOT its index)
