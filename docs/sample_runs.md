## Sample Run for Cassandra Launcher

    Using configuration file: /root/.clusterlauncher.conf

    Welcome to DataStax' Cassandra Cluster Launcher!
        The easiest way to get Apache Cassandra up and running in Amazon's EC2
        in under 5 minutes!

    No existing clusters currently running!

    Cluster Name: Test Cluster
    Total Nodes: 4
    Version:
      [0] Community
      [1] Enterprise
    1

    Confirming credentials...
    Realtime (Non-Analytic) Nodes: 2
    CFS Replication Factor: 1

    Starting an EC2 cluster of type m1.large with image ami-fd23ec94...
    Ensuring DataStax pem key exists on AWS...
    Ensuring DataStax pem key exists on filesystem...
    Ensuring DataStax pem key's permissions are acceptable...
    Configuring ports...
    Launching cluster...
    Waiting for EC2 cluster to instantiate...
        Nodes that have been allocated by EC2:
            Node 0
            Node 1
            Node 2
            Node 3

    Cluster booted successfully!
        Elapsed Time: 1 minutes 17 seconds

    OpsCenter Address:
    http://107.20.59.116:8888
    Note: You must wait 60 seconds after Cassandra becomes active to access OpsCenter.

    Waiting 10 seconds for EC2 instances to warm up...
    Priming connections...
    The authenticity of host '107.20.59.116 (107.20.59.116)' can't be established.
    RSA key fingerprint is 8c:6a:e6:db:7e:0b:4b:f9:cc:bf:0b:16:a8:89:f2:35.
    Are you sure you want to continue connecting (yes/no/all)? all
    Creating a keyless SSH ring...

    Primed Connection Strings:
    ssh -i /root/.ssh/DataStaxLauncher.pem -o UserKnownHostsFile=/root/.ssh/ds_known_hosts ubuntu@107.20.59.116
    ssh -i /root/.ssh/DataStaxLauncher.pem -o UserKnownHostsFile=/root/.ssh/ds_known_hosts ubuntu@50.17.117.133
    ssh -i /root/.ssh/DataStaxLauncher.pem -o UserKnownHostsFile=/root/.ssh/ds_known_hosts ubuntu@23.20.38.109
    ssh -i /root/.ssh/DataStaxLauncher.pem -o UserKnownHostsFile=/root/.ssh/ds_known_hosts ubuntu@107.20.115.228

    Installing DataStax SSH on the cluster...
    Setting up the hosts file for the cluster...
    Waiting for the agent tarball to be created (This can take up to 4 minutes)...
        If taking longer, ctrl-C and login to AMI to see error logs.
    Installing OpsCenter Agents...

    Total Elapsed Time: 3 minutes 22 seconds

    Choose the cluster to destroy (if you wish):
      [0] None
      [1] jcasares - DataStaxAMI Time: 02-22-12 18:06 Size: 4
    1

    Confirm you wish to terminate jcasares - DataStaxAMI Time: 02-22-12 18:06 Size: 4 by pressing 'y'.
    y

    Termination command complete.

## Sample Run for Plain Image Launcher

    host1:~ joaquin$ imagelauncher
    Using configuration file: /root/.clusterlauncher.conf

    Welcome to the Plain Image Launcher!
        The easiest way to interface with Amazon's EC2 and Rackspace's CloudServers
        and produce a plain instance (or cluster) in under 5 minutes!

    Choose your Cloud Testing Host: 
      [0] EC2
      [1] Rackspace
    1

    Choose your Cloud Command: 
      [0] Create
      [1] Destroy
    0

    Choose your Cluster Size: 3

    Choose your Testing Operating System: 
      [0] CentOS
      [1] Debian
      [2] Fedora
      [3] Ubuntu
    0

    Choose your Operating System Version: 
      [0] 5.4 (deprecated)
      [1] 5.5 (deprecated)
      [2] 5.6
      [3] 6.0
    2

    Starting a Rackspace cluster of flavor 4 with image 114...
    Launching cluster...
    Waiting for cluster...
        Nodes that have been allocated by Rackspace:
            Node 0
            Node 1
            Node 2

    Cluster booted successfully!
        Elapsed Time: 4 minutes 42 seconds


    ssh -o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no root@50.57.232.174
    ssh -o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no root@50.57.186.82
    ssh -o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no root@50.57.225.96

    Public IPs:
    50.57.232.174, 50.57.186.82, 50.57.225.96

    Private IPs:
    10.182.113.188, 10.182.113.192, 10.182.113.194

    Total Elapsed Time: 4 minutes 48 seconds



    host1:~ joaquin$ imagelauncher
    Using configuration file: /root/.clusterlauncher.conf

    Welcome to the Plain Image Launcher!
        The easiest way to interface with Amazon's EC2 and Rackspace's CloudServers
        and produce a plain instance (or cluster) in under 5 minutes!

    Choose your Cloud Testing Host: 
      [0] EC2
      [1] Rackspace
    1

    Choose your Cloud Command: 
      [0] Create
      [1] Destroy
    1

    Choose the cluster to destroy:
      [0] jcasares-Time-02-22-12-1822-CentOS-56-Size-3
    jcasares-Time-02-22-12-1822-CentOS-56-Size-3 automatically chosen.

    Confirm you wish to terminate jcasares-Time-02-22-12-1822-CentOS-56-Size-3 by pressing 'y'.
    y

    Termination command complete.

