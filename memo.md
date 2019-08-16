## 本番用プロジェクト準備
- [] `choreonoid/ext/WRS2019/`に`choreonoid/sample/WRS2018/TNK/TS*.cnoid`をコピー
- [] マップのパスを確認(`WRS2019/TS1.cnoid`など)

## QRコード
- [] `roslaunch wrs_tnk_bringup qr_detector.launch namespace:=hogehoge`
- [] `rostopic echo /qr_codes`

## PCD保存
- [] `source wrs_tnk_bringup/scripts/pcl_saver.bash`
- [] 見るときは `pcl_viewer hoge.pcd`
