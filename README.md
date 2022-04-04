# Android-kotlin
Guess the Number game!
fun main(){
    var number = (0..10).random()
    var guess :Int;var counter = 1

    println("Lets play guess the Number")
    print("I am ready, ")
    println("What's  Your guess")
    guess = readLine()?.toInt()!!
    do {
       if (number<guess){
           println("Low.Guess again")
        guess = readLine()?.toInt()!!
       counter++}
        else if(number>guess){
           println("High.Guess again")
           guess = readLine()?.toInt()!!
           counter++
        }
    }while (number!=guess)
    println("You got it in $counter")
}
