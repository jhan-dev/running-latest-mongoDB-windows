# running-latest-mongoDB-windows
## mongo not recognized when mongod is running on another terminal window for Windows users.

MongoDb version-6.01+ For those who are facing any connection errors or bash errors.

Currently, mongo shell is not available in the new version. But if you want to use it, then you can download any mongodb version less than 6 and you will find it there.

## Step 1. 
  You can download it through this link MongoDB Shell.

## Step 2. 
  After downloading it extract the zip and copy the mongosh folder.

## Step 3. 
  Now go inside program-files available in c drive(C:\Program Files)  and paste the copied folder.

## Step 4. 
  Now open the mongosh folder and go inside bin folder then copy the exact path of that bin directory.
  It will be similar to my path i.e. C:\Program Files\mongosh-1.5.4-win32-x64\bin
  (copy this path on a NotePad to use later).
  
## Step 5. 
  Now go back to program files and open MongoDb folder (At this point I hope so you have downloaded the mongodb by following the above video)

## Step 6.
  Now open the bin folder by following the path C:\Program Files\MongoDB\Server\6.0\bin
  (copy this path and paste it into your NotePad as before).


# This is the time to setup enviroment variable


## Step 1. 
  So to setup the enviroment variable click the windows button type env + press enter.

## Step 2. 
  The System Property Dialog Box will apppear. Click on Enviroment Variable.

## Step 3. 
  Enviroment Variable Dialog Box will Appear. There you can see many variable presents inside use Variable for (WindowsUserName).

## Step 4. 
  Select the Path variable and click on the Edit button.

## Step 5. 
  Edit Enviroment Variable Dialog Box will appear (*If not then make sure you have clicked on the 1st edit button).

## Step 6. 
  Paste the paths you have copied into NotePad one by one by clicking on New button.

## Step 7. 
  Once you have pasted both paths, click on Ok for all 3 dialog boxes to confirm changes.
  
  
# Check the connection to the mongo server


## Step 1. 
  Open hyper terminal and type "mongod" or "Mongod" and it will start the server

  *Don't take stress if you see something like this :--

 {"t":{"$date":"2022-08-20T10:12:09.003+05:30"},"s":"I",  "c":"NETWORK"................
This is not any error you can read its doc for more information Log Messages

## Step 2. 
  Now wait until you see something like this...

{"t":{"$date":"2022-08-19T22:29:25.840-07:00"},"s":"I",  "c":"NETWORK",  "id":46887,   "ctx":"listener","msg":"Waiting for connections","attr":{"port":27017,"ssl":"off"}} 


## Step 3. 
  Open new hyper terminal and type "mongosh"

  After sometime you can see something like  test>  or a normal greater bracket >


