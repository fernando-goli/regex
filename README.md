# regex
Template for regex

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions
https://regex101.com/

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

| Input String	| Pattern | Pattern	Description |	Total matches	| Result | 
| --- | --- | --- | --- | --- |
| Hello World! |	. |	Corresponde a qualquer personagem |	12	| 'H', 'e', 'l', l'', 'o', ' ', 'W', 'o', 'r', 'l', 'd', '!' |
| Hello World! |	..o |	Corresponde a 'a' que segue quaisquer dois caracteres	| 4	| 'llo', ' Wo' |
| Hello World! |	..l |	Correspondência 'l' que segue quaisquer dois caracteres	| 2	|'Hel', 'orl' |
| Hello World! |	..l.. |	Corresponde a 'l' que está entre quaisquer dois caracteres	| 2 |	Hello, orld! |
| Hello World 123 |	\S |	Encontre qualquer caractere que não seja espaço	| 13 |	'H', 'e', 'l', l'', 'o', 'W', 'o', 'r', 'l', 'd', '1', '2', '3' |
| Hello World 123 |	\s	| Encontre um caractere espacial	' ', ' ' (Two white spaces) |
| Hello World! |	^H	| Encontre 'H' que começa na linha	| 1 |	'H' |
| Hello World! |	^Hello |	Encontre 'Hello' que começa na linha	| 1 |	'Hello' |
| Hello World! |	^hello |	Encontre 'hello' que vem no início da string	| 0 |	No match found |
| Hello World! |	^World |	Encontre 'World' que começa na linha	| 0 |	No match found |
| Hello World! |	World!$ |	Encontre 'World' que vem no final da string.	| 1 |	'World!' |
| Hello World! |	Worl$ |	Encontre 'Worl' que vem no final da string.	| 0 |	No match found|
| Hello World! |	...$	| Encontre quaisquer três caracteres do final da string	| 1 |	'ld!' |
| Hello World! |	..\s	| Encontre quaisquer dois caracteres antes do espaço na string	| 1 |	'lo ' |
| A12B34C567 *890X | \d | Encontre qualquer numero | 10 | 1, 2, 3, 4, 5, 6, 7, 8, 9, 0 |
| A12B34C567 *890X | \D | Encontre por qualquer caractere não-dígito | 10 | A,B,C |
