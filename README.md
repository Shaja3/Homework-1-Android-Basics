# Name: Shujaa Almutairi | الأسم:شجاع المطيري

# Homework-1-Android-Basics

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

### website | الموقع
[kotlin playground](https://www.bing.com/ck/a?!&&p=b369e8c07fffd4eeJmltdHM9MTY1OTQxMTU2NCZpZ3VpZD1mNTgxNzI0Ni02NDgwLTQ1YmItODFhZC05MzNiYjcwOThiYjQmaW5zaWQ9NTE0Mg&ptn=3&hsh=3&fclid=b35987e9-1214-11ed-880d-6e9d0a6b5fdc&u=a1aHR0cHM6Ly9kZXZlbG9wZXIuYW5kcm9pZC5jb20vdHJhaW5pbmcva290bGlucGxheWdyb3VuZA&ntb=1)

### The Solution | الحل

[Solution](https://pl.kotl.in/DdZHsA7ZG)

  ```
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
  ```

### Here is a picture of the cake you will be baking | صورة النتيجة النهائية

[Cake Output]

![image](https://user-images.githubusercontent.com/95444663/182286566-ce362015-a396-4336-a943-ab91b1c06897.png)
