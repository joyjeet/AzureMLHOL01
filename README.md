# AzureMLHOL01
Azure Machine Learning Studio Hands on Lab. 
This contains information and steps for learning about how to use Azure Machine Learning Studio.

## Lab Setup
### 1.	Microsoft Azure Portal Login
* Open up your web browser and type in the address: https://portal.azure.com
* Enter your credential: Example “user@domain.com” (if prompted type in your password just like logging onto your laptop).

### 2.	Microsoft Azure Portal
Once you are logged into the Azure Portal you will be within the default “Resource Group” (DataScienceClub_Lab). It is from here that we will begin by adding the necessary resources for creating your own “Machine Learning Studio Workspace” environment to work in for this lab course. If you do not see a screen like the one below choose “Resource Groups” from the left hand navigation bar, you should then see this screen.


![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub2.png)
 

### 3.	Create a Storage Account
* Now we want to create a storage account for your Machine Learning Studio Workspace, from the left hand side navigation bar choose “Storage accounts”:

 ![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub3.png)

* Now choose the “+ Add” to create a new storage account:

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub3_1.png)

* The Storage accounts page is displayed, it is here that we want to only make the following two changes:

  *	Storage account name=enteryourcorpcredential (note in the top right of the portal image below shows the credential of which you are logged in with. In my case it’s “robsau”), now add your own 6 char corp credential all lower case nothing else. 
  *	It’s very Important to note why we want you to use your corp credential to name your resources, because everyone in the lab will be creating resources as well and the easiest way to know which ones are yours is by using your corp credentials. Later in the lab you will see why.
  *	The Account kind=Storage (general purpose v1) – by default it has selected general purpose v2, please change this to v1
  *	Select the “Review + create” button.


 ![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub3_2.png) 


* Azure now performs a quick validation and once it passes you can select the “Create” button if there are no issues.

 ![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub3_4.png) 


* Your deployment is now underway, you may now go back to the “Resource Groups” page. The storage account will show up in the right side window pane once it has been created. Note: you should start seeing many other lab users storage account resources being created as well. This is the first of three resources you will be using for your Machine Learning Studio Workspace.

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub3_5.png)  

### 4.	Create your Machine Learning Studio Workspace
* Choose “+ Add”

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub4.png) 

* Begin typing in “Machine Learning” and then press “enter” a list of resources comes up.
* Choose the  “Machine Learning Studio Workspace” resource listed.

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub4_1.png)  

* On the next screen select the “Create” button

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub4_2.png) 

•	Now we are going to make three changes and select the Web service plan on the next screen.

  A.	Workspace name=enteryourcorpcredential_Workspace (Example: “robsau_Workspace”).
  
  B.	Storage account, first select the “Use Existing” radio button and importantly select the storage account name that you created in step 3 from the drop down list, if you fail to choose your own storage account you may lose where your data is located.
  
  C.	Web service plan=enteryourcorpcredential and leave the _WorkspacePlan in the naming structure (Example: “robsau_WorkspacePlan”).

 ![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub4_3.png)

D.	Select the “Web service plan pricing tier” and a new menu pops up.
E.	Choose the “S1 Standard” plan and click on the “Select” button.

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub4_4.png) 

•	In the next screen select the “Create”.

 ![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub4_5.png)

•	This in turn creates/names the other two resources identified by your corp credentials and you will easily be able to locate these objects from the many other resources in the “DataScienceClub_Lab” Resource Group.
•	Select “Resource Groups” and go back to the DataScienceClub_Lab resource group.

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub4_6.png) 

•	You should now be able to find your three “named” resources similar to below. You will see a growing list of resources and this is where naming them with your credentials helps you to find them.
•	Next you will want to select your resource “yourcorpcredential_Workspace” which opens another screen to allow you to launch the Machine Learning Studio Workspace service that you just created.

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub4_7.png) 

•	Now select “Launch Machine Learning Studio”

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub4_8.png) 

•	Click on “Sign In”

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub4_9.png) 

5.	Upload the lab Dataset into your Machine Learning Studio Workspace
•	Once you landed on the Machine Learning Studio Workspace page select “DATASETS” and then select “+ New”

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub5.png) 

•	On the next page choose “From Local File”

 ![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub5_1.png)

•	Now open up the location to where you saved the course dataset CustomerChurnTrainingSample.csv file and click the checkbox image and upload the file.

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub5_2.png) 

•	You should now see the course dataset file: CustomerChurnTrainingSample.csv
•	This concludes the loading of the dataset into the Machine Learning Studio Lab

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub5_3.png)

### 6. Create Machine Learning Studio Workspace

In Azure portal click on the plus sign to create a new Azure Machine learning workspace.

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub6.png)

Fill in the name and other values then choose a pricing tier then click on create. 

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub6_1.png)

Select Launch machine learning studio

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub6_2.png)

After the workspace is launched, select the new workspace that was created, in this case it is "hollabtest01"

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub6_3.png)

### 7 Create an experiment

Once in the workspace, click new a the bottom left, then click on blank experiment.

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub6_4.png)

The blank experiment will looks like the image belew (left) and after we complete the expercise it will look something very similar to that we have on the the right side. 

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub6_5.png)

First we need to do is to add dataset. For this we will import the data that was uploaded to teh blob earlier. 

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub7_3.png)

While the import data is selected, click on launch wizard, then follow the promt and fill in the required field as shown below.

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub7_4.png)

At this time, you can run the experiment by clicking the run button at the bottom. You can now visualize the data that was loaded by clicking on the node as show in the image below. This will give a quick view of the data that was loaded. 

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub7_5.png)

Add module "Clean Missing Data" that will replace all missing value with "0"

Add module "Remove duplicate rows". Select all columns in the "Launch Column Selector" and check the box "Retain first duplicate row"

Add module "Select Columns in Dataset". In this module we can include or exlude columns that we need for our experiment. For this lab we selected all the columns, then only excluded two columns (year and month).

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub7_6.png)

Add module "Execute Python Script", then add the below code in the module. 

````python
# The script MUST contain a function named azureml_main
# which is the entry point for this module.

import pandas as pd

# The entry point function can contain up to two input arguments:
#   Param<dataframe1>: a pandas.DataFrame
#   Param<dataframe2>: a pandas.DataFrame
def azureml_main(dataframe1 = None, dataframe2 = None):

    print('Input pandas.DataFrame #1:\r\n\r\n{0}'.format(dataframe1))
    
    df= dataframe1

    columns_to_encode = list(df.select_dtypes(include=['category','object']))

    for column_to_encode in columns_to_encode:
        dummies = pd.get_dummies(df[column_to_encode])
        one_hot_col_names = []
        for col_name in list(dummies.columns):
            one_hot_col_names.append(column_to_encode + '_' + col_name)
        dummies.columns = one_hot_col_names
        df = df.drop(column_to_encode, axis=1)
        df = df.join(dummies)
    
    return df,

````

Next, add module "Split Data" to train the module with some of the data and then test it with some of the data. In this case we will split the data in 70% and 30% perent. We will use later set to train then rest to score the model. 

Add module "Train Model" then add the machine learning model that we want to use to train this experiment. add another train model and a machine learning model to compare for the best alorithm. 

![image](https://github.com/joyjeet/AzureMLHOL01/blob/master/images/DataScienceClub7_8.png)
