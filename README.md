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


Output


![image](https://user-images.githubusercontent.com/95444663/182279567-6b7c33e4-f133-4a75-bc16-5621949c3d51.png)


