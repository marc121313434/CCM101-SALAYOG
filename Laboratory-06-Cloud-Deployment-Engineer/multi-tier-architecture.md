Web/Application Tier
- The Web/Application Tier is responsible for serving the user interface and handling incoming HTTP requests. It processes client interactions, manages business logic, and delivers dynamic or static content to the user’s browser.

Database Tier
- The Database Tier is dedicated to storing persistent data such as user accounts, application records, and transactional information. It ensures data integrity, security, and efficient retrieval whenever the application tier requests information.

Why Separate Them?
- Separating the web server and the database into distinct tiers improves scalability, security, and maintainability. Each tier can be optimized independently, making it easier to update, troubleshoot, or scale without affecting the other.

Containers Advantage
- Running the web server and database in two separate containers is better than packing them into one because it enforces isolation and modularity. This separation allows independent scaling (e.g., adding more web containers during high traffic), simplifies updates, and reduces the risk of one service failure impacting the other. It also aligns with best practices in cloud-native deployment, ensuring flexibility and resilience.
