# C-Practice

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
一、程式作業繳交注意事項
1. 作業遲交不計分。
2. 程式碼有抄襲者，任何一次抄襲，學期成績不及格。
二、程式作業撰寫規則，違反規則該次作業不予計分
1. 程式碼不得使用全域變數，亦即，宣告在 main外面的變數！
2. 程式碼不得使用 goto 指令。
3. 程式碼不得使用 system("pause") 功能。
4. 程式碼不得使用 非 C 語言的功能，如 C++ for (int i=0; i<x, i++) {}。
5. 作業上傳請繳交.c 檔，不得繳交 .cdp .zip .rar .7z .exe等不合法檔案！
三、課程注意事項
1. 跟助教、卓越小老師預約課後輔導時間，請準時，學校會派人來簽到。
2. 作業要跟助教討論除錯問題，請跟助教約時間，當面討論比較有效果。
3. 作業等相關問題可寄至助教信箱詢問。
4. 下列網站提供很好的查詢資源請同學使用。
http://www.cplusplus.com/reference/clibrary/
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 1
001. 計算總成績、平均
某一學生修國文、計算機概論、計算機程式設計三科，使用者輸入名字（一個char）、學號
（int）、三科成績(int)。
(1) 計算學生總成績、平均。
(2) 印出名字、學號、總成績、平均。
Input
K
905067
100
100
100
Output
Name:K
Id:905067
Total:300
Average:100
------------------------------------------------------------------------

Week 1
002. 一元二次方程式
一元二次方程式，aX^2 + bx + c = 0，輸入a, b, c, 求 方程式的兩個實根。
-------------
輸入說明
第一個數 a
第二個數 b
第三個數 c
---------------
輸出說明
第一個實根， x1 = ((-b)+sqrt(b*b-4*a*c))/(2*a)
第二個實根， x2 = ((-b)-sqrt(b*b-4*a*c))/(2*a)
須 #include <math.h>
x1, x2 輸出到小數點第一位 printf("%.1f",x1);
---------------
Input
1
-2
1
Output
1.0
1.0
------------------------------------------------------------------------
Week 1
003. 數值運算
分別輸入 num1 num2 求出兩數的 Sum,Difference,Product,Quotient。
Difference結果取絕對值，使用 double fabs(double);
須 #include <math.h>
結果須輸出到小數點第二位 printf("%.2f",x1);
輸入:
25
2
輸出:
Sum:27.00
Difference:23.00
第 2 頁
c10401.txt
Product:50.00
Quotinet:12.50
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 2
004
判斷基數偶數
輸入說明：
輸入一個整數
輸出說明：
輸出奇數或偶數
輸入範例:
3
6
輸出範例:
odd
even
---------------------------------------------------------------------
Week 2
005
請輸入五個數字，分別計算出平均數、變異數、標準差，
並精確到小數點後第二位(註，之後的小數捨去)。
平均數參考公式
μ=Σ(Xi)/N
變異數參考公式
Σ(Xi-μ)^2/N
標準差參考公式
(Σ(Xi-μ)^2/N)^(0.5)
例如：1 2 8 9 10
平均值:6.00 (1+2+8+9+10)/5.0 = 6.0
變異數:14.00 Σ(Xi-μ)^2=(1-6)^2+(2-6)^2+(8-6)^2+(9-6)^2+(10-6)^2
=25+16+4+9+16=70
700./5.0=14.0
標準差14^(0.5) = 3.74165
取兩位小數 = 3.74

---------------------------------------------------------------------
Week 2
006
A、B、C三本書價格及折扣表如下：
定價 1~10本 11~20本 21~30本 31本以上
A 380 原價 打9折 打8.5折 打8折
B 1200 原價 打9.5折 打8.5折 打8折
C 180 原價 打8.5折 打8 折 打7折
有一顧客欲購買A:ｘ本、B:ｙ本、C:ｚ本（ｘ、ｙ、ｚ為使用者輸入），請計算需花費多少
錢？
例如:
A購買6本 B購買12本 C購買30本
6*380+12*1200*0.95+30*180*0.8
=20280
範例輸入:
6
12
30
輸出範例:
20280
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 4
007. 最佳資費選擇
輸入每月網內、網外、市話、通話時間(秒)及網內、網外簡訊則數，求最佳資費。
費率如下表:
資費類型 183型 383型 983型
月租費 183元 383元 983元
優惠內容 月 租 費 可 抵 等 額 通 信 費
語音費率 網內 0.08 0.07 0.06
(元/秒) 網外 0.139 0.130 0.108
市話 0.135 0.121 0.101
(元/秒)
簡訊費率 網內 1.128 1.128 1.128
(元/則) 網外 1.483 1.483 1.483
---------------------------------
輸入說明

---------------
網內語音(秒)，整數
網外語音(秒)，整數
市話 (秒)，整數
網內簡訊數，整數
網內簡訊數，整數
---------------------------------
輸入說明
---------------------------------
最佳資費類型，(183, 383, 983)
最佳資費，到小數點第三位
---------------------------------
測試資料：(Test Case)
input
120
150
20
10
5
output
183
183.000
input
3000
4000
200
5
5
output
383
767.255
---------------------------------------------------------------------
Week 4
008.
請檢查輸入的三門課程是否衝堂
依序輸入課程編號(數字)、上課小時數(1-2小時)、上課時間(依小時數輸入上課時間, 星期
1-5, 第1-9節)
---------------------------------
輸入說明
---------------------------------
1001 (課程編號)
2 (2小時)
11 (星期1 第1節課)
59 (星期5 第9節課)
... (第二門課)
... (第三門課)
---------------------------------
輸出說明
---------------------------------
課程編號,課程編號,衝突時間
(課程編號輸出順序與輸入順序相同，即12,13,23)
(每次列出兩個衝突課程編號，一個衝突時間)
(若沒有衝突則輸出 correct)
---------------------------------
測試資料：
---------------------------------
input
1001
2
12
13
1002
2
13
21
1003
2
25
21
---------
output
1001,1002,13
1002,1003,21
---------------------------------
input
1001
1
21
1002
2
33
32
1003
2
45
46
---------
output
correct
---------------------------------------------------------------------
Week 4
009 判斷何種三角形
當三個邊長能夠構成三角形時，再判斷該三角形為鈍角、銳角或是直角三角形，其判別方法
如下：
1. 直角三角形：其中有兩個邊的平方和等於第三邊的平方。
2. 鈍角三角形：其中有兩個邊的平方和小於第三邊的平方。
3. 銳角三角形：任兩邊的平方和大於第三邊的平方。
輸入三個整數
輸出：顯示直角三角形(Right Triangle)、鈍角三角形(Obtuse Triangle)、
銳角三角形(Acute Triangle)或無法構成三角形(Not Triangle)。
此題必須寫一個運算的function
int compute(int a, int b, int c);
a, b, b 為三角形三個邊
回傳值
0:Not Triangle
1:Right Triangle
2:Obtuse Triangle
3:Acute Triangle
測試資料：
input
5 12 13
output
Right Triangle
input
3 4 5
output
Right Triangle
input
1 2 3
output
Not Triangle
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 05.
010. 請使用一個 while loop 和 function call
給定一些線段，求這些線段所覆蓋的長度，注意，重疊的部分只能算一次。
輸入說明 ：
第一列有一個正整數 n:
代表共有 n 組測試案例。
接下來每一組測試案例的第一列是一個整數 m
表示此測試案例有m個線段，
接著的m列每一列是一個線段的兩端點，
每一個端點是一個整數介於0~60000之間，
端點之間以一個空格區隔，線段個數不超過 5000。
起始端點小的先輸入。
此題不使用陣列。
輸出說明 ：
針對每一組測試案例，輸出其覆蓋的長度，每組測試案例輸出一列。
Input:
2 (共有2組次是案例)
2 (此組測試案例有2個線段)
0 1
2 3
3 (此組測試案例有3個線段)
0 20
10 30
40 50
Output:
2
40
Input:
3
3
10 111
150 3450
160 180
2
100 180
150 3333
1
150 150
Output:
3401
3233
0
--------------
Input:
1
2
150 320
160 190
Output:
170
-----------------------------------
Week 5
011.判斷何種三角形
當三個邊長能夠構成三角形時，再判斷該三角形為正三角形(Regular Triangle)、
等腰三角形(Isoscceles Triangle )、鈍角、銳角或是直角三角形，
其判別方法如下：
依序判斷是否為正三角形、直角三角形、等腰三角形。
若都沒有符合，再判斷是否為銳角或鈍角。
1. 直角三角形：短邊的平方和等於最長邊的平方。
2. 鈍角三角形：短邊的平方和小於最長邊的平方。其中有一個角大於90度。
3. 銳角三角形：短邊的平方和大於最長邊的平方。所有內角均為銳角，小於90度。
輸入說明
輸入數個三角形三個邊，直到 -1 停止輸入。
三個邊為三個整數。
scanf 用法請參考
http://www.cplusplus.com/reference/cstdio/scanf/
輸出說明
印出
直角三角形(Right Triangle)、
正三角形(Regular Triangle)、
等腰三角形(Isoscceles Triangle)、
鈍角三角形(Obtuse Triangle)、
銳角三角形(Acute Triangle)、
或無法構成三角形(Not a Triangle)。
input
4 12 13
5 12 13
1 2 3
3 4 5
2 2 2
2 2 3
-1
output
Obtuse Triangle
Right Triangle
Not a Triangle
Right Triangle
Regular Triangle
Isoscceles Triangle
input:
80 90 160
5 5 5
7 7 6
30 50 40
1 8 7
30 31 29
-1
Output:
Obtuse Triangle
Regular Triangle
Isoscceles Triangle
Right Triangle
Not a Triangle
Acute Triangle
----------------------------------------------
Week 6
012. 請使用 while loop, 不可使用 array, for loop
第一個輸入為選擇二種圖形:
1 三角形方尖方面向右邊
2 三角形方尖方面向左邊
第二個輸入意義為畫幾行
input
1 (第一種圖形，三角形尖方面向右邊)
5 (共 5 行)
註: 符號為 * 和 .
output
*....
**...
***..
****.
*****
----------------------------
input
2 (第二種圖形，三角形尖方面向左邊)
3 (共 5 行)
output
..*
.**
***
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 6
013. 停車費計算
假設某個停車場的費率是停車2小時以內，每半小時30元，未滿半小時部分以半小時計費。
超過2小時，但未滿4小時，每半小時40元，未滿半小時以半小時計費。
超過4小時以上的部份，每半小時60元，未滿半小時部分以半小時計費。
請撰寫程式計算輸入數筆資料，共需繳交的停車費。
本程式不考慮隔夜情況。
輸入說明：
輸入多組時間，每組分別為開始與離開時間，24小時制。
輸入 -1 停止輸入，若輸入格式錯誤，則顯示錯誤訊息。
輸出說明：
輸出總停車費。
input:
10:23
15:20
25:25
10:70
-1
output:
340
error

input:
10:23
13:20
21:25
25:70
-1
output:
200
error
------------------------------------------------------------------------------
Week 6
014. 請使用一個 while loop 和 function call
給予一個十進位整數，請撰寫一程式可以將此十進位整數轉換為指定的進制的整數。
輸入說明:
輸入分為兩部份，包括指定的進制數
(2 ~ 16)
與十進位整數(0 ~ 1000000000)
16 進位數字為 0 1 2 3 4 5 6 7 8 9 A B C D E F
輸出說明:
經轉換後的新進位制的整數( y )
input:
16 1234
output:
4D2
Input:
8 56456456
Output:
327272410
-----------------------
Input:
11 17489465
Output:
9966104
-----------------------
Input:
4 17489
Output:
10101101
--------------------------------------------------------------------------------
--
Week 6
015.
劃兩個"小組吉祥物"，在 800 X 600 視窗不斷移動，遇到邊界會回彈。
一個半徑30，第二個半徑60。
一個往右下角移動，另一個往右上角移動。
每移動一百步則[隨機]變換顏色。
每次呼叫 delay 重新畫圖，定義為一次移動。
參考以下可執行檔執行結果
https://youtu.be/fUZwgllNEho
，以及程式碼。
#include <graphics.h>
#include <stdlib.h>
#include <time.h>
#include <stdio.h>
#define RADIUS1 30
#define RADIUS2 60
#define STEP 10
#define DELAY_TIME 50
int main() {
srand(time(NULL));
initwindow(800,600);
draw(1,1,0,1);
getch();
closegraph( );
}
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 7
016. 最大質數
給定一個2～100,000之間的數字，找出該數字的子字串中最大的質數值。
子字串為原字串（長度n）中連續取k個字元所組合而成，1 ? k ? n。
輸入說明：
一個正整數，值介於2～100,000之間。
輸出說明：
若有，則輸出該數字的子字串中最大的質數值； 若無，請輸出”No prime found”
input:
97560
output:
97
-----------------------------------------
input:
50113
output:
5011
-----------------------------------------
input:
3413
output:
3413
------------------------------------------------------------
Week 7
017.回文結構數字
輸入兩整數，找出兩整數區間內所有具有回文結構的數字。
例如，輸入 80 100 ，則輸出為 88 99 。
例如，100 200 ，則輸出為 101 111 121 131 141 151 161 171 181 191 。若沒有則輸出
0 。
輸入說明：
輸入兩整數。
輸出說明：
輸出區間內所有具有回文結構的數字 。
input:
10 70
output:
11 22 33 44 55 66
-----------------------------------------
input:
1300 2000
output:
1331 1441 1551 1661 1771 1881 1991
-----------------------------------------
input:
17000 18000
output:
17071 17171 17271 17371 17471 17571 17671 17771 17871 17971
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 8
018.
輸入第一個整數，決定輸出圖形種類，
輸入第二個整數，決定輸出的行數。
空白以. 輸出。
..1
.121
12321
.121
..1
7531357
.53135
..313
...1
輸入說明：
每一組兩個數字，輸入-1結束所有輸入。
第一個正整數，1為菱形數字，2為三角形數字，其餘輸入均為不合法。
第二個正整數為行數 N， 第一種圖形合法輸入 N 為奇數，1<=N<=18，
第二種圖形合法輸入，1<=N<=5，其餘輸入均為不合法。
不合法輸入，則輸出 E。
輸出說明：
請參考範例輸出。
Sample Input1:
1,9
1,13
-1
Sample Output:
....1
...121
..12321
.1234321
123454321
.1234321
..12321
...121
....1
......1
.....121
....12321
...1234321
..123454321
.12345654321
1234567654321
.12345654321
..123454321
...1234321
....12321
.....121
......1
Sample Input2:
1,22
1,5
-1
Sample Output:
E
..1
.121
12321
.121
..1
Sample Input3:
2,5
2,4
2,2
2,12
-1
Sample Output:
975313579
.7531357
..53135
...313
....1
7531357
.53135
..313
...1
313
.1
E
-----------------------------------------------------------
Week 8
019.
計算矩形覆蓋的面積
輸入兩個矩形的對角兩點x、y座標
計算兩個矩形重疊的面積為多少
例如輸入
1 5 9 7
2 5 10 11
表示
一個矩形的有其中對角兩點為(1,5)與(9,7)
另一個矩形的有其中對角兩點為(2,5)與(10,11)
而重疊面積為(2,5)與(9,7)構成的矩形
所以面積為(9-2)*7(-5)=14
input:
1 5 9 7
2 5 10 11
output:
14
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 9
020
切割面積加總法公式
使用切割面積加總法公式，
T = (h/2)(f(p) + f(q) + 2 f(xi)) ,
h = (q-p)/n，h 是 double。
計算 f(x) 的面積，到小數點第五位四捨五入。
x 值從區間起始 p 到區間終點 q 的面積，
n 為 切割數，初始設定 n_(0)=2，每次 n_(j+1) = n_(j) + 1。
err為精確小數位數，例如 err=6，即 n_(j+1) 和 n_(j)兩次切割，
計算出的面積值的差小於 10 的負6次方，亦即小於 0.000001。
f1(x) =((a-x^2))^(1/2), a 為常數。 f2(x) = (ax^3 + 7x)/(a+x)^(1/2), a 為常數。
輸入說明：
輸入 1 代表計算 f1(x) 面積，輸入 2 代表計算 f2(x)面積，
接著依序，輸入 a, p, q, err，輸入0為停止輸入。
此題測試資料為連續輸入一至多筆資料。
---------------
Input:
1,4,-2,1,9,0
Output:
5.05481
--------------
Input:
2,1,0,3,9,0
Output:
29.75238
---------------
Input:
1,4,-2,1,9,2,1,0,3,9,0
Output:
5.05481
29.75238
---------------
Input:
2,5,1,2,9,0
Output:
11.37716
-------------------
Input:
2,5,-2,1,9,0
Output:
20.22714
-------------------
HINT
方程式可能會跑到 y<0的地方，此時要算面積，必須將y取絕對值。
若 err=3, Area_(j+1) 跟 Area_(j)的差小於 10負3次方
fabs(Area_(j+1)-Area_(j))*10*10*10<1
若以整數比較會好一點
int k=fabs(Area_(j+1)-Area_(j))*10*10*10*10;
if (k>10) {….}
面積差，為兩次計算出面積的差值(相減)。
數值分析的誤差是兩次面積計算的差值除以，前一次的面積值。
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 10
021
牛頓法解方程式 (Newton's method)
應用牛頓法解以下兩個方程式的根。
(Apply Newton's method) to solve the two equations).
x_(j+1) = x_j – f(x_j)/f'(x_j), (其中 f'(x) 是 f(x) 的一次微分)
f1(x) = x^n - cx^(n-2) – d, and (n>2), ( f1'(x) = nx^(n-1) – (n-2)cx^(n-3) )
f2(x) = x^n - cx – d, and (n>2), ( f2'(x) = nx^(n-1) – c。
(Hint: let x0 = d/2)
輸入說明:
第一個輸入 1 代表 f1，2 代表 f2。
第二個輸入代表 n。
第三個輸入代表 c。
第四個輸入代表 d。
第五個輸入代表 err，精確小數位數，例如err=6，
即兩次疊代差小於0.000001。
也就是說 x_(j+1) 與 x_j 相減小於 0.000001，10 的負6次方。
輸出說明:
一個方程式的根，顯示到小數點 err+1 位。
亦即，若err=6，則要顯示到小數點第七位。
使用去尾法，不需要四捨五入。
----------------
Input:
1 4 5 5 2
Output:
2.419
---------------
Input:
2 4 5 5 2
Output:
1.961
---------------
Input:
1 4 5 5 8
Output:
2.419525153
---------------
Input:
2 4 5 5 8
Output:
1.961673882
-----------------------------------------------------------------------------
Week 10
022.(此題不使用陣列)
寫一個 function 輸入 XY 座標系統的兩個座標 (x1, y1), (x2, y2)；
輸出兩個座標經過的 XY 方程式 y=mx+b;
m=(y1-y2)/(x1-x2)
b=(x2y1-x1y2)/(x2-x1)
void f1(int x1, int y1, int x2, int y2, double *m, double *b);
寫一個 function 輸入 XY 座標系統的兩個座標 (x1, y1), (x2, y2)；
輸出兩個座標經過的 XY 方程式 y=m1/m2x+b1/b2;
m1=(y1-y2), m2=(x1-x2),
b1=(x2y1-x1y2), b2/(x2-x1),
void f2(int x1, int y1, int x2, int y2, int *m1, int *m2, int *b1, int *b2);
輸入說明:
XY的兩個座標 x1, y1, x2, y2，均為整數。
輸出說明:
(1) y=mx+b,
m, b 計算至小數第二位。
(2) y=mx+b
m, b 以分數表達。
=>方程式有可能沒有 x 項，或沒有 y 項。
=>沒有 x 項則 y=b，沒有 y 項則 x = -b/m。
=>若m,b為整數，則使用整數表達。
-------------
input:
1 1 2 2
output:
y=x
y=x
-------------
input:
1 2 2 2
output:
y=2
y=2
-------------
input:
1 2 1 1
output:
x=1
x=1
-------------
input:
1 0 2 1
output:
y=x-1
y=x-1
-------------
input:
3 4 -3 0
output:
y=0.67x+2
y=2/3x+2
------------------------------------------------
Week 10
023. (此題不使用陣列，請參考第六章課本 case study)
分數 +, -, *, / 運算
輸入說明:
輸入三行，每一行代表一個分數
輸出說明:
輸出三組分數+, -, *, / 結果
先輸出第1,2個分數+, -, *, / 結果
在輸出第1,3個分數+, -, *, / 結果
最後輸出第2,3個分數+, -, *, / 結果
若有輸入分數的分母或分子為0，則相關四則運算均輸出ERROR。
若分數大於1，則分數部分要加括號。
----------------
Input
1/2
2/3
3/4
Output
1(1/6)
-1/6
1/3
3/4
1(1/4)
-1/4
3/8
2/3
1(5/12)
-1/12
1/2
8/9
------------
Input
0/2
4/5
2/3
Output
ERROR
ERROR
ERROR
ERROR
ERROR
ERROR
ERROR
ERROR
1(7/15)
2/15
8/15
1(1/5)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 11
024.
寫一個 function 輸入 N 組矩形 XY 座標中的兩個點，輸出 N 組矩形中的最大的周長和最
大的面積。
程式中必須使用以下 function 定義，計算一個矩形的周長與面積。
---------------------------------------
void compute(int x1, int y1, int x2, int y2, int *perimeter, int *area);
第一個點 (x1, y1)
第二個點 (x2, y2)
計算周長結果 *perimeter
計算面積結果 *area
-------------------------------------------
輸入幾組矩形的兩個點，輸入-1停止輸入。
輸出最大的面積和最大的周長。
------------------
輸入說明：
分別輸入幾組矩形的兩個點，
第一筆輸入第一個矩形兩個點，x1, y1, x2, y2，
換行再輸入第一個矩形兩個點，直到輸入 -1 停止。
---------------------
輸出說明：
輸出所有矩形中最大的面積和最大的周長。
input:
-10 -10 20 60
52 52 2 2
85 8 5 38
-1
output:
2500
220
--------------------------------------------------------------------------------
--------------
Week 11
025.
(此題不使用陣列，必須使用指標)
程式碼必須使用以下 function 定義，計算兩個分數的相加。
void add(int n1, int d1, int n2, int d2, int *numerator, int *denominator);
n1: 第一個數的分子
n1: 第一個數的分母
n1: 第二個數的分子
n1: 第二個數的分母
*numerator: 相加結果的分子
*deniminator: 相加結果的分母
程式碼必須使用以下 function 定義，計算兩個分數的相乘。
void mul();
int multiply(int n1, int d1, int n2, int d2, int *numerator, int *denominator);
n1: 第一個數的分子
n1: 第一個數的分母
n1: 第二個數的分子
n1: 第二個數的分母
*numerator: 相乘結果的分子
*deniminator: 相乘結果的分母
--------------------
輸入說明:
輸入二行，每一行代表一個分數
----------------
輸出說明:
輸出分數相加結果
輸出分數相乘結果
若有輸入分數的分母或分子為0，則輸出ERROR。
若分數大於1，則分數部分要加括號。
若為負數，負號在最前面。
----------------
Input
1/2
2/3
Output
1(1/6)
1/3
------------
Input
0/2
4/5
Output
ERROR
ERROR
--------------
Input
-1/2
4/5
Output
3/10
-2/5
---------
Input
-1/2
-4/5
Output
-1(3/10)
2/5
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 12
026.整數的交集聯集
請設計程式，利用兩個一維整數陣列儲存兩個正整數集合 A, B ，
兩個集合 A, B 的陣列大小為 20，正整數 1~100；
程式功能為：
(1) 新增集合元素：輸入一集合與一正整數，若新增的元素與該集合內元素有重複，
則無法新增。
(2) 刪除集合元素：輸入一集合與一正整數，若集合中無該元素，無法刪除。
(3) 計算集合是否空集合。
(4) 計算兩個集合的交集。
(5) 計算兩個集合的聯集。
(6) 計算集合是否為另一個集合的子集合。
------------------------------
輸入說明:
每一行第一數字輸入整數指令選項，意義如下:
0: 結束exit
1: 清空 A，輸出 A 和 B 的內容。
2: 清空 B，輸出 A 和 B 的內容。
3: 新增元素到 A，後面接一個正整數為要插入的元素，
輸出 A 和 B 的內容。
4: 新增元素到 B，後面接一個正整數為要新增的元素，
輸出 A 和 B 的內容。
5: 從 A 刪除一個元素，後面接一個正整數為要刪除的元素，
輸出 A 和 B 的內容。
6: 從 B 刪除一個元素，後面接一個正整數為要刪除的元素。
輸出 A 和 B 的內容。
7: 輸出 A, B 聯集。
8: 輸出 A, B 交集。
9: 輸出 A 是否為 B 的子集合，若是則輸出 1 ，否則輸出 0。
輸出說明:
輸出集合格式
集合名稱:[集合元素,集合元素,...]，中間沒有空白，
元素順序依照輸入先後順序。
交集與聯集的元素順序，先以A的元素順序再以B的元素順序。
每一指令輸出一行。
----------------
Input:
3 4
3 7
4 8
4 9
5 4
6 8
3 8
7
8
9
0
Output:
A:[4,]B:[]
A:[4,7,]B:[]
A:[4,7,]B:[8,]
A:[4,7,]B:[8,9,]
A:[7,]B:[8,9,]
A:[7,]B:[9,]
A:[7,8,]B:[9,]
[7,8,9,]
[]
0
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
Week 13
027. 撲克牌
撲克牌四種花色分別是黑桃、紅心、磚塊、梅花，定義 0~3。
撲克牌數字1~13，與四種花色共有52張牌。
編碼規則為數字+花色，例如 10 表示黑桃 A、72 表示磚塊 7，123 表示梅花 3。
撲克牌遊戲把單一張牌命名為單張，沒有任何花色牌型，編號 0。
兩張數字一樣的命名為 Pair，編號 1。
2 組 pair 的牌稱為 Two pair，編號 2。
三張一樣的稱為 Three of a Kind，編號 3。
Three of a Kind 加一個 Pair 稱為 Full House，編號 4。
四張一樣稱為 Four Of A Kind，編號 5。
數字連續的5張牌稱為 Straight，包括 13 ,1, 2, 3, 4也是，編號 6。
數字連續的5張且花色一樣稱為 Straight Flush，編號 7。
輸入5張撲克牌，判斷哪一類型的牌形編號(1~7)。
程式必須有以下function。
void judge(int data[], int *r);
data[0]~data[4]為輸入 5 張撲克牌，r 為哪一類型的牌形編號(1~7)。
輸入說明 ：
第一列輸入為5個整數分別由空格分開，表示5張撲克牌。
輸出說明 ：
輸出為一個1~7的整數，代表牌型編號，以指標變數傳出。
----------------------
Input
90 82 83 81 92
output
4
---------------
Input
120 110 130 20 10
output
7
---------------
Input
120 111 132 23 10
output
6
---------------
Input
100 101 12 23 10
output
2
---------------
Input
100 101 12 102 103
output
5
------------------------------------------------------------------
Week 13
028. 計算 N 邊形面積 (請參考課本 chapter 7, 習題二)
n 個點連成 n 邊形，n<=20，
點的座標為 (x_(0), y_(0)), (x_(1), y_(1)),....,(x_(n), y_(n))。
Area = fabs(sum)/2
sum = (x_(1)+x_(0))*(y_(1)-y_(0))+ ...
+ (x_(i+1)+x_(i))*(y_(i+1)-y_(i))+ ...
+ (x_(n)+x_(n-1))*(y_(n)-y_(n-1))
--------------------
輸入說明:
每兩個數字為一個座標，最後以-999結束，
數字中間以逗號隔開。
輸出說明:
計算多邊形面積求到小數第一位。
----------------------------------
input:
4,0,4,7.5,7,7.5,7,3,9,0,7,0,-999
---------------------------------
output:
25.5
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
week 14
029. 以陣列實做長整數的運算
將長整數儲存於一維陣列，長度為60位。
計算兩數的相加、相減、相乘。
輸入說明:
兩個小於60位數的數字
輸出說明
兩數的相加、相減、相乘結果
input:
186978448
484312244
output:
671290692
-297333796
90555951730517312
---------------------------------------------------------
Week 14.
030.
輸入說明
輸入一串未經排序的整數數字，數量小於20，結束時輸入-999
接著輸入數字0代表由小到大排序，輸入1代表由大到小排序。
輸出說明
利用Bubble Sort, Insertion Sort, Selection Sortn三種排序方法，
輸出排序完成的數字與三種排序所執行的交換次數。
input:
1 781 848 7 4 99 11 44 88 90 111 11 54 12 55 -999
0
output:
1 4 7 11 11 12 44 54 55 88 90 99 111 781 848
Bubble Sort change times = 48
Insertion Sort changed times = 48
Selection Sort changed times = 12
----------------------------------
input:
1 3 5 7 9 11 13 15 17 -999
1
output:
17 15 13 11 9 7 5 3 1
Bubble Sort change times = 36
Insertion Sort changed times = 36
Selection Sort changed times = 4
---------------------------------------------------------
Week 14.
031.
設一個 nxn 的矩陣，由左而右，由上而下標示自1到 nxn 的數，如下圖為 4x4的。
1 2 3 4
5 6 7 8
9 10 11 12
13 14 15 16
讀入旋轉序列後，將該矩陣的資料輸出。
下圖中，表示向右旋轉一次。
13 9 5 1
14 10 6 2
15 11 7 3
16 12 8 4
下圖表示將圖向左旋轉一次，
4 8 12 16
3 7 11 15
2 6 10 14
1 5 9 13
下圖表示將圖上下對翻一次。
13 14 15 16
9 10 11 12
5 6 7 8
1 2 3 4
------------------------------
輸入說明 ：
第一行是一個正整數 n, n<10，表示一個 nxn 的矩陣。
第二行是一個長度不超過80的字串，字串中R表示向右旋轉，L表示向左旋轉，
N表示上下對翻。
使用字元陣列(字串)說明
#include <string.h>
char s[90]; // 宣告字元陣列
int length=0;
gets(s); // 讀取字串
length = strlen(s);
------------------------------
輸出說明 ：
由左而右，由上而下，輸出經過旋轉後的排列。每筆測試資料共輸出 n 行，每行 n 個整
數，
每筆資料間以空行隔開。
------------------------------
Sample Input:
3
RRNRLLRLNRLLL
------------------------------
Sample output:
7 4 1
8 5 2
9 6 3
------------------------------
Sample Input:
2
RLLRNN
------------------------------
Sample output:
1 2
3 4
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
week 15
032.
中序轉後序
輸入一個由 operand 和 operator 組成的運算式字串。
operand 為 0~9，operator 為 + - * / ，* / 運算優先順序大於 + - 。
operator 在兩 operand 中間的表示方式為中序表示。
請將中序表示的運算式改成後序表示方式。
--------------------------------
輸入說明 ：
輸入為一行長度在512個字母內的字串，用中序表示法表達的算式。
中間有一個空白。
--------------------------------
輸出說明 ：
輸出後序表示的運算式。
中間有一個空白。
--------------------------------
Sample Input
9 + 8 * 7 - 6
Sample Output:
9 8 7 * + 6 -
--------------------------------------------------------------------------------
----------
week 15
033. 井字遊戲
----------------
輸入說明:
第 1 行:
輸入誰先下，1 代表 Computer，0 代表 Player。
第 2 行~第 N 行:
第 32 頁
c10401.txt
第一種情況:兩個 0, 1, 2 數字
分別輸入 Computer 和 Player 的座標，直到一方贏才停止。
第二種情況:
w: 輸出所有Computer可能贏的座標
d: 輸出 Computer 或 player 即將要贏，若沒有答案則輸出 no
座標位置如下:
00 | 01 | 02 |
--------------
10 | 11 | 12 |
--------------
20 | 21 | 22 |
--------------
------------------------------
輸出說明:
(1)
一旦有一方贏，要顯示是 Computer 或 Player贏。
若為 Computer 贏， 輸出 Computer win
若為 Player 贏， 輸出 Player win
(2)
有座標重複輸入時，輸出 input error
(3) 輸入 w
輸出所有Computer可能贏的座標
(4) 輸入 d
輸出誰即將贏與贏的座標
Computer will win with (x, y)
Player will win with (x, y)
-------------------
輸入範例說明
1 (Computer先下)
0 0
1 1
0 2
d (顯示誰即將贏)
0 2 (已重複，要輸出ERROR)
2 2
2 0
w (顯示所有Computer可能贏的座標)
1 0
0 1
----------------------
輸出範例說明
Computer will win with (0, 1) (Computer可能贏)
input error
Computer will win with (0, 1) (Computer可能贏的第一個座標)
Computer will win with (1, 0) (Computer可能贏的第二個座標)
Computer win
-------------------
Sample Input
1
0 0
1 1
0 2
d
0 2
2 2
2 0
w
1 0
0 1
-------------------
Sample Output
Computer will win with (0, 1)
input error
Computer will win with (0, 1)
Computer will win with (1, 0)
Computer win
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~
week 16
034.
數獨的規則
輸入一個9*9的數字矩陣，其中每個元素均為0～9，其中0代表該格尚未填入數字。
請撰寫一支程式判斷該矩陣中，0 應該出現甚麼數字。數獨的規則如下：
(1)矩陣中的每一列（9個元素）只能出現1~9至多各一次。
(2)矩陣中的每一行（9個元素）只能出現1~9至多各一次。
(3)9個3*3的小矩陣（9個元素），亦分別只能出現1~9至多各一次。
輸入說明 ：
9*9的數字矩陣，其中每個元素均為0～9, 0代表該格尚未填入數字.
輸出說明 ：
從上到下，從左到右，輸出 0 的位置與數字。
範例 ：
Sample Input:
023456789
456789123
789123456
231564897
564897231
897231564
312605978
645978312
908312645
Sample Output:
0 0 1
6 4 4
8 1 7
--------------------------------------------------------------------------------
----------
week 16
035.
檢查10*10五子棋可以構成5個連為一線的位置。
1表示有放棋子，0表示沒有放旗子。
----------------------------------
輸入說明
輸入10*10的資料
-----------------------------
輸出說明
可構成5個連為一線的位置。例如
0 0 0 0 0 0 0 0 1 0
0 0 0 0 0 0 1 1 0 0
0 0 0 0 0 0 1 0 0 0
0 0 0 0 0 0 1 1 1 1
0 0 0 0 1 0 1 0 0 0
0 0 0 0 0 0 0 0 0 0
0 0 0 1 0 0 0 0 0 0
0 0 0 1 0 0 0 0 0 0
0 0 1 1 1 1 0 0 0 0
0 0 0 1 0 0 0 0 0 0
可以增加5個連為一線，以下圖表示。
0 0 0 0 0 0 x 0 1 0
0 0 0 0 0 0 1 1 0 0
0 0 0 0 0 0 1 0 0 0
0 0 0 0 0 x 1 1 1 1
0 0 0 0 1 0 1 0 0 0
0 0 0 x 0 0 x 0 0 0
0 0 0 1 0 0 0 0 0 0
0 0 0 1 0 0 0 0 0 0
0 x 1 1 1 1 x 0 0 0
0 0 0 1 0 0 0 0 0 0
其位置為
0 6
3 5
5 3
5 6
8 1
8 6
---------------------
SampleInput:
0 0 0 0 0 0 0 0 1 0
0 0 0 0 0 0 1 1 0 0
0 0 0 0 0 0 1 0 0 0
0 0 0 0 0 0 1 1 1 1
0 0 0 0 1 0 1 0 0 0
0 0 0 1 0 0 0 0 0 0
0 0 0 1 0 0 0 0 0 0
0 0 0 1 0 0 0 0 0 0
0 0 1 1 1 1 1 0 0 0
0 0 0 1 0 0 0 0 0 0
Sample Output:
0 6
3 5
5 3
5 6
8 1
8 6

