    import csv

    lis = csv.reader(open('szavazatok.txt'), delimiter=' ')

    jeloltek = []

    allampolgarok = 12345

    for line in lis:
      jeloltek.append([int(line.pop(0)), int(line.pop(0)), line.pop(0),
                       line.pop(0), line.pop(0)])

    print('\t2. feladat')
    print('A helyhatósági választáson', len(jeloltek), 'képviselőjelölt indult.')

    print('\t3. feladat')
    nev = input('Add meg egy képviselőjejölt nevét: ')

    talalt = False
    for a in jeloltek:
      if nev == a[2] + ' ' + a[3]:
        print(a[1], 'db szavazatot kapott.')
        talalt = True

    if not talalt:
      print('Ilyen nevű képviselőjelölt nem szerepel a nyilvántartásban!')

    print('\t4. feladat')

    szavazok = 0

    for a in jeloltek:
      szavazok += a[1]

    print('A választásokon', szavazok, 'állampolgár, '
          'a jogosultak', round(szavazok/allampolgarok*100, 2), '%-a vett részt.')

    print('\t5. feladat')

    szavazatok = {'GYEP': 0, 'HEP': 0, 'TISZ': 0, 'ZEP': 0, '-': 0}

    for a in jeloltek:
      szavazatok[a[4]] += a[1]

    print('Gyümölcsevők pártja=', round(szavazatok['GYEP']/szavazok*100, 2), '%')
    print('Húsevők pártja=', round(szavazatok['HEP']/szavazok*100, 2), '%')
    print('Tejivók szövetsége=', round(szavazatok['TISZ']/szavazok*100, 2), '%')
    print('Zöldségevők pártja=', round(szavazatok['ZEP']/szavazok*100, 2), '%')
    print('Független jelöltek=', round(szavazatok['-']/szavazok*100, 2), '%')

    print('\t6. feladat')

    tsz = 0
    for i in range(len(jeloltek)):
      if jeloltek[i][1] > tsz:
        tsz = jeloltek[i][1]

    for a in jeloltek:
      if a[1] == tsz:
        print(a[2] + ' ' + a[3], end=' ')
        if a[4] == '-':
          print('független')
        else:
          print(a[4])

    print('\t7. feladat')

    fajl = open('kepviselok.txt', 'w')

    for i in range(1, 9):
      tsz = 0
      for a in jeloltek:
        if a[0] == i:
          if a[1] > tsz:
            tsz = a[1]
      for a in jeloltek:
        if a[1] == tsz and a[0] == i:
          fajl.write('{} {} {} '.format(i, a[2], a[3]))
          if a[4] == '-':
            fajl.write('fuggetlen\n')
          else:
            fajl.write(a[4] + '\n')

    fajl.close()
