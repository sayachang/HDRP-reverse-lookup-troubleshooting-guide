# HDRP-reverse-lookup-troubleshooting-guide
逆引き！HDRPトラブルシューティングガイド

![HDRP image](https://raw.githubusercontent.com/sayachang/HDRP-reverse-lookup-troubleshooting-guide/master/images/HDRP%20image.png "HDRP image")

UnityのHDRPでなんか困った時に見ると役に立つかもしれない逆引き集です。

## もくじ  

1. モデルキャラが緑になってるんだけど
2. 透明にしたいけど光を反射してしまう
3. 画面が真っ黒/真っ白だけどどう戻せばいいのかわからない
4. 別のシーンでライトや明るさを変えてからシーンを開いたら以前に調整した明るさが変わってしまった
5. HDRPについて日本語で読める技術ドキュメントやブログが少ないんですけど
6. ここに困りごとを書きます


### 1. モデルキャラが緑になってるんだけど  

![100_green_mesh.png](https://raw.githubusercontent.com/sayachang/HDRP-reverse-lookup-troubleshooting-guide/master/images/100_green_mesh.png "100_green_mesh.png")

とてもいい質問だね！

HDRPで不自然な緑が見えるなら、典型的なケースは「キャラクターモデルでSSSのディフュージョンプロフィールが未登録」の場合だ。

![101_fix_it_diffusion_profile.png](https://raw.githubusercontent.com/sayachang/HDRP-reverse-lookup-troubleshooting-guide/master/images/101_fix_it_diffusion_profile "101_fix_it_diffusion_profile.png")

該当のメッシュを探して、シェーダーの中を覗いてみよう。「Fix」というボタンが出ていたらそれを押すと良い。

ディフュージョンプロフィールがHDRPクォリティアセットファイルに登録され、SSSが正しく表示されるようになる。

![102_hdrp_quality_asset.png](https://raw.githubusercontent.com/sayachang/HDRP-reverse-lookup-troubleshooting-guide/master/images/102_hdrp_quality_asset "102_hdrp_quality_asset.png")

### 2. 透明にしたいけど光を反射してしまう  

### 3. 画面が真っ黒/真っ白だけどどう戻せばいいのかわからない  

### 4. 別のシーンでライトや明るさを変えてからシーンを開いたら以前に調整した明るさが変わってしまった  

### 5. HDRPについて日本語で読める技術ドキュメントやブログが少ないんですけど  

### 6. TODO: ここに困りごとを書きます  


© UTJ/UCL
