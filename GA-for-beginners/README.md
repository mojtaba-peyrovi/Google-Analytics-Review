### Google Analytics for Beginners
---

__Purchase Funnel__: Purchase funnel has 3 steps:

1) Acquisition: building awareness and acquiring user interest.
2) Behavior:  When the user engages in your business.
3) Conversion: When a user converts to a customer and makes transactions with the business. 

In offline world, it's hard to measure this process, but in online business we can measure so many aspects of it, using digital analytics tools.

For example, an online shop, can track all marketing advertising campaigns, and measure each one's performance, to see which one was the most effective, and expand those efforts.  For example, the store can analyze geographical data and figure out poeple at some geographical area, buy more of the products, so they could invest more on marketing campaigns in those areas.

Another example, is to use analytics data to understand how users progress through their online shopping cart. If they notice that the users have trouble with a particular step on their website, they can improve it. 

Google Analytics can collect data from the website, mobile app, online point-of-sales systems, video game consoles, CCRM systems, or any internet connected platform. 

__Session:__ A session starts when a user navigates to a page that includes the GA tracking js snippet and the session ends after 30 minutes of inactivity. If the user returns after 30 mins, a new session will begin. 

The GA javascript code, collects data, from the page sessions into the GA system in order to make reports. 

When setting up your GA configuration, don't exclude any data you think you might want to analyze later. 

#### Setting up GA account:

here is the hierarchy of objects:

1) Organization
2) Account
3) Property
4) View

Each organization can have multiple accounts, each account multiple properties, and each property multiple views.

(photo: GA-hierarchy.jpg)

Typically you will create separate GA account for distinct businesses or business units.

Each GA account has at least one property.

Each property can collect data independently of each other using a unique tracking ID.

You can have multiple properties to each account so that you can collect data from different websites, or devices associated with the business. 

Each view can have a filer included, to determine which exactly has to be collected.

(photo: ga_hierarchy_with_filters)

For example a multinational company can have multiple views, for each region. also another view for external traffic(filtering out the company employees out.)

In view level, we can also set __GA goals__. 

##### What are Goals?

A Goal is valuable tool, to track conversions, or business objectives from the website. Some example of goals
:  How many visitors signed up for the newsletter, or how many users purchased a product.

#### IMPORTANT:
You can't change the settings for accounts, properties, and views later.

- Views only collect data from the day they are created and onwards. If the view is deleted, only the administrator can return it back within a limited amount of time. 
- we can set permissions to users, at account, property or view level.
- Each level, inherits the permissions from the layer above it.

(photo: user-permission-options.jpg)

When we setup a property, GA automatically makes a view, that has all raw data, and it is called "All Web Site Data." It is recommencded to be renamed to "Raw Data", so that we don't forget the data hasn't been filtered.

We can make a view easily by clicking on the drop down as we see at (create_view_1.jpg) we called it test view. 

Now we see it is added (create_view_2.jpg), then we click on "view settings"

What is important in the new window (create_view_3.JPG), is to click on the radio btn with this title :`Exclude all hits from known bots and spiders.`

Now it is time to make a master view that has all the data we need from the website. For doing this, we can easily copy the test view and call it Master view. 

For each step, we better implement the changes on test view, before doing it for the master view. Under test view, we click on "filters."

When we click on "Create a filter", we see two types on filters (custom_vs_predefined_filters.JPG) 

Predefined filters are the most commonly used filters already made, and custom ones are the ones we can design ourselves of specific scenarios. One of the predefined filters, is excluding data from a specific IP address.

Once we applied this filter to the test view, we can also add it to the master view. 

#### Leftside Bar:

__Customization:__ Where we can make custom reports for specific business needs. (will discuss later in the advanced course.)

__Reports:__ Under reports there are different options. 

- __Real Time:__ shows live user behavior, who is online, where are they coming from if they are converting.

- __Audience:__ Shows the characteristics of the audience, like gender, age, country the user comes from, how engaged they are, whether or not they are returning users, etc.

- __Acquisition:__ It shows which channel (advertising, or marketing campaign) brought users to the site. The sources can be organic, CPC(paid search), Referral (traffic coming from the other website), social (coming from social media), or other low traffic sources.

- __Behavior:__ Shows how people are engaged to the website, including which page they viewed, their landing and exiting pages. __IMPORTANT: WITH SOME EXTRA CONFIGURATION, YOU CAN TRACK WHAT USERS SEARCHED FOR, ON THE WEBSITE OR WHAT ELEMENTS THEY INTERACTED WITH.

- __Conversions:__ It allows us to track website goals based on the business objectives.


#### Reports:

There are tow types of reports:

__1)__ Overview Reports: Overview reports provide a high level summary of metrics in one place.

The audience overview report shows aggregate audience metrics like number of users, page they visited in a session, average session durationm and bounce rate. (photo: audience_overview_report.jpg)

On the top of the overview report, we can add a segment. 

##### What is segment? 

A segment is like a filter that you can apply to look at specific data and compare metrics. The default segment, is all users that visited the website in the chosen time period.

We can also add other metrics to the chart to compare them. (photo: overview_report_two_metrics.jpg)

Also, right under the line graph we can add annotator(notes) to the graph: (photo:overview_report_graph_annotator.jpg)

__User:__ an individual who had at least one session on the website.

__Pageviews:__ The number of times the page containing GA code has been displayed to the users.

__page/session:__ Average number of pages being seen during each session.

__Bounce Rate:__ percentage of users who left after viewing a single page on the website and taking no additional action.


 __2)__ Full Reports: on the right bottom of the overview report, there is a link to the full report. when we click on the link, we see something like this: default_full_report.jpg
 
 It has added the yellow highlighted features. __Site usage__ on the top, shows behavior metrics. 
 
 __Goal set 1__ on the top show metrics based on the number of goals we have configured and they only show up if we already setup goals at GA. Finally, __Ecommerce__ shows all the metrics related to transactions on the website.

We can also add second dimension to the full report as we see at full_report_second_dimension.jpg

##### How to save or share the reports?
 
There is a save button on the top of the reports that we can use to build a link to the report under __Custom Reports__ on the left sidebar.

Also, there is an export button, and share button next to the save button. Export button exports the data as xlsx or csv. Share button lets you email a copy of the report as an attachment, or schedule regular email updates.


##### Making dashboards:

Under customization (left sidebar) we can click on dashboards, and we can create a new dashboard. Like Tableau, or any other BI tool we can customize the dashboard and add the reports we need.

We can share the analytics, inside a gallery called "Solutions Gallery" where all other users will be able to access it.    
    


### Basic Reporting:

1) Audience report: It gives us information about the users of the website. information such as what country they are from, what languages they speak, the technology they use, etc.
    
- __Active Users Report:__ shows how many users had at least one session on the website, we can change the filter to last day, last 7 days, last month, etc.
(photo: audience-active-users.jpg)

We call this __Active Users__ feature, __"Site Reach or Stickiness".__ 

If the content of the page is encouraging to the audience to come back, this number of active users has to grow.

- __Demographics Report:__ it show information about the age, and gender of the users.

- __Interests Report:__ Shows the general user taste for specific web contents. like technology, travel, music, etc.

In order to see the interest and demographic reports, we need to activate them for all properties. In order to do this:
` click on admin, under each property click on property setting, then under advertizing features, enable demographics and interest reports.`

- __Geo Reports:__ It is so useful for example we can see what countries are having high conversion rate, or transactions, but low traffic rates. `This shows unptapped market to be potential target for advertising.` Another analysis, is to see what country or region has already large amount of audience but lower than average performance. `If in some countries we have high bounce rate, or find out people leaving after visiting a particular page, we must update the content of that page or the related ad. Maybe there is an ad that needs to be translaated to the local language.`
 
- __Behavior Reports:__ shows how the users behave. new vs returning users show the different metrics and goals for new and returning users.

-__Technology, and Mobile reports:__ Using these, we make sure that the website works well in any browser, or operation system or device.

2- Acquisition Reports: This is a very useful report that we use to compare which marketing channel is performing better, and discover which sources sends the website the highest quality traffic and conversion. `it helps to decide where and how to foucs on the marketing efforts'.`

When a user lands on a page, the GA tracker, captures 3 info:

- __Medium:__ The mechanism that delivers user to this page: organic, cpc, referral, email, none.
        
        * organic comes from non-paid search results
        * CPC comes from paid google searches.
        * Referral comes another website other than the search engine.
        * email refers to the user clicking on an email marketing campaing.
        * None, is the user who directly typed the url into the browser.
- __Source:__ Source provides more information about the medium. For example, if the medium is referral, then the source will be the url of the website that the user clicked on. If the medium is organic, the source will be the name of the search engine.
Under `acquisition/all traffic` we can use source/medium to see both of medium and source at the same time. in this report we can see the source-mediums with the highest users which shows which one is performing better (photo: acquisition-medium-source-report.jpg).
        
  However, we don't know the quality of this traffic and the number of the users is not a good enough indicator of the business performance. `A good performance indicator, is the bounce rate.` This is a very nice comparision acquisition-bounce-comparison,jpg to know that although Youtube had very high user view, but it had the highest bounce rate.
  
  Another nice example, is to search for organic in the medium-source report and see what source is bringing more organic traffic. (photo: acquisition-organic-traffic-source-comparison.jpg)
  
  Another example, by seeing how much each Google related marketing activity has performed we can search for Google in the same report. (photo: acquisition-google-marketing-sources-comparison.jpg)
  
  Referrals under the acquisition, shows which web pages are sending traffic to the website and we can add second dimension called Landing Page to see what page of our website is being linked to the referring sites. (photo: acquisition-referral-landing-page.jpg)
- __Campaign__ 

__Review:__ URI is the part of URL after the domain name.

