# Rabin-Karp-Algorithm


Rabin-Karp:
Procedure Rabin-Karp(Text, Pattern, Prime):
m := Pattern.Length
HashValue := Calculate-Hash(Pattern, Prime, m)
CurrValue := Calculate-Hash(Pattern, Prime, m)
for i from 1 to Text.length - m
 if HashValue == CurrValue and String-Match(Text, Pattern, i) is true
 Return i
 end if
 CurrValue := Recalculate-Hash(String, i+1, Prime, CurrValue)
end f
return -1;
