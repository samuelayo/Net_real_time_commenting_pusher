# BUILD REALTIME COMMENTS USING ASP.NET

Here, we will learn about implementing real-time comment feature using pusher and .NET. The full tutorial can be found here : [https://pusher.com/tutorials/realtime-comments-aspnet/ ](https://pusher.com/tutorials/realtime-comments-aspnet/) 

## Getting Started


### Prerequisites

#### Setup Pusher

If you don't have one already, create a free Pusher account at https://pusher.com/signup then login to your dashboard and create an app. 


Then fill in your Pusher app credentials in your `Controllers\HomeController` file by replacing this line with your appcluster, appid, appkey and app secret respectively:

```
options.Cluster = "XXX_APP_CLUSTER";
var pusher = new Pusher("XXX_APP_ID", "XXX_APP_KEY", "XXX_APP_SECRET", options);
```

Also, remember to fill in the your secret key and app cluster in your `Views\Home\Details.cshtml` file by updating this line:

```
var pusher = new Pusher('XXX_APP_KEY', {cluster: 'XXX_CLUSTER'});
```

And finally, start the application by clicking the debug button on your visual studio.

## Built With

* [Pusher](https://pusher.com/) - APIs to enable devs building realtime features
* [ASP.NET](https://www.asp.net/) - Open source web framework for building modern web apps and services with .NET. 
* [Vue.js](https://vuejs.org/) - The Progressive JavaScript Framework

