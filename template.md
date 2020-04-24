# Haskell
The language called by the name Haskell. Haskell named after Haskell Curry. (logician)	
## Author
The language was developed by Philip Wadler.  KRC, OL, Miranda and Orwell influenced Haskell.  An influential book on functional programming authored by Wadler and Bird (Wadler and Bird, 1988). 
## History of the Haskell
Lambda calculus is important concept on functional programming languages. It is basis of many functional compiler intermediate languages like Haskell, OCaml, StandartML. 
There was a conference in September of 1987 to define a non-strict functional programming language. They sometimes met and discuss and the first report of Haskell version 1.0 was in 1 April 1990. 
In 1991 The Haskell Report 1.1 Version Published and edited by Hudak, Wadler and Peyton Jones.
In 1992 The Haskell Report 1.1 Version Published and edited by Hudak, Wadler and Peyton Jones and 1992 the first Haskell tutorial was published, and it was written by Fasel and Hudak. At the same year GHC was created. GHC stands for Glasgow Haskell Compiler. GHC is compiler for Haskell. It is open-source native compiler. GHC is still developing.
In 1994 John Peterson registered the Haskell.org so Haskell gained Internet presence.
In 1996 the Haskell version 1.3 report was published and edited by Hammond and Peterson.
In 1997 the Haskell version 1.4 report was published and edited by Hammond and Peterson the only significant change is that list comprehensions were generalised to arbitrary monads, a decision that was reversed two years later.
In 1999 the language and libraries were published and edited by Peyton Jones and Hughes in the Haskell 98 Report.
The most important point is the Haskell 2010 in the modern history of Haskell development, and it is also the currently used by Haskell Developers. 

## Why was it invented
In the 1980s, functional programming languages were invented and extended variously by lots of researchers. Example Languages are ML, Hope and Miranda. However, many of them did not have ‘open-source’ frameworks. Also, researches were fragmented across the various languages. So, a committee is formed by a group of academics for designing and implementing a new language, which would be used as a vehicle for research as well as for teaching functional programming.
## Why shall we use it/- Things that are specific to this language?
We should use Haskell because Haskell is the best mainstream language for writing correct code and has below properties.
-Purity:
Haskell is pure unlike other functional programming languages. It means it is reliable and there are no side effects. For example, if a function f has type Int -> Int you can be sure that f will not read or write any mutable variables, nor will it perform any input/output.
-Laziness:
Haskell is non-script language. It means something is only will be evaluated if it must.
-Strong typing:
It means you cannot convert a double to integer inadvertently. It is a good property because compiler often treats a double like integer or other types. When we need to convert a double to integer it might be hard, but these cases are rare.
-Elegance:
Haskell is elegance it means that things works exactly like what you expect.
-Concise:
Mostly programs are shorts so writing and reading are easy.
-High level:
Mostly programs are read as same as in the algorithm description. 
-Memory managed:
The Garbage Collector takes care all the dangling pointers.
-Modular:
Haskell strongly suggests using already developed programs in your program.

The combination of these features that makes Haskell unique.

## How to setup an environment to use it in different platforms
-For Windows:
You should go to https://www.haskell.org/platform/windows.html and download the Installer for 32 bit or 64 bit.
-For MAC:
You should go to https://www.haskell.org/platform/mac.html and download the installer.
-For Linux:
You should go to https://www.haskell.org/platform/linux.html and choose your distribution. For example, if you choose Ubuntu so will see a message telling you run the “$ sudo apt-get install haskell-platform” command. After opening your terminal (Ctrl+Alt+T) run the command. After installing you will see a confirmation message. After going into your terminal and run GHCI command. You will get the Prelude prompt and after this you are ready to use Haskell. For exiting the GHCI prolog you may use the command “:quit.exit”.

## Example Codes
-Implement a function that doubles any odd Integer:
```haskell
ifOddDouble :: Integer -> Integer
ifOddDouble n =
  if odd n
    then double n
    else n
```
-Implement factorial function
```haskell
factorial :: Natural -> Natural
factorial n =
  if n == 0
    then 1
    else n * factorial (n - 1)
```
-Create an Employee and with Eq give the ability to the check if they are equal
```haskell
data Employee = Employee { name :: String,	
						   position :: String,
						   idNum :: Int 
						   } deriving (Eq, Show)
```
-Create a simple list
```haskell
numbers = [1,4,9,5]
  ```
-Create Colors
	```haskell
  data Colors = Green
					| Blue
					| Yellow
					| Red
				deriving Show
    ```
-Printing with user input
	```haskell
  main = do putStrLn "Type something: 
   " exampleinput <- getLine 
   putStrLn ("You typed " ++ exampleinput)
    ```
   
