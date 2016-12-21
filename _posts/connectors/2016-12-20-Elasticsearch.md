---
layout: connectors-tutorial-single_layout
title: Connect Your Charts and Dashboards to an Elasticsearch Database
subtitle: Graph data from your Elasticsearch database with Plotly 2.0 and the Plotly Database Connector.
permalink: /database-connectors/elasticsearch/
imageurl:  http://cdn.rancher.com/wp-content/uploads/2015/09/14203235/elastic-logo-square.jpg
state: active
tags: other
section: Basics
meta_description: Follow these steps to connect to your Elasticsearch database
popularity: featured
actioncall-url: https://github.com/plotly/electron-sql-connector/releases

steps:
 - title: Download the Plotly Database Connector App
   sub-steps:
    - copy: "Simply [Download](https://plot.ly/database-connectors/) the app to get started!"
 - title: Launch and Connect
   sub-steps:
    - copy: "Once the download is completed, launch the application! If you are on Windows, make sure the application folder is in your C:/Program Files folder. You may have to open the application as administrator. Having launched the app, select *Postgres* by clicking on its icon."
      img: "![](/static/images/database-connectors/select-dialect/elasticsearch.png)"
    - copy: "Enter your username, password, database server name (*host*) and its port number."
    - copy: "Finally, click on the *connect* button!"
    - copy: "Once connection is established, your connection credentials will be saved and greyed out to avoid unintentional changes. If you wish to modify your connection, click on *edit credentials*."
      img: "![](/static/images/database-connectors/connected/elasticsearch.png)"
 - title: Preview Your Indexes and Docs
   sub-steps:
    - copy: "Two dropdown menus will appear. The options are the indexes and documents respectively of the database."
      img: "![](/static/images/database-connectors/preview/elasticsearch.png)"
 - title: Send a Query to Your Database
   sub-steps:
    - copy: "Having connected your app, visit [Plotly Chart Creator](https://plot.ly/create/) and click on *import data* in the top right corner."
      img: "![](/static/images/database-connectors/one-time-query/import-data.png)"
    - copy: "Choose *SQL* from the options on the top."
      img: "![](/static/images/database-connectors/one-time-query/import-sql.png)"
    - copy: "Click *Next*."
      img: "![](/static/images/database-connectors/one-time-query/next.png)"
    - copy: "If you have not setup your connector to use HTTPS protocol, you do not need to modify any of the options. See [HTTPS tutorial](http://help.plot.ly/database-connectors/https) to setup your connector to use the HTTPS protocol. Once done, come back to this point and select the *HTTPS* option."
      img: "![](/static/images/database-connectors/one-time-query/https.png)"
    - copy: "Click on *Connect*"
      img: "![](/static/images/database-connectors/one-time-query/connect.png)"
    - copy: "The modal will close and a new panel will be added to your Plotly Chart Creator."
      img: "![](/static/images/database-connectors/one-time-query/elasticsearch-editor.png)"
    - copy: "On the right, your available connections from the Plotly Database Connector will be displayed. If you have more than one, make sure you select the database connection that you want to use when writing the query."
      img: "![](/static/images/database-connectors/one-time-query/connections.png)"
    - copy: "Also to your right, you will see a dropdown for the database indexes and documents. Once one of each is selected you will be able to view the *Fields* (column names) to help you with your search."
      img: "![](/static/images/database-connectors/one-time-query/elasticsearch-dropdowns.png)"
    - copy: "You can write a search string in the search bar such as *John Smith* which will cause Elasticsearch to only return entries that contain that string somewhere within them.,"
      img: "![](/static/images/database-connectors/one-time-query/elasticsearch-search.png)"
    - copy: "To aggregate your results click on the aggregation-type dorpdown menu. Here we chose *Significant terms* to find most occuring words within the *Response* column and count them. The choice of *counting* them was made by selecting the option *Count* in the *Compute* dropdown menu."
      img: "![](/static/images/database-connectors/one-time-query/elasticsearch-query.png)"
    - copy: "Once your query is finalized, click *Run Query*. If you wish to set your query on a schedule to keep your grid's data updated to the latest entries of your database, visit our [schedule a query tutorial](http://help.plot.ly/database-connectors/schedule-query)."
      img: "![](/static/images/database-connectors/one-time-query/run.png)"
 - title: Making a plot!
   sub-steps:
    - copy: "Let's visualize the most occuring terms in company's response messages in a pie chart. Click on *Graph* on the left side of the window and choose *Pie Chart* as *Chart Type*. Select *Company Response* as the labels and *value Count* as the *values* for the chart."
      img: "![](/static/images/database-connectors/make-graph/elasticsearch-graph-1.png)"
    - copy: "Let's make sure to go back to the graph and make a title to clarify our message."
      img: "![](/static/images/database-connectors/make-graph/elasticsearch-graph-2.png)"
    - copy: "Finally let's not forget to save and share our graph. You can press Control + S to save or click on the *Save* button on the left of the window."
      img: "![](/static/images/database-connectors/make-graph/elasticsearch-share.png)"
    - copy: "You will be prompted to choose your privacy settings for this graph and data. There is nothing here to classify, let's simply set both *plot* and *data* to *public*. Click *SAVE*."
      img: "![](/static/images/database-connectors/make-graph/graph-save-modal.png)"
    - copy: "Let's share this interactive plot with a friend or a coworker (or both)! Click on the *SHARE* tab on the left."
    - copy: "The fastest way is to send the *Shareable Link*, copy and paste it into your favorite e-mail or other communication service. Try out our Twitter, Facebook and Google+ links as well or embed it into your website by obtaining the iframe link in the *Embed* tab. If you set the settings to *public* previously, your friend or coworker will be able to view it even without an account and give you feedback."
      img: "![](/static/images/database-connectors/make-graph/graph-share-modal.png)"

---
