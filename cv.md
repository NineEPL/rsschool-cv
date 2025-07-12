# Eryk Lebiadzinski

## Contact information:
 - Email: lebedinski.erik@gmail.com
 - Discord: @nineepl
 - Phone number: +48 2137 2137(that's a joke)
 - Github: [NineEPL](https://github.com/NineEPL)

## About Me:
Hi! I'm Erik — a passionate learner with a love for both music and code. When I'm not shredding on electric or bass guitar, I’m deep-diving into gear, pushing it to its limits just to see what creative chaos I can unlock. I bring the same curiosity and intensity to programming, especially when solving algorithmic challenges on platforms like Codewars. Whether it’s sound waves or code lines, I’m always looking for ways to break the rules (responsibly) and build something exciting.

## Skills:
 - Blender 3D
 - Python
 - C++

## Code example("Screen Locking Patterns" on codewars):
```python
from itertools import*
def somethinginbetween(F,L):
    limbo = ""
    findex = []
    lindex = []
    screen=["ABC","DEF","GHI"]
    for i in range(3):
        if F in screen[i]:
            findex.append(i)
            findex.append(screen[i].find(F))
    for i in range(3):
        if L in screen[i]:
            lindex.append(i)
            lindex.append(screen[i].find(L))
    if findex[0] == lindex[0]:
        limbo = screen[findex[0]][1]
    elif findex[1] == lindex[1]:
        limbo = screen[1][findex[1]]
    else:
        limbo = "E"
    return limbo


def count_patterns_from(firstPoint, length):
    if length ==0 or length == 1:
        return length
    points = "ABCDEFGHI"
    p_tree = {"A":"BDEFH","B":"ACDEFGI","C":"BDEFH","D":"ABCEGHI","E":"ABCDFGHI","F":"ABCEGHI","G":"BDEFH","H":"ACDEFGI","I":"BDEFH"}
    bast = {}
    already_used = []
    nice_ones = []
    nice_count = 0
    a_points = points[:points.find(firstPoint)]+points[points.find(firstPoint)+1:]
    combinations = []
    for i in permutations(a_points,length-1):
        combinations.append(firstPoint+"".join(list(i)))

    for i in combinations:
        bad = False
        already_used=[]
        already_used.append(i[0])
        for j in range(1,length):
            if i[j] not in p_tree[i[j-1]]:
                if somethinginbetween(i[j],i[j-1]) not in already_used:
                    bad = True
                    break
            already_used.append(i[j])
        if not bad:
            nice_ones.append(i)
            nice_count += 1

    return nice_count

```

## Working expeirence:
 - Participated in the creation of the website [INFORMEJTYCY](https://informejtycy.pl/) as part of the Polish olympiad [Zwolieni z Teorii](https://zwolnienizteorii.pl/).
 - Fully developed the website [MercyRig](https://erikepl.w.staszic.waw.pl/) as part of a school project.

## Education
 - XIV LO ogólnokształcące im. Stanisława Staszica w Warszawie(in progress)
 - RS Schools Course «JavaScript/Front-end. Stage 0» (in progress)

## Languages
 - English: B1/B2
 - Russian: native
 - German: A1
 - Polish: B2/C1