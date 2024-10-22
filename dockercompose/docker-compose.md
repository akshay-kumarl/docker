### docker-compose.yml

```
version: '3.8'

services:
  app:
    image: my-app:latest
    ports:
      - "8080:8080"
    secrets:
      - db_password
    environment:
      DB_PASSWORD_FILE: /run/secrets/db_password
    depends_on:
      - db

  db:
    image: postgres:latest
    environment:
      POSTGRES_USER: user
      POSTGRES_PASSWORD_FILE: /run/secrets/db_password
    secrets:
      - db_password
    volumes:
      - db-data:/var/lib/postgresql/data

secrets:
  db_password:
    file: ./secrets/db_password.txt

volumes:
  db-data:
```

---

Steps: <br/>
Create a secrets folder in the same directory as your docker-compose.yml file.<br/>
Inside that folder, create a db_password.txt file with your secret content (the database password, in this case).
