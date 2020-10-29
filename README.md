# Spotify-Data-Connector
A Power BI custom data connector for Spotify.
Analyse your streaming data with Power BI visuals.
This is for personal use only.

What you can download:

- Spotify Data Connector for Power BI
- Power BI template file
- Documentation files

What is this for:
The Spotify Data Connector for PBI allows you to access to your Streaming History details, such as:

![navigator_recente](https://user-images.githubusercontent.com/34665357/97598759-331fa980-19ff-11eb-8514-12ade2c94b98.PNG)


Here is a quick tutorial on how to set this up for you (a more detailed tutorial can be found in Installation.pdf above):

## Step 1: Creating your own Spotify Application
To be able to use this connector, you have to authenticate to https://developer.spotify.com/dashboard/ and create your own application. This will generate you a **client_id** and a **client_secret**. Next, on the dashboard page, under Edit Settings, you need to enter the following redirect_uris:

- https://oauth.powerbi.com/views/oauthredirect.html
- https://preview.oauth.powerbi.com/views/oauthredirect.html

It should be like this:

![redirect_uri](https://user-images.githubusercontent.com/34665357/70648011-1c832f00-1c42-11ea-96cc-017bd348b1ad.png)

## Step 2: Download the connector and Modify the Credentials.json file
Now you can open the Spotify_Connector.mez file and extract its content. Edit the Credentials.json with a text editor and input your credentials - **client_id, client_secret, and (spotify) user_id**.
Next, assemble the files again into Spotify_Conector.mez. Be careful not to accidentally add subfolders to this file. Keep it as it was before.

## Step 3: Copy the Spotify_Connector.mez into Custom Connectors folder
Create a new folder under C:\Users\<username>\Documents\Power BI Desktop\Custom Connectors and paste the **Spotify_Connector.mez** file. You can now use it in Power BI to see your data.

## Step 4: Change some Power BI settings
You need to Start Power BI Desktop, go to Settings:
- Select **Security**, and under **Data Extensions**, check **Allow any extension to load without validation or warning**
- Select **Privacy** and under **Privacy Levels**, check **Always ignore Privacy Level settings**

## Step 5: Get the Power BI Template for this connector
This is a very simple report with a built-in Data Model, with all queries available set up, a few measures, and two reports to give a first view of you can analyse here.
It also has some code for you to be able to dynamically write the records to a SQL database. More details on this process on the documentation files.

Example 1: Listening history.
![listening_history_1](https://user-images.githubusercontent.com/34665357/97619127-bd740780-1a17-11eb-93ca-20f6a4b661e8.PNG)

Example 2: Album history
![report II](https://user-images.githubusercontent.com/34665357/70930684-ac9fea80-202d-11ea-915e-5d2e7f8d8984.png)

## Step 6: Go get some historic data
One pretty cool thing that spotify provides for its users is 2 years of historic data. All you have to do is go to your profile and ask for it. More details about it can be found on this blogpost: https://www.linkedin.com/pulse/working-json-data-power-bi-spotify-example-zach-renwick/
It takes a few days for the data to be sent. When it does, you'll want to import it to a database. More details about this can be found on the documentation. 

## Step 7: Setup a SQL database to store your data when you refresh the dataset
If you want to keep track of the records that you hear by the years, the 50 most recently played songs that spotify api provides aren't enough. So you might be interested in storing the records in a database, as long as you refresh. Details about this process are explained in the documentation.

## Step 8: Read the Documentation
The documentation provided walks you through the processes in more detail. Be sure to check it out if this interests you.
