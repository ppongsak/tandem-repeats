Build a Tandem Repeat detector in any language. **There is NO single "right" way
to do this**. Many methods and algorithms will work. Some faster than others.  

Tandem Repeat: https://en.wikipedia.org/wiki/Tandem_repeat

DNA is a molecule with 4 proteins represented by the letters 'A', 'C', 'G', 'T'

In data, this effectively makes a string with an alphabet of these 4 letters only.
When the letters repeat in a substring pattern, this is called a Tandem Repeat.

EXAMPLES:  
GAGGCATCATCATCATCATTGCC   Substring 'CAT' repeated 5 times (not substring 'CATCAT')
CATGGCAAGGCAAGGCAATTCGG   Substring 'GGCAA' repeated twice.

It is important to know the following rules:
1) Substrings are only interesting if they are of size 3-10
2) The number of repeats are unknown.
3) The substrings repeating are unknown.
4) The length of the string is unknown.
5) It IS possible for repeats to overlap.


Solutions should have the output in the form of json:
```
{
  'index-substring' : number_of_repeats
}
```

Index is the index of the character starting the repeat. The first letter in a
string is index 0, the second is 1. For the example string: 'GAGGCATCATCATCATCATTGCC'
the output would be:  

```
{
  '4-CAT': 5
}
```

Email a link to a public Github repository with your solution. Solutions must
contain:

1. Source Code
2. Instructions to run
3. Tests, with Instructions how to run tests.
4. Output given test strings.
5. Document explaining choices, limitations and algorithm performance.
