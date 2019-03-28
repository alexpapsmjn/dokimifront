# Exercise 2: Javascript Skills

## Intro

We have provided you with a very basic (and ugly) site that consists of 2 pages.  Each page links to the other and also links away from the "site".  We want you to assume that the user lands on index.html by clicking on a Google Ad.  This ad adds URL parameters to the page url, so that we are able to track the performance of the ad.  The URL parameters it adds are the following:

> **?utm_source=google&utm_medium=search&utm_campaign=summer19**

A problem that arises is when a user navigates to another page within the site, these URL parameters are lost.  We would like you to write some Javascript that passes the URL parameters across the user's journey on the site when they click on **internal** links.  In the case of external links, we MUST NOT include these parameters.

We also use a service called Branch.io for being able to track mobile app installs.  Branch provides us with a Javascript SDK that can give us some information regarding the current user, such as if they have already installed our app.  We would like you to integrate the Branch.io Javascript API (use the API key we sent you in the email for the assignment), and to display on the website whether the user uses the app.  Instructions for the Branch API are here: [BRANCH DOCS](https://docs.branch.io/web/integrate/)


## Deliverables & Tips
- include a script that passes URL parameters to internal links but not external ones
- integrate the Branch.io SDK in index.html
- populate the field "IS USING APP" with the reply from Branch.io (*has_app* key)

- ** When you load index.html, include the URL parameters at the end of the URL ex. http://127.0.0.1/index.html?utm_source=google&utm_medium=search&utm_campaign=summer19**
- your script can be vanilla JS or jQuery