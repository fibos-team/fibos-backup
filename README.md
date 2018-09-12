# eosstore-backup

Fibos mainnet data backup

In order to ensure the security of the mainnet, we made regular backup of the data.We backup data once a day,and include blocks and state.

We can get the data from [fibos-backup-address](http://fibos.team/)

os:Ubuntu16.04

The snapshot only be used to compile version and Ubuntu

Put the data at your bp's data-dir

1.Get latest data with 

```
wget https://s3-ap-northeast-1.amazonaws.com/eosstorebp/xxx.tar.gz
```

2.then tar the xxx.tar.gz

```
tar -zxvf xxx.tar.gz
```

3.we can see one folder called **liuqiangdong_SYNC_Dir** (liuqiangdong is the BP name of FIBOSTEAM)

```
ubuntu@liuqiangdong:~/workspace/fibos-team/liuqiangdong_Dir$ ll
total 32
drwxrwxrwx 4 liuqiangdong liuqiangdong  4096 Sep 11 03:19 ./
drwxrwxr-x 7 liuqiangdong liuqiangdong  4096 Sep 12 22:25 ../
drwxrwxrwx 3 liuqiangdong liuqiangdong  4096 Sep 11 03:19 blocks/
-rw-rw-rw- 1 liuqiangdong liuqiangdong 13868 Sep 11 03:19 config.ini
drwxrwxrwx 2 liuqiangdong liuqiangdong  4096 Sep 12 22:24 state/
```

4.start your fibos bp node
