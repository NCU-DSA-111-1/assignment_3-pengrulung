# 開源程式的使用

Data Structure Assignment4

109503510_通訊三_龍芃如


使用Arithmetic coding和Huffman coding的開源程式

## Arithmetic coding

* 一種壓縮演算法

* 將一段 message 用 0 到 1 間的區間來表示

* Rissanen於1979年提出的一種壓縮方法

## Huffman coding

* 一種壓縮演算法
  
* 機率低編碼長、機率高編碼短
  
* David Huffman於1952年發行的編碼技術

-------------------------------------
# Getting Started!


# 1. Huffman coding
## Compile & Run

```sh
# Compile
cd 109503510_assignment_4/huffman-main/huffmain-main/
gcc -o huffmain huffcode.c huffman.c huffman.h 
# Run (encode)
./huffmain -i [想壓縮的檔案] -o [壓縮完的檔名] -c
# Run (decode)
./huffmain -i [壓縮完的檔案] -o [解壓縮完的檔名] -d
```
## Results

```sh
# show (encode)
PI = 3.142172
Time = 壓縮的時間 
* 同個資料夾底下會有已壓縮的檔案
# show (decode)
PI = 3.142172
Time = 解壓縮的時間 
* 同個資料夾底下會有解壓縮的檔案
```
# 2. Arithmetic coding
## Compile & Run

```sh
# Compile
cd 109503510_assignment_4/arcd-master/examples/
gcc -o arcdmain arcd_stream.c adaptive_model.c adaptive_model.h arcd.h arcd.c
# Run (encode)
./arcdmain -e <想壓縮的檔案|tee [壓縮完的檔名]
# Run (decode)
./arcdmain -d <壓縮完的檔案|tee [解壓縮完的檔名] 
```
## Results

```sh
# show (encode)
PI = 3.142172
Time = 壓縮的時間 
* 同個資料夾底下會有已壓縮的檔案
# show (decode)
PI = 3.142172
Time = 解壓縮的時間 
* 同個資料夾底下會有解壓縮的檔案
```
## Reference
1. https://github.com/wonder-mice/arcd
2. https://github.com/drichardson/huffman
