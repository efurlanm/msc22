# Connection to the SDumont

*Last edited: 2024-11-22*

This notebook is available at: <http://github.com/efurlanm/msc22/blob/main/docs-src/notebooks/connect.ipynb>

- Turn on the VPN first, using the system's network manager

Connect:


```bash
%%bash
ssh -Nf sd
ssh -T sd <<'EOF'
hostname
module load anaconda3
source /scratch/app/anaconda3/2020.11/etc/profile.d/conda.sh
conda activate --stack /scratch${HOME#/prj}/env01
syncthing --no-browser --gui-address=0.0.0.0:28863 > ~/28863.log 2>&1 &
cd ~/Sync
jupyter-lab --no-browser --port=35655 --ip=0.0.0.0 --NotebookApp.token="" > ~/35655.log 2>&1 &
EOF
ssh -NfTL 8385:localhost:28863 sd
ssh -NfTL 8889:localhost:35655 sd
```

    sdumont14


Access to JL and ST is done using the web browser and the addresses:
- JL: http://localhost:8889  
- ST: http://localhost:8385

Disconnect:


```bash
%%bash
ssh sd 'pkill -u ${USER} -f syncthing'
ssh sd 'pkill -u ${USER} -f jupyter'
ssh -O exit sd
pkill -f 8385:
pkill -f 8889:
```

- Turn off the VPN, using the system's network manager


```python

```
