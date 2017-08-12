## PHP intro
### Strings
A string is a word or phrase between quotes, like so: "Hello, world!"

You can type a string all at once, like this:

<?php
  echo "Hello, world!";
?>
Or use the concatenation operator, which glues several strings together:

<?php
   echo "Hello," . " " . "world" . "!";
?>
The concatenation operator is just a dot (.). (If you're coming to PHP from JavaScript, the dot does the same thing for strings that + does in JavaScript.)

### Arithmetic
In addition to outputting strings, PHP can also do math.

<?php
  echo 5 * 7;
?>
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
<!-- Just like we sometimes put comments in our CSS (using /* this syntax */ ) or in our HTML (using <!-- this syntax -->), we can also put comments in our PHP code! We do that using two forward slashes (//), like so:

<?php
    echo "I get printed!";
    // I don't! I'm a comment.
?>

### if/else-if/else
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
###
###
###
###
###
###
