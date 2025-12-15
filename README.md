# Python-Nested-Config-Manager
# Define a nested dictionary for application configuration
app_config = {
    "server": {
        "host": "127.0.0.1",
        "port": 8080,
        "mode": "development"
    },
    "database": {
        "type": "postgres",
        "name": "app_db",
        "enabled": True
    },
    "logging": {
        "level": "INFO",
        "file": "/var/log/app.log"
    }
}

# Accessing a value deep inside the nested structure
db_name = app_config['database']['name']
server_port = app_config['server']['port']

print(f"Database Name retrieved: {db_name}")
print(f"Server Port retrieved: {server_port}")
