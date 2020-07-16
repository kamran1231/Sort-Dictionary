# Sort-Dictionary

import operator

d = {1:4,2:6,8:12,4:3,0:0,6:15}
print('Original dictionary',d)

sorted_d = dict(sorted(d.items(),key= operator.itemgetter(1)))
print('Dictionary in ascending order by values:',sorted_d)


sorted_d = dict(sorted(d.items(), key= operator.itemgetter(1),reverse=True))
print('Dictionary in descending order by values:',sorted_d)
