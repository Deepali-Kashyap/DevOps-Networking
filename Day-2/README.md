# Common Protocols and Ports for DevOps

In DevOps, understanding network protocols and their associated ports is crucial for setting up, securing, and troubleshooting infrastructure and deployments. This guide lists some of the most commonly used protocols, their default port numbers, and explains why they matter in DevOps workflows.

---

## 🔹 1. HTTP (HyperText Transfer Protocol)  
- **Port:** 80  
- **Description:** The foundation of data communication on the web. Used for transmitting web pages.  
- **Relevance to DevOps:**  
  - Managing web servers (Apache, Nginx).  
  - Configuring load balancers and reverse proxies.  
  - Monitoring web traffic and debugging applications.

---

## 🔹 2. HTTPS (HTTP Secure)  
- **Port:** 443  
- **Description:** Secure version of HTTP using SSL/TLS encryption.  
- **Relevance to DevOps:**  
  - Securing web traffic and APIs.  
  - Managing SSL certificates and automated renewals (e.g., Let's Encrypt).  
  - Ensuring compliance and secure deployments.

---

## 🔹 3. FTP (File Transfer Protocol)  
- **Port:** 21 (command), 20 (data)  
- **Description:** Used for transferring files between client and server.  
- **Relevance to DevOps:**  
  - Legacy deployments and file transfers.  
  - Often replaced by more secure protocols like SFTP, but understanding FTP helps in migration.

---

## 🔹 4. SSH (Secure Shell)  
- **Port:** 22  
- **Description:** Secure remote login and command execution.  
- **Relevance to DevOps:**  
  - Accessing servers securely for management and automation.  
  - Used in CI/CD pipelines to deploy code remotely.  
  - Key for tunneling and port forwarding.

---

## 🔹 5. DNS (Domain Name System)  
- **Port:** 53 (UDP/TCP)  
- **Description:** Translates domain names into IP addresses.  
- **Relevance to DevOps:**  
  - Managing domain names and routing traffic.  
  - Configuring internal and external DNS for applications and microservices.  
  - Troubleshooting connectivity issues.

---

## 🔹 6. SMTP (Simple Mail Transfer Protocol)  
- **Port:** 25 (unencrypted), 587 (submission)  
- **Description:** Sending emails between servers.  
- **Relevance to DevOps:**  
  - Configuring alerting and notification systems.  
  - Managing email services for applications.

---

## 🔹 7. SFTP (SSH File Transfer Protocol)  
- **Port:** 22  
- **Description:** Secure file transfer over SSH.  
- **Relevance to DevOps:**  
  - Securely transferring files during deployment.  
  - Automating backup and restore processes.

---

## Why DevOps Professionals Need to Know Protocols & Ports

- **Security:** Opening only necessary ports reduces attack surfaces.  
- **Automation:** Scripts often rely on SSH or APIs over HTTP/S.  
- **Monitoring:** Knowing protocols helps in analyzing network traffic and logs.  
- **Troubleshooting:** Port conflicts or blocked ports can cause deployment failures.

---

## Conclusion

Mastering common protocols and their ports empowers DevOps engineers to design secure, reliable, and efficient infrastructure. This knowledge helps in configuring services correctly, debugging network issues, and ensuring smooth application delivery.

---

**Feel free to use and share!**

