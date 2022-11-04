**Using list1**

If it permitted _not_ to `Flatten` list1: 

    ReplacePart[list0, {i_,j_,2} :> list1[[i,j]]]
    
    (* {{{12, 270}, {34, 271}}, {{56, 272}, {78, 273}}} *)


** Using list2**
If the starting point is a flattened list (`list2`):

    ReplacePart[list0, {i_,j_,2}:> Partition[list2,2][[i,j]]]

**Edit**

As pointed out by
[kglr](https://mathematica.stackexchange.com/users/125/kglr)
in a comment, a better way of using list2 is the following:

    ReplacePart[list0, {i_, j_, 2} :> list2[[2 (i - 1) + j]]]

    (* {{{12, 270}, {34, 271}}, {{56, 272}, {78, 273}}} *)
