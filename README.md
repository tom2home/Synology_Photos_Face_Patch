# Synology_Photos_Face_Patch
Synology Photos Facial Recognition Patch

## Here is my Chinese blog to show how to patch
https://blog.jinlife.com/index.php/archives/49/
Someone is attacking the blog, so it might be down for a while.

1. This patch will ignore GPU and let DS918+ to have facial recognition function in Synology Photos
2. DS3615xs don't need this patch.
3. DS918+ might need this patch.

# Use it at your own risk, you might lose data with this patch.

1. Download libsynophoto-plugin-model.so and upload it to home folder in Synology
2. SSH connect to Synology and input below command to patch the file.
3. Please change 'jinlife' to your own account.
```bash
cp /volume1/homes/jinlife/libsynophoto-plugin-model.so /var/packages/SynologyPhotos/target/usr/lib/ 
```
