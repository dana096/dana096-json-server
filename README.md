# dana096-json-server
![LGTM](https://i.lgtm.fun/2p1o.png)

### RUN
```
$ npx json-server db.json
JSON Server started on PORT :3000
Press CTRL-C to stop
Watching db.json...

(˶ᵔ ᵕ ᵔ˶)

Index:
http://localhost:3000/

Static files:
Serving ./public directory if it exists

Endpoints:
http://localhost:3000/posts
http://localhost:3000/comments
http://localhost:3000/profile
```

### Launch
⚠️ Do you want to tweak these settings before proceeding? Yes
```
$ flyctl launch
Scanning source code
Detected a Dockerfile app
Creating app in /home/dana096/code/dana096-json-server
We're about to launch your app on Fly.io. Here's what you're getting:

Organization: lovejiwon11@gmail.com  (fly launch defaults to the personal org)
Name:         dana096-json-server    (derived from your directory name)
Region:       Tokyo, Japan           (this is the fastest region for you)
App Machines: shared-cpu-1x, 1GB RAM (most apps need about 1GB of RAM)
Postgres:     <none>                 (not requested)
Redis:        <none>                 (not requested)

? Do you want to tweak these settings before proceeding? Yes
failed opening browser. Copy the url (https://fly.io/cli/launch/cf6868841a7f6110a056b388d1e1ce94) into a browser and continue
Waiting for launch data... Done
Created app 'dana096-json-server' in organization 'personal'
Admin URL: https://fly.io/apps/dana096-json-server
Hostname: dana096-json-server.fly.dev
? Create .dockerignore from 1 .gitignore files? Yes
Created /home/dana096/code/dana096-json-server/.dockerignore from 1 .gitignore files.
Wrote config file fly.toml
Validating /home/dana096/code/dana096-json-server/fly.toml
Platform: machines
✓ Configuration is valid
==> Building image
Remote builder fly-builder-blue-star-443 ready
Remote builder fly-builder-blue-star-443 ready
==> Building image with Docker
--> docker host: 20.10.12 linux x86_64
[+] Building 139.1s (10/10) FINISHED
 => [internal] load build definition from Dockerfile                                0.5s
 => => transferring dockerfile: 201B                                                0.4s
 => [internal] load .dockerignore                                                   0.5s
 => => transferring context: 103B                                                   0.4s
 => [internal] load metadata for docker.io/library/node:20.11                       1.5s
 => [internal] load build context                                                   0.8s
 => => transferring context: 373B                                                   0.6s
 => [1/5] FROM docker.io/library/node:20.11@sha256:fd0115473b293460df5b217ea73ff2  92.5s
 => => resolve docker.io/library/node:20.11@sha256:fd0115473b293460df5b217ea73ff21  0.0s
 => => sha256:c3e72880014551ecfe631aae3aef14ed33b7e58b4b682f5a3988 2.00kB / 2.00kB  0.0s
 => => sha256:723a77f71cf06aeaa21ea74bfc1299e8362d26db488a7fba4e8b 7.34kB / 7.34kB  0.0s
 => => sha256:e08e8703b2fb5e50153f792f3192087d26970d262806b39704 24.05MB / 24.05MB  1.5s
 => => sha256:fd0115473b293460df5b217ea73ff216928f2b0bb7650c5e7aa5 1.21kB / 1.21kB  0.0s
 => => sha256:6a299ae9cfd996c1149a699d36cdaa76fa332c8e9d66d6678f 49.58MB / 49.58MB  3.0s
 => => sha256:5b9fe7fef9befda786bc8e1dd1ae42ffd8b9c37a4cce3c43 211.11MB / 211.11MB  8.3s
 => => sha256:dc95f2a6ccee7fb934bd659ef134da3e3c71c2a4a8059fe3c79a7d23 450B / 450B  0.9s
 => => sha256:68e92d11b04ec0fe48e60d59964704aca234084f87af5d1a06 64.14MB / 64.14MB  4.5s
 => => sha256:9b5f63cb30c69fe1a827c8fea9d33bd7026dffa193ed449ff4 47.99MB / 47.99MB  3.9s
 => => sha256:278d467c182fb935287ed6f4be3d44f8ac2714264bcb58b883d0 3.37kB / 3.37kB  1.1s
 => => sha256:230542c909b8c810d61434d1f259307fac388dda9d2daca1aaf0 2.21MB / 2.21MB  1.4s
 => => extracting sha256:6a299ae9cfd996c1149a699d36cdaa76fa332c8e9d66d6678fa9a231  13.3s
 => => extracting sha256:e08e8703b2fb5e50153f792f3192087d26970d262806b397049d61b9a  4.4s
 => => extracting sha256:68e92d11b04ec0fe48e60d59964704aca234084f87af5d1a068c4945  17.3s
 => => extracting sha256:5b9fe7fef9befda786bc8e1dd1ae42ffd8b9c37a4cce3c433e65ebb8  36.8s
 => => extracting sha256:278d467c182fb935287ed6f4be3d44f8ac2714264bcb58b883d0cd257  0.0s
 => => extracting sha256:9b5f63cb30c69fe1a827c8fea9d33bd7026dffa193ed449ff44e1c98  12.5s
 => => extracting sha256:230542c909b8c810d61434d1f259307fac388dda9d2daca1aaf069c0b  0.7s
 => => extracting sha256:dc95f2a6ccee7fb934bd659ef134da3e3c71c2a4a8059fe3c79a7d230  0.0s
 => [2/5] WORKDIR /app                                                              0.4s
 => [3/5] RUN npm install -g npm                                                   26.3s
 => [4/5] RUN npm install -g json-server                                           15.3s
 => [5/5] COPY ./db.json /app                                                       0.0s
 => exporting to image                                                              2.3s
 => => exporting layers                                                             2.3s
 => => writing image sha256:3d2b1d82254a110ef24fb721d186902ba367f9e10a187fd27cfe5e  0.0s
 => => naming to registry.fly.io/dana096-json-server:deployment-01HNMDSAKBWA9B4MSH  0.0s
--> Building image done
==> Pushing image to fly
The push refers to repository [registry.fly.io/dana096-json-server]
dcd5aaa78b50: Pushed
136691a782ac: Pushed
0a378751f46c: Pushed
b2fb9bd5793d: Pushed
f6780a659019: Pushed
b0445205348c: Pushed
91d97cac4f7c: Pushed
e27cf0956124: Pushed
d43f876e6f21: Pushed
9f843c569746: Pushed
bcd354c940e1: Pushed
1dae5147cd29: Pushed
deployment-01HNMDSAKBWA9B4MSHPAHSEFQ5: digest: sha256:84b28624b21b54a3cc31258922b715be6f75f73a8725a1963dd1bd0b8b83c9f7 size: 2839
--> Pushing image done
image: registry.fly.io/dana096-json-server:deployment-01HNMDSAKBWA9B4MSHPAHSEFQ5
image size: 1.1 GB

Watch your deployment at https://fly.io/apps/dana096-json-server/monitoring

Provisioning ips for dana096-json-server
  Dedicated ipv6: 2a09:8280:1::15:f84a
  Shared ipv4: 66.241.124.60
  Add a dedicated ipv4 with: fly ips allocate-v4

This deployment will:
 * create 1 "app" machine

No machines in group app, launching a new machine

WARNING The app is not listening on the expected address and will not be reachable by fly-proxy.ine 32875161b50398 [app] update finished: success
You can fix this by configuring your app to listen on the following addresses:
  - 0.0.0.0:8080
Found these processes inside the machine with open listening sockets:
  PROCESS        | ADDRESSES
-----------------*---------------------------------------
  /.fly/hallpass | [fdaa:5:ca3a:a7b:22f:3af4:8d87:2]:22

Finished launching new machines
-------
NOTE: The machines for [app] have services with 'auto_stop_machines = true' that will be stopped when idling

-------
Checking DNS configuration for dana096-json-server.fly.dev

Visit your newly deployed app at https://dana096-json-server.fly.dev/
```

### DEPLY
```
$ fly deploy
```

### FROM
- https://www.npmjs.com/package/json-server
