# Net_real_time_commenting_pusher
Implementing real-time comment feature using pusher and .NET

### Getting Started

Clone the project repository by running the command below if you use SSH

```
git clone git@github.com:samuelayo/Net_real_time_commenting_pusher.git
```

If you use https, use this instead

```
git clone https://github.com/samuelayo/Net_real_time_commenting_pusher.git
```

After cloning, open the `Real-Time-Commenting.sln` file in visual studio.

### Setup Pusher

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
