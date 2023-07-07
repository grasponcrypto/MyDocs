## Teku
````
cd /opt
wget [current url copied from https://github.com/ConsenSys/teku/releases]
tar -xvfz teku-[version].tar.gz
rm teku teku-[version].tar.gz #remove symlink and tarball which is no longer needed
ln -s teku-[version] teku
rm teku-[2 versions ago] #keeping previous version for easier rollback
sudo systemctl restart teku
tail -f /var/log/teku.log
````

## Besu
````
cd /opt
wget [current url copied from https://github.com/hyperledger/besu/releases]
tar -xvfz besu-[version].tar.gz
rm besu besu-[version].tar.gz #remove symlink and tarball which is no longer needed
ln -s besu-[version] besu
rm besu-[2 versions ago] #keeping previous version for easier rollback
sudo systemctl restart besu
tail -f /var/log/besu.log
````
