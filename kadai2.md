2階調，4階調，8階調での画像の表示を行い，それによる移り変わり，及び階調特性による擬似輪郭を確認する．  
まず始めに原画像の入力，原画像をグレースケール画像に変換し，表示を行う．

ORG=imread(0.jpg); % 原画像の入力  
ORG = rgb2gray(ORG); colormap(gray); colorbar; % グレースケール画像へ変換  
imagesc(ORG); axis image; % 画像の表示  

結果を図1に示す．

![原画像](https://github.com/ariga11029/lecture_image_processing/image/0-1.jpg?raw=true)  
図1 グレースケールに変換した原画像


グレースケール画像は8ビットの画像であり，濃淡を2の8乗，つまり256階調で表している．  
これを2階調の画像にするには，256階調に対し基準となる値を設けることで階調を2つに分ければ良い．  
今回は128を境に分けている．  
2階調画像の生成は次のように行う．

IMG = ORG>128;
imagesc(IMG); colormap(gray); colorbar;  axis image;

結果を図2に示す．

![原画像](https://github.com/ariga11029/lecture_image_processing/image/0-2.jpg?raw=true)  
図2 2階調画像
同様に
