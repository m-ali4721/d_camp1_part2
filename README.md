Command:
    docker ps

Description:
    Provides list of running containers

Output:
    CONTAINER ID   IMAGE        COMMAND            CREATED        STATUS        PORTS                                       NAMES
f4cc2ccc8fe7   assignment   "python3 app.py"   28 hours ago   Up 28 hours   0.0.0.0:8000->8000/tcp, :::8000->8000/tcp   Assignment_1

-----------------------------------------------------------------------------------------------------------------------------------

Command:
    docker logs f4cc2ccc8fe7
Description:
    Provide logs of given container depicting the actions taken and current state
Output:
* Serving Flask app 'app'
 * Debug mode: off
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on all addresses (0.0.0.0)
 * Running on http://127.0.0.1:8000
 * Running on http://172.17.0.2:8000

 -----------------------------------------------------------------------------------------------------------------------------------

 Command:
    docker inspect f4cc2ccc8fe7
Description:
    Provides all the details/information on given image/container within the scope of Docker ranging from name to networking etc.
Output: 
[
    {
        "Id": "f4cc2ccc8fe76f629a50103ebc557346d6141abb4a6b6f412670cee62014b0fe",
        "Created": "2024-01-15T14:29:06.683527613Z",
        "Path": "python3",
        "Args": [
            "app.py"
        ],
        "State": {
            "Status": "running",
            "Running": true,
            "Paused": false,
            "Restarting": false,
            "OOMKilled": false,
            "Dead": false,
            "Pid": 23956,
            "ExitCode": 0,
            "Error": "",
            "StartedAt": "2024-01-15T14:29:08.002155976Z",
            "FinishedAt": "0001-01-01T00:00:00Z"
        },
        "Image": "sha256:2e576734f83aadc621c8e0bc4d181924c44a8329866be7cda4662b2738fa12ed",
        "ResolvConfPath": "/var/snap/docker/common/var-lib-docker/containers/f4cc2ccc8fe76f629a50103ebc557346d6141abb4a6b6f412670cee62014b0fe/resolv.conf",
        "HostnamePath": "/var/snap/docker/common/var-lib-docker/containers/f4cc2ccc8fe76f629a50103ebc557346d6141abb4a6b6f412670cee62014b0fe/hostname",
        "HostsPath": "/var/snap/docker/common/var-lib-docker/containers/f4cc2ccc8fe76f629a50103ebc557346d6141abb4a6b6f412670cee62014b0fe/hosts",
        "LogPath": "/var/snap/docker/common/var-lib-docker/containers/f4cc2ccc8fe76f629a50103ebc557346d6141abb4a6b6f412670cee62014b0fe/f4cc2ccc8fe76f629a50103ebc557346d6141abb4a6b6f412670cee62014b0fe-json.log",
        "Name": "/Assignment_1",
        "RestartCount": 0,
        "Driver": "overlay2",
        "Platform": "linux",
        "MountLabel": "",
        "ProcessLabel": "",
        "AppArmorProfile": "docker-default",
        "ExecIDs": null,
        "HostConfig": {
            "Binds": null,
            "ContainerIDFile": "",
            "LogConfig": {
                "Type": "json-file",
                "Config": {}
            },
            "NetworkMode": "default",
            "PortBindings": {
                "8000/tcp": [
                    {
                        "HostIp": "",
                        "HostPort": "8000"
                    }
                ]
            },
            "RestartPolicy": {
                "Name": "no",
                "MaximumRetryCount": 0
            },
            "AutoRemove": false,
            "VolumeDriver": "",
            "VolumesFrom": null,
            "CapAdd": null,
            "CapDrop": null,
            "CgroupnsMode": "private",
            "Dns": [],
            "DnsOptions": [],
            "DnsSearch": [],
            "ExtraHosts": null,
            "GroupAdd": null,
            "IpcMode": "private",
            "Cgroup": "",
            "Links": null,
            "OomScoreAdj": 0,
            "PidMode": "",
            "Privileged": false,
            "PublishAllPorts": false,
            "ReadonlyRootfs": false,
            "SecurityOpt": null,
            "UTSMode": "",
            "UsernsMode": "",
            "ShmSize": 67108864,
            "Runtime": "runc",
            "ConsoleSize": [
                0,
                0
            ],
            "Isolation": "",
            "CpuShares": 0,
            "Memory": 0,
            "NanoCpus": 0,
            "CgroupParent": "",
            "BlkioWeight": 0,
            "BlkioWeightDevice": [],
            "BlkioDeviceReadBps": [],
            "BlkioDeviceWriteBps": [],
            "BlkioDeviceReadIOps": [],
            "BlkioDeviceWriteIOps": [],
            "CpuPeriod": 0,
            "CpuQuota": 0,
            "CpuRealtimePeriod": 0,
            "CpuRealtimeRuntime": 0,
            "CpusetCpus": "",
            "CpusetMems": "",
            "Devices": [],
            "DeviceCgroupRules": null,
            "DeviceRequests": null,
            "KernelMemory": 0,
            "KernelMemoryTCP": 0,
            "MemoryReservation": 0,
            "MemorySwap": 0,
            "MemorySwappiness": null,
            "OomKillDisable": null,
            "PidsLimit": null,
            "Ulimits": null,
            "CpuCount": 0,
            "CpuPercent": 0,
            "IOMaximumIOps": 0,
            "IOMaximumBandwidth": 0,
            "MaskedPaths": [
                "/proc/asound",
                "/proc/acpi",
                "/proc/kcore",
                "/proc/keys",
                "/proc/latency_stats",
                "/proc/timer_list",
                "/proc/timer_stats",
                "/proc/sched_debug",
                "/proc/scsi",
                "/sys/firmware"
            ],
            "ReadonlyPaths": [
                "/proc/bus",
                "/proc/fs",
                "/proc/irq",
                "/proc/sys",
                "/proc/sysrq-trigger"
            ]
        },
        "GraphDriver": {
            "Data": {
                "LowerDir": "/var/snap/docker/common/var-lib-docker/overlay2/1e97cab45dc5a0d3c5858652f718262e8223a4ee4e2977eba4a6dc79b2b6aa5d-init/diff:/var/snap/docker/common/var-lib-docker/overlay2/rrsrqqonrvq4lvt40c81020u4/diff:/var/snap/docker/common/var-lib-docker/overlay2/ryo9yw0qax5unn16rj34h6eom/diff:/var/snap/docker/common/var-lib-docker/overlay2/f5e25f791fccd2aa16b58c32092cd0cdf2b110d4b75160cb969b634e05804119/diff:/var/snap/docker/common/var-lib-docker/overlay2/551a0a8dd41d93a420b2933973bbbc980194024a00c5472010b1d218f056e75f/diff:/var/snap/docker/common/var-lib-docker/overlay2/3c6ffc7d7488e1fd3467105391933e5a89c560c93566e3463e1f8c6c6c0735e4/diff:/var/snap/docker/common/var-lib-docker/overlay2/7ed578669003fb6f94dfebdeb4f3a369df6752fc10595b9c661a3530b97101de/diff:/var/snap/docker/common/var-lib-docker/overlay2/b3f34f6545c83f41acc484f6fb8d887bda1067f12f50a02e1633d14dcbc16b3c/diff",
                "MergedDir": "/var/snap/docker/common/var-lib-docker/overlay2/1e97cab45dc5a0d3c5858652f718262e8223a4ee4e2977eba4a6dc79b2b6aa5d/merged",
                "UpperDir": "/var/snap/docker/common/var-lib-docker/overlay2/1e97cab45dc5a0d3c5858652f718262e8223a4ee4e2977eba4a6dc79b2b6aa5d/diff",
                "WorkDir": "/var/snap/docker/common/var-lib-docker/overlay2/1e97cab45dc5a0d3c5858652f718262e8223a4ee4e2977eba4a6dc79b2b6aa5d/work"
            },
            "Name": "overlay2"
        },
        "Mounts": [],
        "Config": {
            "Hostname": "f4cc2ccc8fe7",
            "Domainname": "",
            "User": "",
            "AttachStdin": false,
            "AttachStdout": false,
            "AttachStderr": false,
            "ExposedPorts": {
                "8000/tcp": {}
            },
            "Tty": false,
            "OpenStdin": true,
            "StdinOnce": false,
            "Env": [
                "PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin",
                "LANG=C.UTF-8",
                "GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568",
                "PYTHON_VERSION=3.9.18",
                "PYTHON_PIP_VERSION=23.0.1",
                "PYTHON_SETUPTOOLS_VERSION=58.1.0",
                "PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4cfa4081d27285bda1220a62a5ebf5b4bd749cdb/public/get-pip.py",
                "PYTHON_GET_PIP_SHA256=9cc01665956d22b3bf057ae8287b035827bfd895da235bcea200ab3b811790b6"
            ],
            "Cmd": [
                "python3",
                "app.py"
            ],
            "Image": "assignment",
            "Volumes": null,
            "WorkingDir": "",
            "Entrypoint": null,
            "OnBuild": null,
            "Labels": {}
        },
        "NetworkSettings": {
            "Bridge": "",
            "SandboxID": "4a07a8b7b98e8d006c9f23c532970a0f85043206c69ec055ab16c64cb12f109d",
            "HairpinMode": false,
            "LinkLocalIPv6Address": "",
            "LinkLocalIPv6PrefixLen": 0,
            "Ports": {
                "8000/tcp": [
                    {
                        "HostIp": "0.0.0.0",
                        "HostPort": "8000"
                    },
                    {
                        "HostIp": "::",
                        "HostPort": "8000"
                    }
                ]
            },
            "SandboxKey": "/run/snap.docker/netns/4a07a8b7b98e",
            "SecondaryIPAddresses": null,
            "SecondaryIPv6Addresses": null,
            "EndpointID": "4d1d339a8dde20ec33044f9c510915e7eb36507c1d955f61aa2b25805144b37b",
            "Gateway": "172.17.0.1",
            "GlobalIPv6Address": "",
            "GlobalIPv6PrefixLen": 0,
            "IPAddress": "172.17.0.2",
            "IPPrefixLen": 16,
            "IPv6Gateway": "",
            "MacAddress": "02:42:ac:11:00:02",
            "Networks": {
                "bridge": {
                    "IPAMConfig": null,
                    "Links": null,
                    "Aliases": null,
                    "NetworkID": "022dfcd0bd5ee447a3b95fc3d0fb81eeb087e207b741b77e3eceafde22bbef04",
                    "EndpointID": "4d1d339a8dde20ec33044f9c510915e7eb36507c1d955f61aa2b25805144b37b",
                    "Gateway": "172.17.0.1",
                    "IPAddress": "172.17.0.2",
                    "IPPrefixLen": 16,
                    "IPv6Gateway": "",
                    "GlobalIPv6Address": "",
                    "GlobalIPv6PrefixLen": 0,
                    "MacAddress": "02:42:ac:11:00:02",
                    "DriverOpts": null
                }
            }
        }
    }
]
------------------------------------------------------------------------------------------------------------------------------

Command:
    docker exec -it Assignment_1 sh 
Description:
    Allows to run commands within Container by opening a new shell

-----------------------------------------------------------------------------------------------------------------------------

Command:
    docker attach Assignment_1
Description:
    Allows to interact with running container by connecting to running container

-------------------------------------------------------------------------------------------------------------------------------

Command:
    docker stop f4cc2ccc8fe7
Description:
    Stops a running container
Output:
    It has stopped a previously running container

---------------------------------------------------------------------------------------------------------------------------------

Command:
    docker commit Assignment_1 new_image:latest
Description:
    Allows to make changes in a running container and commit changes to a new image
Output:
REPOSITORY           TAG       IMAGE ID       CREATED         SIZE
new_image            latest    e0433ec621ae   6 seconds ago   135MB

----------------------------------------------------------------------------------------------------------------------------------

Command:
    docker stats Assignment_1
Description:
    It depicts the details of usage by the container/resource
Output:
CONTAINER ID   IMAGE        COMMAND            CREATED        STATUS         PORTS                                       NAMES
f4cc2ccc8fe7   assignment   "python3 app.py"   29 hours ago   Up 3 seconds   0.0.0.0:8000->8000/tcp, :::8000->8000/tcp   Assignment_1
CONTAINER ID   NAME           CPU %     MEM USAGE / LIMIT     MEM %     NET I/O       BLOCK I/O   PIDS
f4cc2ccc8fe7   Assignment_1   0.02%     18.12MiB / 15.23GiB   0.12%     6.74kB / 0B   0B / 0B     1

----------------------------------------------------------------------------------------------------------------------------------

Command:
    docker top Assignment_1
Description:
    Provides the processes being run for the given container
Output:UID                 PID                 PPID                C                   STIME               TTY                 TIME                CMD
root                32712               32691               0                   00:12               ?                   00:00:00            python3 app.py

-----------------------------------------------------------------------------------------------------------------------------------

Command:
    docker pause Assignment_1 
Description:
    Pauses the container temporarily rather than terminating it like done in docker stop 
Output:
CONTAINER ID   IMAGE        COMMAND            CREATED        STATUS                  PORTS                                       NAMES
f4cc2ccc8fe7   assignment   "python3 app.py"   29 hours ago   Up 8 minutes (Paused)   0.0.0.0:8000->8000/tcp, :::8000->8000/tcp   Assignment_1

------------------------------------------------------------------------------------------------------------------------------------

Command:
    docker unpause Assignment_1 
Description:
    Unpauses a paused container 
Output:
CONTAINER ID   IMAGE        COMMAND            CREATED        STATUS          PORTS                                       NAMES
f4cc2ccc8fe7   assignment   "python3 app.py"   29 hours ago   Up 10 minutes   0.0.0.0:8000->8000/tcp, :::8000->8000/tcp   Assignment_1

------------------------------------------------------------------------------------------------------------------------------------

Command:
    docker start Assignment_1 
Description:
    It starts an earlier stopped container 

--------------------------------------------------------------------------------------------------------------------------------------

Command:
    docker rename Assignment_1 Assignment_rename_1 
Description:
    It allows to change the name of a container 
Output:
CONTAINER ID   IMAGE        COMMAND            CREATED        STATUS          PORTS                                       NAMES
f4cc2ccc8fe7   assignment   "python3 app.py"   29 hours ago   Up 14 minutes   0.0.0.0:8000->8000/tcp, :::8000->8000/tcp   Assignment_rename_1

------------------------------------------------------------------------------------------------------------------------------------------

Command:
    docker wait Assignment_rename_1 
Description:
    Block until one or more containers stop, then print their exit codes
Output:
docker wait Assignment_rename_1
137

-------------------------------------------------------------------------------------------------------------------------------------

Command: 
    docker port f4cc2ccc8fe7
Description:
        List port mappings or a specific mapping for the container
Output:
    8000/tcp -> 0.0.0.0:8000
8000/tcp -> [::]:8000

--------------------------------------------------------------------------------------------------------------------------------------
Command:
    docker restart f4cc2ccc8fe7
Description:
    Restarts a running container 
Output:
f4cc2ccc8fe7   assignment   "python3 app.py"   29 hours ago   Up 3 seconds   0.0.0.0:8000->8000/tcp, :::8000->8000/tcp   Assignment_rename_1

---------------------------------------------------------------------------------------------------------------------------------------

Command:
     docker update --cpu-shares 512 f4cc2ccc8fe7

Description:
    The docker update command dynamically updates container configuration. You can use this command to prevent containers from consuming too many resources from their Docker host. 

-----------------------------------------------------------------------------------------------------------------------------------------       




