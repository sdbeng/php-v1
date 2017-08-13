## PHP intro
### Strings
A string is a word or phrase between quotes, like so: "Hello, world!"

You can type a string all at once, like this:
```php
<?php
  echo "Hello, world!";
?>
```
Or use the concatenation operator, which glues several strings together:
```php
<?php
   echo "Hello," . " " . "world" . "!";
?>
```
The concatenation operator is just a dot (.). (If you're coming to PHP from JavaScript, the dot does the same thing for strings that + does in JavaScript.)

### Arithmetic
In addition to outputting strings, PHP can also do math.
```php
<?php
  echo 5 * 7;
?>
```
Here we use echo to multiply 5 and 7, and we end our line of code with a semicolon. PHP will output 35.

### Variables
So far we've been outputting strings and doing math.

To do more complex coding, we need a way to "save" these values. We can do this using variables. A variable can store a string or a number, and gives it a specific case-senstive name.

Examples:

$myName = "Beyonce";
$myAge = 32;
All variable names in PHP start with a dollar sign ( $ ).

###Semicolons
You've probably noticed that our lines of PHP code end in semicolons (;). PHP requires semicolons at the end of each statement, which is the shortest unit of standalone code. (For example, echo "Hello!"; or 2 + 2;)

You can think of a statement is a complete PHP thought. 19 + or echo aren't complete thoughts, so you wouldn't put semicolons at the end of them!

<?php echo "Use your semicolons!"; ?>
### Comments
```php
<?php
    echo "I get printed!";
    // I don't! I'm a comment.
?>
```
### if/else-if/else
```php
<?php
        $gameNinja = "Jin";
        if ($gameNinja == "Jin"){
            echo "Hi Jin!";
        }else if($gameNinja == "Zulu"){
            echo "Hi Zuluuu";
        }
        else{
            echo "You are the master!";
        }
    ?>
```
### switch statement
```php
<?php
    switch (2) {
        case 0:
            echo 'The value is 0';
            break;
        case 1:
            echo 'The value is 1';
            break;
        case 2:
            echo 'The value is 2';
            break;
        default:
            echo "The value isn't 0, 1 or 2";
    }
    ?>
    // another example
    <?php
    $fruit = "Apple";

    switch ($fruit) {
        case 'Apple':
            echo "Yummy.";
            break;
        case 'Orange':
            echo "Mmmm";
            break;
        default:
            echo "not a fuit";
    }
    ?>
```
### Multiple Cases. Falling Through!
You sometimes want to make multiple expressions, all of which have the same result. Consider the following if statement:
```php
if ($i == 1 ||
    $i == 2 ||
    $i == 3) {
 echo '$i is somewhere between 1 and 3.';
}
```
With a switch statement, you can do this by adding cases right after another without a break. This is called falling through. The following code works exactly like the above if statement:
```php
case 1:
case 2:
case 3:
    echo '$i is somewhere between 1 and 3.';
    break;
```
<!-- example complete -->
```php
<?php
    $i = 5;

    switch ($i) {
        case 0:
            echo '$i is 0.';
            break;
        case 1:
        case 2:
        case 3:
        case 4:
        case 5:
            echo '$i is somewhere between 1 and 5.';
            break;
        case 6:
        case 7:
            echo '$i is either 6 or 7.';
            break;
        default:
            echo "I don't know how much \$i is.";
    }
    ?>
```

### Using "Endswitch". Syntactic Sugar!
You have two ways of creating a switch. First, there's the way we have made all the past exercises:
```php
switch ($i) {

}
```
But we can also make it this way:
```php
switch ($i):

endswitch;
```
This is called alternative syntax. It exists to provide syntactic sugar

There's no difference when using either the curly brace syntax (first example) or alternative syntax (second example), it only provides readability, thus it's usually used when mixing HTML and PHP code in the same file.
```php
<?php
    $i = 5;

    switch ($i) :
        case 0:
            echo '$i is 0.';
            break;
        case 1:
        case 2:
        case 3:
        case 4:
        case 5:
            echo '$i is somewhere between 1 and 5.';
            break;
        case 6:
        case 7:
            echo '$i is either 6 or 7.';
            break;
        default:
            echo "I don't know how much \$i is.";
    endswitch;
    ?>
```
### Arrays
```php<?php
      $array = array("Egg", "Tomato", "Beans");
    ?>  
```
###
###
