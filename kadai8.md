ORG = imread('A.jpg'); % 画像の読み込み
ORG = rgb2gray(ORG); % グレースケールに変換
imagesc(ORG); colormap(gray); colorbar;  axis image; % 画像の表示

によって、原画像をグレースケールに変換した画像を読み込む。  
表示した結果を以下の結果に記す。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/8-1.jpg?raw=true)
図1 グレースケール変換後

以下のようにして閾値128で二値化を行う

IMG = ORG > 128; % 閾値128で二値化
imagesc(IMG); colormap(gray); colorbar;  axis image; % 画像の表示

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/8-2.jpg?raw=true)  
図2 閾値128で二値化

以下のようにしてイメージ内の連結要素をラベル付けを行う

IMG = bwlabeln(IMG);
imagesc(IMG); colormap(jet); colorbar;  axis image; % 画像の表示

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/8-3.jpg?raw=true)
図3 ラベル
