# PHP Variables

## 1. Variable kya hota hai?

Variable ek **container** ki tarah hota hai jisme hum data store karte
hain.

Example: Maan lo tumhe apna naam, age aur city store karni hai.

``` php
<?php

$name = "Raj";
$age = 22;
$city = "Mumbai";

?>
```

Yahan humne 3 variables banaye:

-   `$name` mein `"Raj"` store hai.
-   `$age` mein `22` store hai.
-   `$city` mein `"Mumbai"` store hai.

## 2. PHP mein variable kaise banate hain?

PHP mein variable banane ke liye `$` (dollar sign) use hota hai.

**Syntax:**

``` php
$variable_name = value;
```

Example:

``` php
<?php

$name = "Raj";

echo $name;

?>
```

Output:

``` text
Raj
```

Samjho:

  Part      Meaning
  --------- ---------------------
  `$name`   Variable name
  `=`       Assignment operator
  `"Raj"`   Stored value
  `;`       Statement ends

## 3. Variable naming rules

PHP mein variables banane ke kuch rules hain:

1.  Variable ka naam `$` se start hona chahiye.
2.  `$` ke baad naam letter ya underscore `_` se start hona chahiye.
3.  Variable name number se start nahi ho sakta.
4.  Variable name mein spaces allowed nahi hain.
5.  PHP variables case-sensitive hote hain.

Examples:

``` php
<?php

$name = "Raj";       // Valid
$_city = "Mumbai";   // Valid
$userAge = 22;       // Valid

// $2name = "Raj";     // Invalid
// $user name = "Raj"; // Invalid

?>
```

**Case-sensitive example:**

``` php
<?php

$name = "Raj";
$Name = "Rahul";

echo $name;
echo PHP_EOL;
echo $Name;

?>
```

Output:

``` text
Raj
Rahul
```

`$name` aur `$Name` PHP ke liye alag variables hain.

## 4. Variable ki value display kaise karein?

Variable ki value display karne ke liye `echo` use karte hain.

``` php
<?php

$name = "Raj";
$age = 22;

echo $name;
echo PHP_EOL;

echo $age;

?>
```

Output:

``` text
Raj
22
```

### PHP_EOL kya hai aur iska use kyun hota hai?

`PHP_EOL` ka full form hai **PHP End Of Line**.

Iska use output mein ek line khatam karke next output ko **new line**
par dikhane ke liye hota hai.

Example without `PHP_EOL`:

``` php
<?php

echo "Hello";
echo "Raj";

?>
```

Output:

``` text
HelloRaj
```

Dono outputs ek hi line mein aa gaye, kyunki `echo` apne aap new line
add nahi karta.

Example with `PHP_EOL`:

``` php
<?php

echo "Hello";
echo PHP_EOL;
echo "Raj";

?>
```

Output:

``` text
Hello
Raj
```

Yahan `PHP_EOL` ne `Hello` ke baad line break add kiya.

**PHP_EOL kyun use karein?**

-   Output ko readable banane ke liye.
-   Har result ko alag line mein dikhane ke liye.
-   Windows, Linux aur macOS ke liye appropriate line-ending character
    use karne ke liye.

**Important:** `PHP_EOL` terminal/command-line output ke liye useful
hai. Browser mein HTML page par line break dikhane ke liye aam taur par
`<br>` use karte hain.

``` php
<?php

echo "Hello<br>";
echo "Raj";

?>
```

Browser output:

Hello\
Raj

## 5. Double quotes ke andar variables

PHP mein double quotes ke andar variable likhne par uski value display
hoti hai.

``` php
<?php

$name = "Raj";
$age = 22;

echo "My name is $name";
echo PHP_EOL;

echo "My age is $age";

?>
```

Output:

``` text
My name is Raj
My age is 22
```

Is technique ko **variable interpolation** kehte hain.

## 6. Variable ki value change karna

PHP mein ek variable ki value baad mein change bhi kar sakte hain.

``` php
<?php

$name = "Raj";

echo $name;
echo PHP_EOL;

$name = "Rahul";

echo $name;

?>
```

Output:

``` text
Raj
Rahul
```

Jab humne `$name` ko dobara assign kiya, toh uski purani value replace
ho gayi.

------------------------------------------------------------------------

## Practical Exercise

Ab tumhari baari!

`variables.php` naam ki file banao aur ye task complete karo.

**Task:** Apni 4 details variables mein store karo:

1.  Name
2.  Age
3.  Favourite programming language
4.  City

Starter code:

``` php
<?php

$name = "";
$age = 0;
$language = "";
$city = "";

// Display all four details using echo

?>
```

Expected output (example):

``` text
My name is Raj.
My age is 22.
My favourite language is Python.
I live in Mumbai.
```

## Quick Check

**Q1.** Inmein se valid PHP variable kaunsa hai?

-   A. `name`
-   B. `$name`
-   C. `2name`
-   D. `@name`

**Q2.** Is code ka output kya hoga?

``` php
$x = 10;
$y = 20;

echo $x + $y;
```

Apna exercise code aur dono answers check karne ke liye apne tutor ko
bhejo.

------------------------------------------------------------------------

## Lesson Recap

-   Variable data store karne ke liye use hota hai.
-   PHP variable `$` se start hota hai.
-   `=` value assign karta hai.
-   `echo` output display karta hai.
-   `PHP_EOL` output ko next line par le jaata hai.
-   PHP variable names case-sensitive hote hain.
-   Double quotes ke andar variable ki value directly display ho sakti
    hai.
