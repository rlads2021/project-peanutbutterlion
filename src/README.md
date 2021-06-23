# 原始碼說明文件
## 候選人政見
我們與臺大學生會選委會聯繫過後，對方表示未曾有人整理歷年來之選舉政見，因此我們的資料出自二處：  
   粉專爬文(104-109學年度): 自臺大學生會選委會的粉專，找出每年度「選舉公報」中之學生會會長候選人的政見，將其儲存成`.txt`文字檔。  
   查找PTT(97-103學年度): 這七年的政見皆有人整理放在PTT網站中，同樣儲存成`.txt`文字檔。
   - `Politics_txt/`：各檔案為每個候選人的政見
   - `Politics_txt_by_years/`：各檔案為每年度所有候選人的政見
   
## 使用者字典和停用詞字典
- [使用者字典](./user_dict.txt)
- [停用詞字典](./stop_word.txt)

## jiebaR
- [jiebaR原始檔HTML檔](./jiebaR.html)
- [tf-idf原始檔HTML檔](./tf-idf.html)

## CKIPtagger
資料夾`CKIPtagger/`裡為使用CKIP斷詞系統做的文本分析，有`.Rmd`和`.html`，而`ckiptagger_result_png/`則是我們在將`.Rmd`輸出成`.html`時，因為我們載入模型檔的緣故使得RStudio跑得過慢，容易當掉，因此我們把`result(年份)`在`Rconsole`執行，並把結果截圖下來，儲存在`ckiptagger_result_png/`這個資料夾中。另外由於CKIPtagger的模型檔案太大，於是我們採用下方超連結的方式：
- [CKIPtagger模型檔](https://drive.google.com/drive/folders/105IKCb88evUyLKlLondvDBoh7Dy_I1tm)
- [原始碼HTML檔](./CKIPtagger/finalproject_ckiptagger.html)
- [原始碼Rmd檔](./CKIPtagger/finalproject_ckiptagger.Rmd)

## TextRank
- [原始碼HTML檔](./textrank.html)