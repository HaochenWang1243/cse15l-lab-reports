# CSE 15L Lab Report-week 4

![here](parserDiff.jpg)
## change __No.1__:    
## line __43__: add statement  
## `if(markdown.charAt(nextOpenBracket - 1) != '!')`
This change intends to address the incorrect output caused by a image link. Image link should not be included in the collections of URLs.  
link to the failure-inducing input:  
[failure-inducing input-1](test-file-2.md)  
__symptom__: image link included in the output
 ![here](imageCaptured.jpg)
___
 ## change __No.2__:    
## line __43__: changed to:
## `if(nextOpenBracket==0 || markdown.charAt(nextOpenBracket - 1) != '!')`
This change intends to address the StringIndexOutOfBoundsException thrown when running the program after change No.1 with a input file that begins with a URL.  
link to the failure-inducing input:  
[failure-inducing input-2](test-file-3.md)  
__symptom__: `StringIndexOutOfBoundsException` thrown
 ![here](indexOf[-1Is-1.jpg)
___
 ## change __No.3__:    
 ## line __43__: changed to: 
## `if (nextCloseBracket+1==openParen && (nextOpenBracket ==0 || markdown.charAt(nextOpenBracket - 1) != '!'))`  
This change intends to address the incorrect output when input a file that has pairs of close brackets `[]` and open brackets `()` that are not adjacent, which means the close and open brackets are not used for link.  
link to the failure-inducing input:       
[failure-inducing input-3](test-file-4.md)  
 __symptom__: ppap isn't a URL but included in the output.
 ![here]([]sth().jpg)