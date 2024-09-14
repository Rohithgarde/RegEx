# RegEx
**Sequence of characters that define search patterns, enabling users to find, replace, or validate text efficiently**

/ \w /g              matches all the word characters



/ \W/g              matches all non character words



/\s/g                 match any form of white space



/\S/g                 match anythin not a white space



/\w{4,5}/g       matches any character that are 4 to 5 words long



/[a-zA-Z]at/g   matches any character that start with a-z or A-Z and end with at



/(t|T)he/g        groups all the words that start with small or capital (t/T)



/(t|e|r){2,3}\./g    matches 2 to 3 words of the groups followed by period



/(re){2,3}/g             matches any set of re that is seen 2 to 3 times



/^character/g                    matches the beginning of liine



/^character/gm                 for multiline



/$character/g                     end of the line



/$character/gm                  multiline



/\.$/gm                matches the period at end



/\d{10}/gm         groups 10 digits  like this "1234567890"



/\d{3}-?\d{3}-?\d{4}/gm   suppose if digits are like this "123-456-7890"



/\d{3}[ -]?\d{3}[ -]?\d{4}/gm   suppose if digits are like this "123 456 7890" either space or dash



**LOOK BEHIND:**



    Positive lookbehind:       /(?<=[tT]he)./g      matches all the words that is preceeded by "the"



    Negative lookbehind:     /(?<![tT]he)./g       gets anything that does not have the word "the" before



**LOOK AHEAD:**



    Positive lookahead:      /.(?=at)/g          get any character that has "at" after it



    Negative lookahead:      /.(?!at)/g          get anything that is not followed by "at"
