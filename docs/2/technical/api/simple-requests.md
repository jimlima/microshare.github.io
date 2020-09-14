---
layout: docs
title: Simple Requests
description: Get started with the Microshare™  API 
toc: true
---






{% include image.html url="/assets/img/thumbnail-7.jpg" height="900" width="900" description="thumbnail 2" %}


<br>

---------------------------------------

##### SUMMARY : 

1. [Overview](./#1-overview)
2. [Write Data](./#2-write-data)
3. [Read Data](./#3-read-data)
4. [From a postman call to a piece of code](./#4-from-a-postman-call-to-a-piece-of-code)

---------------------------------------

## 1. Overview
---------------------------------------

Now that you have completed authentication, you can now make your first requests.

This guide will walk you through how to write data and request information from the APIs. 

For this there are endpoints, similar to addresses, where data is stored. 

In the examples below we will create your own specific endpoints (recType). But we often use predefined endpoints that correspond to the type of data itself. You can find this information in the [data ingestion page.](/docs/2/technical/microshare-platform-advanced/data-ingestion/)

If you then want to read more conventional data, you can try the [demo APIs.](/docs/2/technical/api/quick-start/#4-demo-api) 



## 2. Write data
---------------------------------------

**1.** From the Postman collection, open the request `Shares -> Create one Share`.

<br>
**2.** Click on `Params`, next to the `Send` button, to edit the recType Value. The recType is the category, or id, under which the data is stored in Microshare®. You usually have one recType per data stream (per IoT gateway, or IoT device if you can differentiate them).

<br>
{% include image.html url="/assets/img/api/create_one_share_1new.png" description="create one share" %}

<br>
**3.** Enter you own recType there, by using your `firstName.lastName` combination.

<br>
**4.** Click on the `Body` tab, under the Params zone, and write any JSON body there, for example `{"Test":"Data"}`.

<br>
{% include image.html url="/assets/img/api/create_one_share_2new.png" description="create one share" %}

<br>
**4.** Click `Send`

<br>
{% include image.html url="/assets/img/api/create_one_share_3new.png" description="create one share" %}

<br>
**5.** A confirmation message will be sent, indicating that the data was successfully written to Microshare®. It returns metadata usable with other API calls.



## 3. Read data
---------------------------------------

**1.** From the Postman collection, open the request `Shares -> Get Shares by recType` to configure it.

<br>
**2.** Click on `Params`, next to the `Send` button, to edit the recType Value. Specify the recType you used in the Write query.

<br>
{% include image.html url="/assets/img/api/read_share_1new.png" description="read share" %}

<br>
**3.** Click `Send`. The return response will be all the information stored under that recType(endpoint). Part of the displayed metadata is your login and API key, showing that YOU are the owner of that data:

{% include image.html url="/assets/img/api/read_share_2new.png" description="read share" %}

**4.** If you execute Write request again, and then the Read, the number of records increases as you have created a new record. The Microshare® metadata tells you how many pages of records you have, and the total number of records (platform wide) stored under this recType.

**Note:** The `totalCount` value can be higher than the total number of records you own.  This is because another user could be storing data under the same recType. Don't worry, you will only see your data, and the other users will only be able to see their data, unless you have created Rules to share your data.

Rules are an advanced feature of the platform, and are better described in the [Rules Guide.](/docs/2/technical/microshare-platform/rules-guide)

**5.** You can use the request `Shares -> Get Latest Shares by recType`, that returns only the very last record created under this recType.

**6.** For more information on how to setup a IoT data stream from a web platform using this API, check our [Robots Library.](docs/2/technical/microshare-platform-advanced/robots-library/)



## 4. From a postman call to a piece of code
---------------------------------------

We have a list of 7 fairly simple API requests available in this Postman Collection. You can find the information and parameters of each of them in the API Collection file.

##### > [API Collection](../api-collection)

Once you have found the query you need on Postman, you can very quickly extract a functional code for your application: 

- Simply click on the code button once your query is good. 

{% include image.html url="/assets/img/api/get_code_postman_0new.png" description="read share" %}

- Choose your programming language and you will get your code. 

{% include image.html url="/assets/img/api/get_code_postman_1new.png" description="read share" %}


**<!> Be careful the token is valid for only 48 hours, it is generally necessary to have a request of authentification beforehand and then use this token through your request. <!>**

{% include image.html url="\assets\img\microshare-logo.png"  description="ms logo" %}