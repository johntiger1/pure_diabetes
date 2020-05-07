# pure_diabetes
Repo for PURE diabetes project


Instructions for running the Jupyter notebook:
just make sure you do the following:

1. ssh chenj4@risctrlp1
2. bash
3. XDG_RUNTIME_DIR='' srun --nodelist=RICREATET1 --mem=16G -c 4 jupyter notebook --ip 0.0.0.0
4. http://ricreatet1:8888/tree WITH THE TOKEN GENERATED FROM SRUN

If ricreate1 is down then we could tunnel the traffic back to THIS RDP comp!
