    import csv

    reader = csv.reader(open('lottosz.dat'), delimiter=' ')
    lottosz = []

    for line in reader:
      lottosz.append([int(line.pop(0)), int(line.pop(0)), int(line.pop(0)),
                      int(line.pop(0)), int(line.pop(0))])

    print('\t1. feladat (52. hét lottószámai)')

    lottosz.append([int(input('1. szám: ')), int(input('2. szám: ')),
                    int(input('3. szám: ')), int(input('4. szám: ')),
                    int(input('5. szám: '))])

    print('\t2. feladat')

    lottosz[-1].sort()
    print(lottosz[-1])

    print('\t3-4. feladat')

    sz = int(input('(1-51 - ig szám)'))
    print(lottosz[sz-1])

    print('\t5. feladat')

    szamok = [False]*90

    for row in lottosz:
      for n in row:
        szamok[n-1] = True

    all = True

    for i in szamok:
      all = all and i

    print('Az összes számot kihúzták' if all else 'Nem húzták ki az összes számot')

    print('\t6. feladat')

    ptl = 0
    hetek = 0

    for row in lottosz:
      ezhet = False
      for n in row:
        if n % 2 != 0:
          ptl += 1
          ezhet = True
      if ezhet:
        hetek += 1

    print(ptl, 'db páratlan szám volt kihúzva', hetek, 'db héten')

    print('\t7. feladat')

    fajl = open('lotto52.ki', 'w')

    for row in lottosz:
      asd = ('{} {} {} {} {}\n').format(row[0], row[1], row[2], row[3], row[4])
      fajl.write(asd)

    fajl.close()

    print('\t8. feladat')

    szamok = [0]*90

    for row in lottosz:
      for n in row:
        szamok[n-1] += 1

    for i in range(90):
      print(szamok[i], end=' ')

    print('\n\t9. feladat')

    primek = [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61,
              67, 71, 73, 79, 83, 89]

    for szam in primek:
      van = False
      for row in lottosz:
        if szam in row:
          van = True
      if not van:
        print(szam)
