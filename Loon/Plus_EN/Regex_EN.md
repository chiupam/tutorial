# Regular expression

Filter subscription nodes using regular expressions

## Common expressions

-`any value` .*

    -All nodes will match as long as they have names, this does not need to be explained

-`Contain` .*(A)

   -If the node name contains ʻA`, such as `.*(IPLC)`, filter nodes with ʻIPLC` in the name
 
-`or` (A)|(B) or ^.*(A|B)

   -Node names containing ʻA` or `B`, such as `(IPLC)|(IEPL)`, filter nodes with ʻIPLC` or ʻIEPL` in the name
 
-`Without` ^((?!A).)*$ or ^(?!.\*?A)

   -The node name does not contain ʻA`, such as `^(?!.*?x1.5)`, and the node name does not contain `x1.5`
 
  ## General method of combination
 
-`containing` and `containing`
 
    -(Hong Kong).\*(IPLC), to filter nodes whose name contains both `Hong Kong` and ʻIPLC`
   
-`Contains` and `Contains` and `Contains`
 
   -(Hong Kong).\*(tunnel).\*(x1), to filter nodes whose names contain both `Hong Kong` and `tunnel` and `x1`
 
-`With` and `Without`
 
   -^(?!.*?x1.5).\*(Hong Kong), to filter nodes whose name does not contain `x1.5` but contains `Hong Kong`