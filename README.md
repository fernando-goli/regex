# regex
Template for regex

### Metacaracteres

"^" matches the position at the beginning of string(unless used for negation "[^]")<br/> 
"$" matches the position at the end of string character.<br/> 
"?" match preceding literal or sub-expression 0 or 1 times.<br/> 
"+" match preceding literal or sub-expression one or more times.<br/> 
"*" match preceding literal or sub-expression zero or more times<br/> 
"." match any character except new line.<br/> 
"[ ]" match any one of the characters inside, accepts a range, e.g., "[a-c]".<br/> 
"( )" used to create a sub-expression<br/> 
"\d" match any digit character. "\D" is the complement.<br/> 
"\w" match any word character (letters, digits, underscore). "\W" is the complement.<br/> 
"\s" match any whitespace character including tabs and newlines. \S is the complement.<br/> 
"*?" Non-greedy version of *. Not fully discussed in class.<br/> 
"\b" match boundary between words. Not discussed in class.<br/> 
"+?" Non-greedy version of +. Not discussed in class.<br/> 
"{m,n}" The preceding element or subexpression must occur between m and n times, inclusive.<br/> 
