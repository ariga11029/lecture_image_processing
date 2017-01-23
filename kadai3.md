ORG=imread('0.jpg'); % 原画像の入力
ORG= rgb2gray(ORG); % カラー画像を白黒濃淡画像へ変換
imagesc(ORG); colormap(gray); colorbar; % 画像の表示
````
によって、原画像をグレースケールに変換した画像を読み込む。  
表示した結果を以下の結果に記す。  
(https://github.com/ariga11029/lecture_image_processing/blob/master/image/3-1.jpg?raw=true)
図1 グレースケール変換後

閾値を以下のように処理する。。
````
IMG = ORG > A; % 輝度値がA以上の画素を1，その他を0に変換
imagesc(IMG); colormap(gray); colorbar;  axis image; 
````

閾値64とした場合。  
(https://github.com/ariga11029/lecture_image_processing/blob/master/image/3-2.jpg?raw=true)
図2 閾値64

閾値96とした場合。  
(https://github.com/ariga11029/lecture_image_processing/blob/master/image/3-3.jpg?raw=true)
図3 閾値96

閾値128とした場合。  
(https://github.com/ariga11029/lecture_image_processing/blob/master/image/3-4.jpg?raw=true)
図4 閾値128

閾値192とした場合。  
(https://github.com/ariga11029/lecture_image_processing/blob/master/image/3-5.jpg?raw=true)
図5 閾値192
