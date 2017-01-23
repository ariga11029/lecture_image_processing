ORG = imread('0.jpg'); % 画像の読み込み
ORG = rgb2gray(ORG); % グレースケールに変換
imagesc(ORG); colormap(gray); colorbar;  axis image; % 画像の表示

によって、原画像をグレースケールに変換した画像を読み込む。  
表示した結果を以下の結果に記す。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/10-1.jpg?raw=true)
図1 グレースケール変換後

プレウィット法を用いてエッジ抽出を行う。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/10-2.jpg?raw=true)
図2 プレウィット法

ソベル法を用いてエッジ抽出を行う。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/10-3.jpg?raw=true)
図3 ソベル法

キャニー法を用いてエッジ抽出を行う。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/10-4.jpg?raw=true)
図4 キャニー法
