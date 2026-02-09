# AWS-System-Monitoring-with-Netdata
**Overview**

This project demonstrates the setup of a real-time system monitoring dashboard using Netdata on a Linux server hosted on AWS. The primary goal is to monitor system health, visualize performance metrics, and set up alerts for key resources like CPU, memory, and disk usage.

This project showcases practical skills in system monitoring, dashboard customization, and alert configuration — essential for DevOps and system administration.

**Features**

1.Real-time Monitoring: Monitor system metrics including CPU usage, memory usage, and disk I/O in real time.

2.Web-Based Dashboard: Access an interactive Netdata dashboard via a web browser.

3.Dashboard Customization: Customize charts and layouts for enhanced visualization.

4.Alerts Setup: Configure alerts for specific thresholds, e.g., CPU usage above 80%, to proactively manage system health.

5.AWS Deployment: The monitored server runs on AWS, demonstrating cloud-based monitoring capabilities.

**Technologies Used**

Netdata – Real-time performance and health monitoring tool for systems and applications.

 Linux Server – Cloud-based Linux environment used for hosting and running Netdata.

Linux Command Line (CLI) – Used for installation, configuration, and management of the monitoring system.

Web Browser – Access and visualize the Netdata dashboard.

**Usage**

Follow these steps to set up and use the monitoring dashboard:

1.Access your AWS Linux server via SSH:
```
ssh -i <your-key.pem> ec2-user@<your-server-ip>
```

2.Install Netdata using the official installation script:
```
bash <(curl -Ss https://my-netdata.io/kickstart.sh)
```

3.Start Netdata (if not already running):
```
sudo systemctl start netdata
```

4.Access the dashboard in your web browser:
```
http://<your-server-ip>:19999

```
6.Customize the dashboard:

•Add new charts or modify existing charts via the Netdata configuration files.

•Example: Monitor a custom directory or application metric.

7.Set up alerts for critical metrics:

•Edit the Netdata configuration to trigger alerts, e.g., CPU usage > 80%.

•Netdata will notify you in real-time via email, Slack, or other configured channels.

•Monitor system health in real-time and explore the interactive charts for CPU, memory, disk I/O, and other metrics.



**Metrics**

<img width="1919" height="869" alt="Screenshot 2026-02-10 004530" src="https://github.com/user-attachments/assets/61e44676-79eb-48a2-887a-b327bba85022" />



**Custom Dashboard**



<img width="1911" height="858" alt="Screenshot 2026-02-10 004554" src="https://github.com/user-attachments/assets/cef3ad41-5495-40d3-840a-4f4e0f37bdeb" />

**Alerts**

<img width="1913" height="871" alt="Screenshot 2026-02-10 004619" src="https://github.com/user-attachments/assets/b70f1ae0-c642-4361-ac77-dd1fb249c0ba" />
