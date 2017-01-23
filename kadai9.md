ORG = imread('0.jpg'); % 画像の読み込み
ORG = rgb2gray(ORG); % グレースケールに変換
imagesc(ORG); colormap(gray); colorbar;  axis image; % 画像の表示

によって、原画像をグレースケールに変換した画像を読み込む。  
表示した結果を以下の結果に記す。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/9-1.jpg?raw=true)
図1 グレースケール変換後

読み込んだ画像にノイズを添付する。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/9-2.jpg?raw=true) 
図2 ノイズ添付

ノイズを添付した画像を平滑化フィルタでノイズ除去を行う

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/9-3.jpg?raw=true)
図3 平滑化フィルタ

次にノイズを添付した画像をメディアンフィルタでノイズ除去を行う

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/9-4.jpg?raw=true)
図4 メディアンフィルタ

さらにメディアンフィルタでノイズ除去を行った画像にフィルタをかけて先鋭化する

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/9-5.jpg?raw=true)
図5 フィルタ
