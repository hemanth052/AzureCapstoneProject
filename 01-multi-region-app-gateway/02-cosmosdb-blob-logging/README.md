# Cosmos DB Logging & Azure Blob Integration

In this project, a Python-based web app uploads files to Azure Blob Storage and logs metadata into Cosmos DB.

Key Features:
- Uploads files through a Python app hosted on Azure VM
- Stores metadata in Cosmos DB using SQL API (timestamp, file ID)
- Uses a container named `upload` inside the storage account
- Hosted error page in Blob Storage as a static site

Important Configuration:
- Modify `config.py` with the correct Blob Storage and Cosmos DB credentials
- Use `app.py` to test and verify uploads and logging
