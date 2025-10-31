# 🚀 Task 7 – Monitor System Resources Using Netdata

This repository contains the solution for **Task 7** of the DevOps Internship Program. The objective of this task was to install and configure **Netdata** to monitor system and application performance metrics in real-time.

-----

## 📌 Objective

The primary goal of this project was to gain hands-on experience with a lightweight monitoring tool. By deploying Netdata and visualizing key performance metrics, this task demonstrates an understanding of how to monitor system health, a critical skill in the DevOps and Systems Administration domains.

-----

## 🛠️ Tools Used

  * **Netdata:** A free, open-source, and real-time performance monitoring tool.
  * **Docker:** Used to run Netdata in an isolated container, simplifying the installation and setup process.

-----

## 📂 Project Structure

```
task-7-netdata-monitoring/
├── README.md                 # Project documentation
└── docs/                     # Documentation and output screenshots
    └── screenshots/          # Verification screenshots
        ├── dashboard.png
        └── running-metrics.png
```

-----

## ▶️ Steps to Complete the Task

### 1️⃣ Run Netdata via Docker

Netdata was launched using a single Docker command, which automatically pulls the `netdata/netdata` image and starts a container in the background.

```bash
docker run -d --name netdata -p 19999:19999 netdata/netdata
```

  * `-d`: Runs the container in detached mode.
  * `--name netdata`: Assigns a name to the container for easy management.
  * `-p 19999:19999`: Maps port `19999` on the host machine to port `19999` inside the container, allowing access to the dashboard.

### 2️⃣ Access and Explore the Dashboard

After the container started, the Netdata dashboard was accessed by navigating to `http://localhost:19999` in a web browser. The dashboard presented a rich, real-time view of various system metrics.

### 3️⃣ Capture Screenshots

Two key screenshots were captured to fulfill the task requirements:

1.  **Dashboard Screenshot (`dashboard.png`):** This image shows the main Netdata interface, highlighting a comprehensive overview of the system's performance.
2.  **Running Metrics Screenshot (`running-metrics.png`):** This image captures a closer look at specific, active metrics, such as CPU, memory, and disk usage, showcasing the real-time visualization capabilities of Netdata.

Both screenshots are located in the `docs/screenshots` directory.

### 4️⃣ Stop the Netdata Container

To conserve system resources after completing the task, the Netdata container was gracefully stopped.

```bash
docker stop netdata
```

-----

## 📸 Screenshots

  * **Dashboard** → Located at `docs/screenshots/dashboard.png`
  * **Running Metrics** → Located at `docs/screenshots/running-metrics.png`

-----

## ✅ Key Learnings

  * **Understanding Monitoring:** Gained an understanding of what system monitoring is and why it's crucial for maintaining the health of servers and applications.
  * **Docker Fundamentals:** Practiced using Docker commands to deploy an application quickly and efficiently.
  * **Netdata Concepts:** Explored key features of Netdata, including its real-time dashboard, metric visualization, and the ability to monitor various system components like CPU, memory, and disk I/O.
  * **Lightweight Solutions:** Learned about the benefits of using a lightweight, open-source tool like Netdata for monitoring without heavy resource consumption.

-----


-----

## 🤝 Author

**Sumit Wade**

[🔗 GitHub Profile](https://www.google.com/search?q=https://github.com/SumitWade)

-----

## 📌 Summary

This task successfully demonstrates practical knowledge of system monitoring, containerization with Docker, and the ability to use an open-source tool to visualize performance data. The project provides a solid foundation for understanding critical aspects of system administration and DevOps.