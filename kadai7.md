ORG = imread('0.jpg'); % 画像の読み込み
ORG = rgb2gray(ORG); % グレースケールに変換
imagesc(ORG); colormap(gray); colorbar;  axis image; % 画像の表示

によって、原画像をグレースケールに変換した画像を読み込む。  
表示した結果を以下の結果に記す。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/7-1.jpg?raw=true) 
図1 グレースケール変換後

グレースケール後の濃度ヒストグラム  
![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/7-2.jpg?raw=true)
図2 グレースケール変換後

以下のようしてダイナミックレンジを0から255にする。

![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/7-3.jpg?raw=true) 
図3 実行結果

ダイナミックレンジ拡大後の濃度ヒストグラム  
![画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/7-4.jpg?raw=true)
図4 ダイナミックレンジ拡大後

ダイナミックレンジを拡大したことによってヒストグラムが変わった
