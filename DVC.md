To delete all files in linode storage recursivly
```bash
s3cmd rm --recursive --force s3://neuralvision/
```
### Initial setup
Install required packages
```bash
sudo apt-get install awscli
```

```bash
pip install s3cmd "dvc[all]"
```
Configure `s3cmd` and `awscli`
Initialize dvc
```bash
dvc init
dvc remote add linode s3://neuralvision/axon_s/
dvc remote modify linode endpointurl https://eu-central-1.linodeobjects.com
git status
git commit -m "Initialize DVC"
git push
```
Uploading new version of dataset to cloud storage
```bash
dvc add data/dataset_v4_1_zones
git commit -m "added images dataset"
git push
dvc push
```
Setting default remote
```bash
dvc remote default myremote
```
Retriving data from dvc remote storage
```bash
git clone
git pull
dvc pull data/data.xml
```

```cli
dvc list https://alekseykonoiko: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@github.com/alekseykonoiko/dvc_test data
```
