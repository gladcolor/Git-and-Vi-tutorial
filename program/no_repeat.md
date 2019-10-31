# What is "don't Repeat Yourself"?
[Wikipedia](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself) explain this coding principle quite clearly. ___Don't repeat yourself___ (DRY) aims at reducing repetition line of coding. When you are going to write down a piece of code second time, replace it with a function to avoid redundancy.

# Why "don't Repeat Yourself"?
Also from [Wikipedia](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself), the DRY principle is derived from an assumption:
>Every piece of knowledge must have a single, unambiguous, authoritative representation within a system. 

> -- <cite>Hunt, Andrew; Thomas, David (1999). The Pragmatic Programmer : ___From Journeyman to Maste___</cite>

That is the reason for DRY principle. DRY is applied successfully because is divide complexity of the targeted system into small pieces and make maintenance simple. The reusability and robustness is also enhanced.
 
# How "don't Repeat Yourself"?
When writing a function which have be written previously in other functions exactly or similarly, you need to think refactorying that piece of code. Once you have implemented this new generalized function, it can be used in the new code block and the previous functionality. 