# Task 7: Monitor System Resources Using Netdata

## 📝 Objective
Set up **Netdata**, a free and open-source real-time monitoring tool, to visualize system and application performance metrics such as CPU, memory, disk, and running processes.

---

## 🛠 Tools Used
- **Netdata** (lightweight system monitoring)
- **Docker** (containerized setup)

---

## 🧩 Steps Performed

1. **Pulled and Ran Netdata via Docker:**

   ```bash
docker run -d --name=netdata \
  -p 19999:19999 \
  --cap-add=SYS_PTRACE \
  --security-opt apparmor=unconfined \
  netdata/netdata
 
   

2. **Accessed the Netdata Dashboard:**
   - Opened browser and visited:  
     `http://<EC2-PUBLIC-IP>:19999`

3. **Explored System Metrics:**
   - Real-time charts for:
     - CPU usage
     - Memory consumption
     - Disk activity
     - Active processes and app performance
   - Observed alerts and performance spikes


## 📸 Dashboard Screenshot

> ![Uploading image.png…]()

)

---

## ✅ Outcome
- Gained experience with lightweight performance monitoring
- Understood how to visualize system health in real-time
- Learned how to use Docker for quick setup of monitoring tools

---
