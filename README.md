# Homework-1-Android-Basics

شجاع عايش المطيري

### Description | وصف الواجب
In this task, you are going to build a code to bake a cake to always be the right number of layers, size, and with the right number of candles.


### Instructions | التعليمات
1. You will create a total of three functions for drawing a layered cake with candles.
2. You will use a repeat() inside another repeat(), creating what's called a "nested loop".


### Functions used | الدوال المستخدمة
1. printCakeCandles(candles: Int)
2. printCakeTop(candles: Int)
3. printCakeBottom(candles: Int, layers: Int)


### Notes | ملاحظات
> The way you will build up this code is how you can build up any program, starting with the big picture and adding detail. This is called "top-down development".

### Solution | الحل

fun main() {
   val candles = 24
   val layers = 5
   println("Number of candels: $candles")
   println("Cake top length: $candles")
   println("Number of layers: $layers ")
   printCakeCandles(candles)
   printCakeTop(candles)
   printCakeBottom(candles,layers)
}

fun printCakeCandles(candles: Int){
   print(" ")
   repeat(candles){
       print(",") 
   }
   println()
   
 	print(" ")
   repeat(candles){
       print("|")
   }
   println()
}

fun printCakeTop(candles: Int){
   
  repeat(candles+2){
      print("=")
  }
  println()
}

fun printCakeBottom(candles: Int, layers: Int){
    
  repeat(layers){
      repeat(candles+2){
      print("@")
  }
  println()
  }
   
}

### Here is a picture of the cake you will be baking | صورة النتيجة النهائية

![Cake Output](https://github.com/shaima-alghamdi-tuwaiq/Homework-1-Android-Basics/blob/a745ff19ff5912d2533905b53421b6a3f0cbd85d/output.png)
