##1. Fixnum和Fixnum計算結果會是Fixnum，
##  Float和Float計算結果會是Float，
##  但是Float和Fixnum運算結果會是Float
##2. str1+str2會吃兩個字串的記憶體位置，
##  "#{str1#{str2}}"則會視為一個字串，比較省記憶體
##3. Array內部存的資料沒有特定的格式限制，
##  但是Hash所存的資料，結構一定要是Key、Value的組合，
##  兩種存法內部資料都是以","分隔
##4. 
```ruby
arr.reject{|x|x.is_a?(String)}
```
##5. 
```ruby
arr.map{|x|x+2}
```
##6. .uniq會把陣列中重複值不顯示
```ruby
[1,2,3,3].uniq 
```
##結果會變成[1,2,3],但是並不會修改原本的陣列,
##uniq!則會改變本來的陣列的內容
##7. 以1~3隨機而言[1,2,3].sample，
##  rand(3)+1也可以得到1~3隨機
##8. 1 > 3 結果為 false，true == true 結果為 true，
##  !!!false 結果為 true，最終結果 false && true || true，
##  最後回傳結果為 true
##9. binding.pry是能夠下程式中斷點，方便Debug的工具。
##  再Terminal輸入 gem install pry 就能安裝套件，
##  使用情況
```ruby
ruquire 'pry'
a = 1
b = 2

binding.pry
puts a+b
```
##程式會停在 binding.pry，此時能夠檢查 a, b 的值
##10. 
```ruby
puts var>=5?"var is greater than or equal to 5":"var is less than 5"
```
##11. 
```ruby
Test = {
    :name=>"Bob",
    :phone=>147258369
}

Test = {
    name:"Bob",
    phone:147258369
}

```
