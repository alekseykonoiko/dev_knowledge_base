Download files from Linode
```bash
python linode_storage.py --type d lF1aihMfi9FwFajzKIXT8rI1f3o9kOHlkByigZx2 models/dataset_v3_zones1.zip datasets_v3_zones1.zip
```
```bash
python linode_storage.py --type d lF1aihMfi9FwFajzKIXT8rI1f3o9kOHlkByigZx2 lossles_cut_data.zip lossles_cut_data.zip
```
```bash
python linode_storage.py --type d lF1aihMfi9FwFajzKIXT8rI1f3o9kOHlkByigZx2 code_1.72.2-1665614327_amd64.deb code_1.72.2-1665614327_amd64.deb
```
```bash
sudo apt install code_1.72.2-1665614327_amd64.deb
```
To count number of files in folder
```bash
ls -1q lossles_cut_imgs/kampf5_220808/* | wc -l
```
To process all pic and vids and label them
```bash
python gen_zones_and_lbl.py --mach kampf6_t4 --src lossles_cut_data/kampf6_type4 --dst lossles_cut_imgs/kampf6_type4
```
```bash
zip -r lossles_cut_imgs.zip lossles_cut_imgs
```
Uploading generated and labeled images to Linode
```bash
python linode_storage.py --type u --key lF1aihMfi9FwFajzKIXT8rI1f3o9kOHlkByigZx2 --file dataset_v4_zones/dataset_v4_zones.pkl --obj_key dataset_v4_zones.pkl
```