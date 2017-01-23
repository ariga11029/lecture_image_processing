ORG=imread('0.jpg'); % 原画像の入力
ORG = rgb2gray(ORG); % グレースケールに変換
imagesc(ORG); colormap(gray); colorbar;  axis image; % 画像の表示

によって、原画像をグレースケールに変換した画像を読み込む。  
表示した結果を以下の結果に記す。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/4-1.jpg?raw=true)
図1 グレースケール変換後

以下のようにしてヒストグラムを表示する。

imhist(ORG); % ヒストグラムの表示
![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/4-2.jpg?raw=true)
図2 ヒストグラム
