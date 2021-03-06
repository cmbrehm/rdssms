+++
title = "CloudWatch and Enhanced Monitoring"
date = 2020-06-10T09:35:30-07:00
weight = 30
pre = "<b>6.3 </b>"
+++

You can monitor DB instances using Amazon CloudWatch, which collects and processes raw data from Amazon RDS into readable, near real-time metrics. By default, Amazon RDS metric data is automatically sent to CloudWatch every 60 seconds. Metrics collected with a period of 60 seconds (1 minute) are retained for 15 days. Metrics may be retained for longer if collection interval changes. For more information, see [Metrics Retention](https://docs.aws.amazon.com/AmazonCloudWatch/latest/DeveloperGuide/cloudwatch_concepts.html#metrics-retention) in the Amazon CloudWatch User Guide. 

* Open the [Amazon RDS  service console](https://console.aws.amazon.com/rds/home) and click on [Databases](https://console.aws.amazon.com/rds/home#databases:) from left navigation pane. From list of databases click on `sqlserver-rdssql` under **DB identifier**. On the database details view, click on the **Monitoring** tab.
{{% img "cloudwatch.png" "cloudwatch" %}}

* You can click on a chart to drill down for more details, select any chart area to zoom in on a specific time period. 
{{% img "chart.png" "chart" %}}

* If you have Enhanced Monitoring option enabled for the database instance, select **Enhanced Monitoring** option from the **Monitoring** dropdown list. 
{{% img "enhancedMonitoring.png" "enhancedMonitoring" %}}

* You will see additional counters showing metrics captured at the guest OS level.
{{% img "enhancedMonitoringCharts.png" "enhancedMonitoringcharts" %}}