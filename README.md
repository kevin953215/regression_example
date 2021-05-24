# regression_example
此處為一個簡易的regression model的範例

裏頭的data是一個糖尿病的資料集，主要包括442行資料，10個屬性值，分別是：Age(年齡)、性別(Sex)、Body mass index(體質指數)、Average Blood Pressure(平均血壓)、S1~S6一年後疾病級數指標。Target為一年後患疾病的定量指標。
此處sklearn datasets的參考網址:https://www.itread01.com/content/1546080514.html

在這一個程式碼中主要是在探討Is average blood pressure an important factor for diabetes disease這個問題,因此我建立了兩個完全相同的網路架構並且分別給予有含average blood pressure的training data和無average blood pressure的training data。搭配K-fold cross validation驗證最後得到average blood pressure is an important factor for diabetes disease的結論,詳細過程請參閱程式碼。最後我也有使用autokeras來創建另一個網路模型並透過繪製residual plot來做比較。
