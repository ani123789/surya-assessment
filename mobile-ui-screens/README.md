# UI-Dashboards

The goal of this problem is to create a mobile application that displays information to the user.

You can build your mobile application with any technology of your choice. You are also free to use any framework/libraries of your choice for your platform of choice. You are also free to build the layouts of this mobile application in a web technology of your choice.

Please include documentation (in a file called `SETUP.md`) on any prerequisites we would need to have installed to run your application.

We have created a Figma design for the app you need to create, that shows you step-wise layouts.

> [!WARNING]
> For every step, the design is a requirement and must be created as-is.

The [designs can be seen here](https://www.figma.com/design/qlX9bngOXoPGdZm6vfF4CM/Interview-Designs--Mobile-?node-id=0-1&p=f&t=b0fyLnopnZLzHuAq-0). The icons you will need [can be accessed here](https://drive.google.com/drive/folders/1XNsmc8kPt9Mash5ycsjQVrFK-qQXCq1K?usp=sharing).

Please go step by step when creating each of these designs since each step is designed to be tougher than the next. Chances are high that you may not be able to complete all the steps due to time constraints.

> [!WARNING]
> After each step, you need to check in your code on Github. Checking in all steps in the code at the very end fails sometimes.

Note that the data of the UI is going to be populated either with hard coded data, or by calling an API. Each step lays out instructions for how to fetch the data.

## Step 1: Cards 1

For the first step, please build the UI seen [here](https://www.figma.com/design/qlX9bngOXoPGdZm6vfF4CM/Interview-Designs--Mobile-?node-id=2003-1355&t=b0fyLnopnZLzHuAq-4). Note, again, that the designs have to be built exactly as seen in the linked Figma design.

The data should be populated using this hard-coded text:

```
title: "Total Orders",
value: 862,
timestamp: 1754476592000


title: "Ordered Items This Week",
value: 156,
timestamp: 1754641532000


title: "Return Orders",
value: 12,
timestamp: 1754562992000


title: "Fulfilled Orders This Week",
value: 124,
timestamp: 1754627132000
```

## Step 2: Create a Sidebar (aka a Menu Bar) and Scaffolding for Cards 2

In this step you need to create a sidebar and link two screens to it. The design is seen [here](https://www.figma.com/design/qlX9bngOXoPGdZm6vfF4CM/Interview-Designs--Mobile-?node-id=2003-1433&t=b0fyLnopnZLzHuAq-4). The first screen is called "Cards 1", the second is called "Cards 2". Cards 1 should be the screen created in Step 1 and Cards 2 can be left empty for now (you will implement it in the next step).

## Step 3: Create Cards 2

For the third step, please build the UI seen [here](https://www.figma.com/design/qlX9bngOXoPGdZm6vfF4CM/Interview-Designs--Mobile-?node-id=2003-781&t=b0fyLnopnZLzHuAq-4). Note, again, that the designs have to be built exactly as seen in the linked Figma design.

As part of this step, please also add an entry into the sidebar for this step as shown in the design.

TThe data to populate the UI seen in Cards 2 (including the images for a card) should be fetched from [this API](http://interview.surya-digital.in/get-products). Note that the product data (name, price, total number of items) you see in the response can vary from the product data seen in the Figma designs.

## Step 4: Charts

For the fourth step, we would like for you to create a screen that shows charts. The designs for these charts can be seen [here](https://www.figma.com/design/qlX9bngOXoPGdZm6vfF4CM/Interview-Designs--Mobile-?node-id=2003-524&t=b0fyLnopnZLzHuAq-4). Please note that the charts have a certain amount of interactivity. When the taps on the bars of the bar chart or the segments of the pie chart, they are able to see details about those segments of the charts. Make sure you implement these interactions when you build the charts.

As part of this step, please also add an entry into the sidebar for this step as shown in the design.

Please use the following text data to create the bar chart (the chart with title "Sale By Device"):

```
date 01-01-2025  
Mobile 80  
Desktop: 100  

date 01-02-2025  
Mobile 70  
Desktop: 90  

date 01-03-2025  
Mobile 60  
Desktop: 70  

date 01-04-2025  
Mobile 85  
Desktop: 95  

date 01-05-2025  
Mobile 80  
Desktop: 100
```

Similarly, please use the following text data to create the pie chart (the chart with title "Revenue Contribution"):

```
date:- 01-01-2025  
revenue:- 18000  

date:- 01-02-2025  
revenue:- 28000  

date:- 01-03-2025  
revenue:- 12000  

date:- 01-04-2025  
revenue:- 22000  

date:- 01-05-2025  
revenue:- 20000  
```

## Step 5: Table & Photo Attachment

For the fifth step, please build the UI seen [here](https://www.figma.com/design/qlX9bngOXoPGdZm6vfF4CM/Interview-Designs--Mobile-?node-id=2003-77&t=b0fyLnopnZLzHuAq-4). The data should be populated by calling [this API](http://interview.surya-digital.in/get-people-list).

Please ensure that you handle the loading and error states seen in the designs while fetching the results from the API.

Note that the API returns location field's data with the comma character escaped. For example, `Jaipur, India` is written as `Jaipur\, India`.

As part of this step, please also add an entry into the sidebar for this step as shown in the design.

Lastly, as part of this step, the user should be able to attach a photo against an item's detail view in the API response. Note that the photo chosen by the user needs to come from the user's camera or photo gallery. Once a photo is attached against one item of an API response, it should continue to be located on that item's detail view. That is, once a user attaches a photo for an item, goes back to view the item list in the response, and opens the same item's detail view again, the screen should show the user the photo that was previously attached.

## Step 6: Re-Create the Server

For the sixth step, please recreate the server that you have used throughout the preceding steps and implement all of the APIs that you have consumed so far. The API endpoints, parameter behaviors, and responses should be familiar to you by now given that you have used them in the preceding steps.

While implementing the server, make sure that you handle common errors such as incorrect parameters being passed.

In order to complete this step, you will need to point the frontend you have developed so far to the server that you are creating as part of this step.

As usual, feel free to use any technology that you would like to implement this server.
