---

copyright:
  years: 2016

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:screen: .screen}
{:pre: .pre}


# Getting started with {{site.data.keyword.iotmapinsights_full}} (Experimental)
{: #gettingstartedtemplate}
*Last updated: 18 March 2016*

## Overview

{{site.data.keyword.iotmapinsights_full}} makes it easy for developers to enable their applications to use geospatial functions such as map matching and shortest path search based on the road networks across the globe.
{:shortdesc}

You can use the following functions through the {{site.data.keyword.iotmapinsights_short}} REST API:

- Highly accurate map matching that use road network geometry.
- Create, find, and remove real-time events on a map, such as traffic.
- Dynamic shortest path search (route search) considering real-time events, such as traffic.
- Retrieve road geometry data that can be used for drawing road shapes on a map.

The {{site.data.keyword.iotmapinsights_short}} service uses the road network data in WGS84 coordinates that is extracted from OpenStreetMap. Only the roads that a vehicle can travel on are used for analysis.

Supported map regions are:

- Europe (map_id=1)
- Africa (map_id=2)
- Asia (map_id=3)
- Australia Oceania (map_id=4)
- North America (map_id=5)
- Central America (map_id=6)
- South America (map_id=7)

## How to add {{site.data.keyword.iotmapinsights_short}} service

Follow these steps to add {{site.data.keyword.iotmapinsights_short}} service to your Bluemix organization:

1. From your Bluemix account Dashboard, click **CATALOG**.
2. Locate the **Internet of Things** section of the service catalog and select **{{site.data.keyword.iotmapinsights_full}}**.
3. On the {{site.data.keyword.iotmapinsights_full}} page, verify the **Add Service** selections:
  - App - Leave unbound.
  - Service name - Optionally change the service name to something that is easy to remember. This name is displayed in the {{site.data.keyword.iotmapinsights_full}} tile in the Bluemix Dashboard.
  - Selected plan - Select Free or purchase plan that is suitable for your needs.  
    **Important:** With the Free plan, the total number of REST API calls is limited to 10000 times per month.
4. Click **CREATE** to deploy {{site.data.keyword.iotmapinsights_full}} to your Bluemix services.

## How to use the {{site.data.keyword.iotmapinsights_short}} service

Follow these steps to use the analytics functions of the {{site.data.keyword.iotmapinsights_short}} service.

### Map Matching

1. Prepare a set of raw GPS coordinates data to be analyzed.
2. Send raw GPS coordinates data in time-series order to the {{site.data.keyword.iotmapinsights_short}} service by using the mapMatching REST API. You can optionally set a heading angle of each position in degrees (North is 0, clockwise angle) to specify its direction of travel.
3. Receive a map matched coordinates and road link information in response to the mapMatching REST API call.
4. Optionally, you can retrieve road shape data of the map matched road link by using the getLinkInformation REST API. Call the getLinkInformation REST API with a link ID to get a series of coordinates that consists of a road shape.

### Route Search

1. Determine a start and end position that you want to get a shortest path for.
2. Send a start and end coordinates to the {{site.data.keyword.iotmapinsights_short}} service by using the routeSearch REST API. You can optionally set a heading angle of each position in degrees (North is 0, clockwise angle) to specify its direction of travel.
3. Receive a list of road links in response to the routeSearch REST API call. You can draw the shape of the found path on a map by using the shape data that is included in the result data.

### Traffic Event Manipulation

1. Determine a type and position of a traffic event that you want to create.
2. Send traffic event information to the {{site.data.keyword.iotmapinsights_short}} service by using the createEvent REST API.
3. Receive an event ID of the created traffic event in response to the createEvent REST API call.
4. You can search traffic events within a specific rectangular area, and/or with a specific traffic event type, by using the queryEvent REST API.
5. You can remove a traffic event that is no longer valid using the deleteEvent REST API.
6. Optionally, you can retrieve an area on the road that is affected by a traffic event by using the getAffectedLinksInformation REST API.

For more information on REST API usage, see the {{site.data.keyword.iotmapinsights_short}} REST API documentation.


## Copyright Notice

Map data [(C) OpenStreetMap contributors](http://www.openstreetmap.org/){:new_window}, [ODbL](http://opendatacommons.org/licenses/odbl/){:new_window}


# Related Links
{: #rellinks}

## API Reference
{: #api}
* [REST API Documentation](https://new-console.ng.bluemix.net/apidocs/123){:new_window}

## Related Links
{: #general}
* [dW Answers on IBM developerWorks](https://developer.ibm.com/answers/topics/iot-map-insights/){:new_window}
* [Stack Overflow](http://stackoverflow.com/questions/tagged/iot-map-insights){:new_window}
* [What's new in Bluemix Services](http://www.ng.bluemix.net/docs/whatsnew/index.html#services_category){:new_window}

