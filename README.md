# Setup:

create `my_network` with `docker network create my_network`


# Launch server

```
cd server/
docker-compose up
```

# Launch client

## With docker-compose (What I want to do)
```
cd client/
docker-compose up
```
but that gives me:
```
Creating client_my_client_1 ... done
Attaching to client_my_client_1
my_client_1  |   % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
my_client_1  |                                  Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
my_client_1  | curl: (7) Failed to connect to localhost port 3000 after 0 ms: Couldn't connect to server
my_client_1  | Message:
client_my_client_1 exited with code 0
```

## Manually
```
cd client/
sh script.sh
```
which works, and gives me:
```
➜ sh script.sh
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100    13  100    13    0     0   1957      0 --:--:-- --:--:-- --:--:--  2166
Message: Hello, World!
```
