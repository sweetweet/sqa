Software Quality Assurance
===

Sample code for software quality assurance at FCU.

### Unit1x: [Debugging](LectureNotes.md/#unit-1x-debugging)

**Lab 1**: debug this [program](/src/debug/BubbleSort.java)

**Lab 2**: 應⽤迴圈來寫一個程式計算 sin(x),其中 x 為一個徑度。30度 等於 30*PI/180徑度, 例如 sin(30’) = sin(pi/6) = sin(3.14159/6) 約等於 0.5。使用 debug 的工具來協助你撰寫此程式。sin(x) 的公式如下,迴圈跑的越多次值會越精準,你可以⼤約設定 10 個迴圈。

```
sin(x) = x - (x^3/3!) + (x^5/5!) - (x^7/7!) + ...
```

**Lab 3**: 改寫 Lab2, 一開始迴圈只跑3, 每次增加 2 個，一直到相鄰的兩次`新增迴圈`所得到的值小於 0.00001。請利用 debugging 的各種 view 來協助擬進行此程式。或使用這個 [buggy sample code](/src/debug/Sin.java) 來除錯。

### Unit 2x Defensive Programming

#### [Assertion](LectureNotes.md/#assertion)

**Lab 1**: 學期成績由期中考、期末考、平成成績所組成，各佔 30%, 30%, 40%。計算出的成績應該小於 100 分，請用斷言來確保最後成績的正確。

**Lab 2**: 經過 Sort 後，我們斷言第一個元素一定比第二個元素小，請用 assert 來完成。

#### [Exception] (LectureNotes.md/#exception-handling)

**Lab 1**: 修改 [ExceptionDemo.java](src/debug/ExceptionDemo.java) 中的 getGradeAverage，當學生個數為 0 時，會拋出一個 NoStudentException。	


### Unit 3x [JUnit](LectureNotes.md/#unit-3x-junit)

Lab 1: 寫一個程式來依據 BMI 檢驗體重是否過重。BMI = 體重 (kg) / 身高 (m2)。其分級如下：
* 體重過輕	BMI ＜ 18.5
* 正常範圍	18.5 ≦ BMI ＜24
* 過    重	24 ≦ BMI ＜ 27
* 輕度肥胖	27 ≦ BMI ＜ 30
* 中度肥胖	30 ≦ BMI ＜ 35
* 重度肥胖	BMI ≧ 35

開發流程

1. design class *Health.checkBMI(): String*
2. design *HealthTest.checkBMITest()*
3. implement *Health.checkBMI()*
4. test *checkBMI()* by *checkBMITest()*


### Unit 4x Test coverage

### Unit 5x Improving testability

### Unit 6x Load testing
