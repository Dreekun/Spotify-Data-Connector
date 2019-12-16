# Spotify-Data-Connector
A Power BI custom data connector for Spotify.
Analyse your streaming data with Power BI visuals.
This is for personal use only.

What you can download:

- The Spotify Data Connector for Power BI
- The Power BI template file
- Documentation files

What is this for:
The Spotify Data Connector for PBI allows you to access to your Streaming History details, such as:
  
 ![navigatorMaisRecente](https://user-images.githubusercontent.com/34665357/70452197-9f6b8480-1a9e-11ea-91c9-ff2709634ec9.png)
 
Here is a quick tutorial on how to set this up for you (a more detailed tutorial can be found in Installation.pdf above):

## Step 1: Creating your own Spotify Application
To be able to use this connector, you have to authenticate to https://developer.spotify.com/dashboard/ and create your own application. This will generate you a **client_id** and a **client_secret**. Next, on the dashboard page, under Edit Settings, you need to enter the following redirect_uris:

![redirect_uri](https://user-images.githubusercontent.com/34665357/70648011-1c832f00-1c42-11ea-96cc-017bd348b1ad.png)

## Step 2: Change some Power BI settings
You need to Start Power BI Desktop, go to Settings:
- Select **Security**, and under **Data Extensions**, check **Allow any extension to load without validation or warning**
- Select **Privacy** and under **Privacy Levels**, check **Always ignore Privacy Level settings**

## Step 3: Download the connector and Modify the Credentials.json file
Now you can open and extract the Spotify_Connector.mez file with winrar, edit the Credentials.json inputting your credentials, and assemble the files again into Spotify_Conector.mez.

## Step 4: Copy the Spotify_Connector.mez into Custom Connectors folder
Create a new folder under C:\Users\username\Documents\Power BI Desktop\Custom Connectors and paste the connector.mez file.

## Step 5: Get the Power BI Template for this connector
This is a very simple report with a built-in Data Model, with all queries available set up, a few measures, and a report to give a first view of you can analyse here.
![report I](https://user-images.githubusercontent.com/34665357/70461416-823fb180-1ab0-11ea-95a1-b63586c5a4fb.png)
![report II](https://user-images.githubusercontent.com/34665357/70930684-ac9fea80-202d-11ea-915e-5d2e7f8d8984.png)


## Step 6: Read the Documentation
In order for this connector to be useful, there are a few workarounds and solutions to common problems you may face in the documents provided above. Please read it, and feel free to contact me in case you need any help.
