# Lesson 1: PHP Basic Syntax

Variables se pehle PHP ka **basic syntax** samajhna zaroori hai. Syntax
ka simple meaning hai: kisi programming language mein code likhne ke
rules.

## 1. PHP code kaise start hota hai?

PHP code likhne ke liye hum `<?php` use karte hain.

``` php
<?php

echo "Hello World!";

?>
```

Isme:

  Code               Meaning
  ------------------ --------------------------
  `<?php`            PHP code start karta hai
  `echo`             Output display karta hai
  `"Hello World!"`   Text jo display hoga
  `;`                Statement end karta hai
  `?>`               PHP code close karta hai

**Important:** Agar file mein sirf PHP code hai, toh closing `?>` likhna
optional hai. Professional PHP files mein aksar ise omit karte hain.

## 2. PHP file ka extension

PHP files ka extension `.php` hota hai.

Examples: - `index.php` - `about.php` - `login.php` - `variables.php`

## 3. Statements kya hote hain?

PHP mein har instruction ko statement kehte hain.

``` php
<?php

echo "Hello";
echo "Welcome";
echo "Learning PHP";
```

Yahan 3 statements hain.

Har statement ke end mein semicolon (`;`) lagta hai.

## 4. Comments kya hote hain?

Comments ka use code ko explain karne ke liye hota hai. PHP comments ko
execute nahi karta.

**Single-line comment:**

``` php
<?php

// This is a comment
echo "Hello";
```

**Multi-line comment:**

``` php
<?php

/*
This is a
multi-line comment
*/

echo "Hello";
```

## 5. PHP mein output kaise display karein?

Do common ways hain:

**Using echo:**

``` php
<?php

echo "Hello Raj";
```

**Using print:**

``` php
<?php

print "Hello Raj";
```

Dono output display karte hain. Abhi hum primarily `echo` use karenge.

## 6. HTML ke saath PHP

PHP HTML ke andar bhi likh sakte hain.

``` php
<!DOCTYPE html>
<html>
<head>
    <title>My PHP Page</title>
</head>
<body>

    <h1>Welcome</h1>

    <?php
        echo "Hello from PHP!";
    ?>

</body>
</html>
```

Isse browser mein HTML heading aur PHP ka output dono show honge.

------------------------------------------------------------------------

## Practice: Apna code likho

Apni `syntax.php` file banao aur ye program khud likho:

``` php
<?php

// My first PHP practice

echo "My name is Raj.";
echo PHP_EOL;

echo "I am learning PHP.";
echo PHP_EOL;

echo "PHP is interesting.";
```

Terminal mein run karo:

``` powershell
php syntax.php
```
