# SQL Server Docker Compose Template 🐳

This Docker Compose template simplifies the process of setting up and running a Microsoft SQL Server instance using Docker. You can quickly spin up a SQL Server container with the configuration specified below.

## Usage

1. **Start SQL Server Container:**
   - Open a terminal in the directory containing the `docker-compose.yml` file.
   - Run the following command:
     ```bash
     docker-compose up -d
     ```
   This command will pull the SQL Server image and start a container with the specified configuration.

2. **Access SQL Server:**
   - Once the container is running, you can connect to the SQL Server instance using your preferred SQL client.
   - Use the following connection details:
     - **Server:** localhost (or Docker host IP)
     - **Port:** 1433
     - **Authentication:** SQL Server Authentication
     - **Username:** sa
     - **Password:** `<YourStrong@Passw0rd>` (as specified in the `docker-compose.yml` file)

3. **Stop and Remove Container:**
   - To stop the SQL Server container, run:
     ```bash
     docker-compose down
     ```
   This command will stop and remove the container, but the data volume will persist unless explicitly removed.

## Customization

- **Password:** Replace `<YourStrong@Passw0rd>` in the `docker-compose.yml` file with your desired SQL Server SA password.
- **Additional Configuration:** Modify other parameters such as environment variables, ports, and volumes as needed.

## Thank You! 🙏

Thank you for using this Docker Compose template! We hope it simplifies your SQL Server setup process. If you encounter any issues or have suggestions for improvement, feel free to reach out.

---

Happy SQL querying! 🚀