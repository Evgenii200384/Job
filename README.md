import sys
import string

js = 0
php = 0
data = sys.stdin.read().lower()
words = data.split(string.punctuation + string.whitespace)
for w in words:
    if w == 'php':
        php += 1
    elif w == 'javascript':
        js += 1
if js == php:
    print 'C++, Java or Python'
elif js > php:
    print 'JavaScript'
else:
    print 'PHP'# Job
