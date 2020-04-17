# Instructions
Please note that the [Transform secrets engine](https://www.vaultproject.io/docs/secrets/transform) is an Enterprise only feature. If you wish to use Transform in this demo, make sure you are using Vault Enterprise. The Vault Enterprise binary is available at releases.hashicorp.com/vault, and will be denoted by a +ent in the name. It will run for 30 minutes without a license before shutting down.

Install flask, hvac, and mysql connector:
```
pip3 install Flask mysql-connector-python hvac
```

## Configuration

The application reads a file named "config.ini" when it starts.  Database location, credentials, etc, are contained therein.  

## Run

Run the application from the backend folder:
```
python3 app.py
```

