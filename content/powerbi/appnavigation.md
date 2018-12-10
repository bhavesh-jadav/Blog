---
title: "Better App Navigation in Power BI"
date: 2018-12-10
draft: false
categories: 
    - "Power BI"
tags: 
    - "Power BI"
    - "Power BI Apps"
---

Power BI Apps are great way to share the content such as dashboards and reports to large Audience. But the way to categorize your content in App is very limited. Once you setup your App without specifying any landing page, you are greeted with following screen.

<figure>
  <img class = "center" src = "/images/appnavigation/default_app_navigation.png" alt = "Default App navigation" style="height: 250px; width:600px"></img>
  <figcaption class = "center" style = "margin-top: 5px; text-align: center;">Default App navigation in Power BI</figcaption>
</figure>


Power BI Apps are categorized into 3 sections, Dashboards, Reports and Datasets. Dashboards and Reports are primary focus for most of the end users. Now if you want to categorize your Dashboards and Reports further down with your own categories, you won't be able to do that because Power BI does not support that yet. But there is way for you to provided good looking and well categorized App to end users.  

When you publish an App, you have option to select landing page as shown below. We can use this feature to create better navigation for your App.

<figure>
  <img class = "center" src = "/images/appnavigation/app_landing_page_selection.png" alt = "App landing page selection" style="height: 250px; width:500px"></img>
  <figcaption class = "center" style = "margin-top: 5px; text-align: center;">Select the content that end users will see when the App is opened</figcaption>
</figure>

Create one report with only dummy data loaded and create your navigation layout in that report. Then we can use this report as a landing page of the App. So whenever end users opens the App, they will see this report which will include custom built navigation. Below is the screenshot of one of the example of how navigation can look like but it is definitely based on your preferences.

<figure>
  <img class = "center" src = "/images/appnavigation/custom_app_navigation.png" alt = "Custom App navigation" style="height: 380px; width:700px"></img>
  <figcaption class = "center" style = "margin-top: 5px; text-align: center;">One of the example of how navigation can look like</figcaption>
</figure>

On left side you see different categories in which I want to categorized my report and dashboards. When you click on say for example Category 2, it will show you "Cards" which links to reports and dashboards which are part of Category 2. 

To make this simple, I have made a custom visual (External Link Card in above screenshot) which is useful to create link to the dashboard and reports with ease. How it works is that you add link of report or dashboard from browser to this custom visual. When user click this custom visual, it will open that report or dashboard in new tab. The custom visual is called **External Link** and it has following settings to modify look and feel.

* **General settings**: Modify border colour, border hover colour etc.
* **Image settings**: Show image or GIF. For example you can show screen shot of report or dashboard. If you have image stored in dataset, drop that field in Image Link in fields pane, enable Link Image Settings and remove the link from the text box in Link Image Settings. This way, it will take URL from the field that you dropped in Image Link.
* **Title settings**: Adding actual link to report or dashboard, title of the link etc.
* **Content settings**: Adding short description about dashboard or report
* **Link Bottom (footer)**: Add some text such as Go to report, Go to Dashboard etc.

<figure>
  <img class = "center" src = "/images/appnavigation/different_parts_of_External_Link.png" alt = "Different parts of External Link custom visual" style="height: 280px; width:400px"></img>
  <figcaption class = "center" style = "margin-top: 5px; text-align: center;">Different parts of External Link custom visual</figcaption>
</figure>

First you finalize look and feel of the External Link card after playing with different settings, then You can go to URL bar of the browser and get the link of the report or dashboard and add it to External Link in Link Title settings and you are good to go.

**Some of the advantages of using this approach are:**

* Clean look and feel of the content navigation.
* Customize look and feel based on your organization standards.
* You can add link for reports and dashboards from other workspaces as well but end user will see it all coming from one place.

**Download Links And Other Resources**  

* Download External Link custom visual [from here](https://github.com/bhavesh-jadav/External-Link/tree/master/dist) (check and download the latest version)
* [Click here](https://app.powerbi.com/view?r=eyJrIjoiMTRjZWM5MjgtZjI3My00NzI4LTkxYzAtOTQ2MDY1ZjE0ZjVkIiwidCI6IjIyMDBiNjQ3LTdmM2EtNGMxYS04ZTkzLTRhYjBiZjRhYWU1OSIsImMiOjN9) to see sample report online (browse through different pages of sample report for more configurations)
* Download sample report [from here](https://github.com/bhavesh-jadav/External-Link/blob/master/Power%20BI%20App%20Navigation%20Sample%20Report.pbix?raw=true)
* Source code: [https://github.com/bhavesh-jadav/External-Link](https://github.com/bhavesh-jadav/External-Link)

Leave a comment below for any feedback or suggestions.