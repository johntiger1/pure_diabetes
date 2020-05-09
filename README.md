# pure_diabetes
Repo for PURE diabetes project


Instructions for running the Jupyter notebook:
just make sure you do the following:

1. ssh chenj4@risctrlp1
2. bash
3. XDG_RUNTIME_DIR='' srun --nodelist=RICREATET1 --mem=16G -c 4 jupyter notebook --ip 0.0.0.0
4. http://ricreatet1:8888/tree WITH THE TOKEN GENERATED FROM SRUN

If ricreate1 is down then we could tunnel the traffic back to THIS RDP comp!

Actually, we can simply use a technical solution! We have knowledge of basic Unix networking and hostnames. Intro to unix, and setting up a unix environment is KEY! Therefore, the solution is straightforward: 

1. specify a specific server to run from (ex. lambda-server). You can check via `sinfo`
2. make sure to get the IP address.
3. Then connect normally.

Specifically:

1. getent hosts lambda-server => 192.168.200.250
2. Then, we simply do: `192.168.200.250:8888?token=$TOKEN` 
