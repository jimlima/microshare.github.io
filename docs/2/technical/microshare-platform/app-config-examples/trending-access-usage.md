---
layout: docs
title: Trending Access Usage JSON
description: 
toc: true
---

---------------------------------------

The following is JSON example code for a Trending Access Usage App. 

{% highlight java %}

{
  "appTitle": "Trending Access Usage",
  "navOptions": [
    {
      "title": "Realtime Desk Availability",
      "link": "https://dapp.microshare.io/apps/view/5e0f8cd22b0000d1c260????"
    },
    {
      "title": "Realtime Room Availability",
      "link": "https://dapp.microshare.io/apps/view/5e2b627d2b000057df94????"
    },
    {
      "title": "Trending Environment",
      "link": "https://dapp.microshare.io/apps/view/5de835881d0000dbbc83????"
    },
    {
      "title": "Trending Environment F",
      "link": "https://dapp.microshare.io/apps/view/5e0a72cc2b0000940160????"
    },
    {
      "title": "Trending Air Quality",
      "link": "https://dapp.microshare.io/apps/view/5e0a75502b0000600260????"
    },
    {
      "title": "Trending Refrigerator",
      "link": "https://dapp.microshare.io/apps/view/5e0f6d2a2b0000dcb760????"
    },
    {
      "title": "Trending Access Usage",
      "link": "https://dapp.microshare.io/apps/view/5e0fa0842b00008dc960????"
    },
    {
      "title": "Trending Desk Availability",
      "link": "https://dapp.microshare.io/apps/view/5e0e1f632b00006e4360????"
    },
    {
      "title": "Trending Usage",
      "link": "https://dapp.microshare.io/apps/view/5e0e02e92b0000433960????"
    },
    {
      "title": "Trending Feedback 3",
      "link": "https://dapp.microshare.io/apps/view/5e1742252b00001ce1e2????"
    },
    {
      "title": "Trending Feedback 5",
      "link": "https://dapp.microshare.io/apps/view/5e172aa52b0000656860????"
    }
  ],
  "": "optional parameters",
  "getRecType": "io.microshare.fm.master.agg",
	"headerLogo": "https://s3.amazonaws.com/cdn.point.io/distribution/product/1_00/header.png",
	"headerSecondaryLogo": "",
	"footerLogo": "https://s3.amazonaws.com/cdn.point.io/distribution/product/1_00/footer.png",
	"axisFormat": "EEE HH:mm",
	"location1": "Building",
	"location2": "Floor",
	"location3": "Location",
	"startOfWorkDay": 6,
	"endOfWorkDay": 20,
	" ": "end optional parameters",

  "dataRecType": "com.netvox.security.R311A",
  "dataContext": "toilet",
  "query1variable": "5e0f639546e0fb00283f????",
  "query2variable": "5e0f9e3046e0fb00284a????",
  "query3variable": "5e0f9e5446e0fb00283f????",
  "charts": [ 
    { 
      "fieldName":"counter",
      "title": "Access Usage",
      "": "optional parameters"
    }
  ],
  "selectionOptions": [
    {
      "name": "Boston",
      "floors": [
        {
          "name": "1st Floor",
          "locations": [
            "A",
            "B",
            "C"
          ]
        },
        {
          "name": "2nd Floor",
          "locations": [
            "A",
            "B",
            "C"
          ]
        },
        {
          "name": "3rd Floor",
          "locations": [
            "A",
            "B",
            "C"
          ]
        }
      ]
    },
    {
      "name": "London",
      "floors": [
        {
          "name": "1st Floor",
          "locations": [
            "A",
            "B",
            "C"
          ]
        },
        {
          "name": "2nd Floor",
          "locations": [
            "A",
            "B",
            "C"
          ]
        },
        {
          "name": "3rd Floor",
          "locations": [
            "A",
            "B",
            "C"
          ]
        }
      ]
    }
  ]
}

{% endhighlight %}