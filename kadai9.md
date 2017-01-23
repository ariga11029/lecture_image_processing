ORG = imread('0.jpg'); % 画像の読み込み
ORG = rgb2gray(ORG); % グレースケールに変換
imagesc(ORG); colormap(gray); colorbar;  axis image; % 画像の表示

によって、原画像をグレースケールに変換した画像を読み込む。  
表示した結果を以下の結果に記す。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/9-1.jpg?raw=true)
図1 グレースケール変換後

以下のようにして読み込んだ画像にノイズを添付する。

ORG = imnoise(ORG,'salt & pepper',0.02); % ノイズ添付
imagesc(ORG); colormap(gray); colorbar;  axis image; % 画像の表示

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/9-2.jpg?raw=true) 
図2 ノイズ添付

ノイズを添付した画像を平滑化フィルタでノイズ除去を行う

IMG = bwlabeln(IMG);
imagesc(IMG); colormap(jet); colorbar;  axis image; % 画像の表示

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/9-3.jpg?raw=true)
図3 平滑化フィルタ

次にノイズを添付した画像をメディアンフィルタでノイズ除去を行う

IMG = bwlabeln(IMG);
imagesc(IMG); colormap(jet); colorbar;  axis image; % 画像の表示

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/9-4.jpg?raw=true)
図4 メディアンフィルタ

さらにメディアンフィルタでノイズ除去を行った画像にフィルタをかけて先鋭化する

f=[0,-1,0;-1,5,-1;0,-1,0]; % フィルタの設計
IMG = filter2(f,IMG,'same'); % フィルタの適用
imagesc(IMG); colormap(gray); colorbar;  axis image; % 画像の表示

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/9-5.jpg?raw=true)
図5 フィルタ
