# rosaddress client & catkin source!!!!!!
## 本番用プロジェクト準備
- [ ] `choreonoid/ext/WRS2019/`に`choreonoid/sample/WRS2018/TNK/TS*.cnoid`をコピー
- [ ] マップのパスを確認(`WRS2019/TS1.cnoid`など)


## 起動するlaunch(操作用PC側)
- [ ] `choreonoid_joy DoubleArmV7.launch`
- [ ] `double_arm_tnk_description joint_state.launch`
- [ ] `double_arm_tnk_description mapping.launch`

## QRコード
- [ ] `roslaunch wrs_tnk_bringup qr_detector.launch namespace:=hogehoge`
- [ ] `rostopic echo /qr_codes`

## PCD保存
- [ ] `source wrs_tnk_bringup/scripts/pcl_saver.sh`
- [ ] 見るときは `pcl_viewer hoge.pcd`


## csvフォーマット
- QRコードの内容，場所

### 場所コード一覧
- 車両周辺
右側フロントバンパー前 : R-1
右側フロントタイヤ前 : R-2
右側タイヤ間 : R-3
右側リアタイヤ後 : R-4
右側リアバンパー後 : R-5
左側フロントバンパー前 : L-1
左側フロントタイヤ前 : L-2
左側タイヤ間 : L-3
左側リアタイヤ後 : L-4
左側リアバンパー後 : L-5

- 車外(車に付いているやつ)
側面 ：S-f,  S-r  （前, 後）
後部：R-r, R-c, R-l（右, 中,左）
ボンネット：B-r, B-c, B-l （右, 中,左） 
トランク：T-r, T-c, T-l    （右, 中,左）

- 車両内
左から(左，中央，右),　(前席，後席), (床, シート)の順に３文字で記述する
(L, C, R),(F, B),(F, S)の組み合わせ

- 要救助者
頭 : H
胴 : B
腕 : A
足 : L
