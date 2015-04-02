    import csv

    reader = csv.reader(open('HIVASOK.TXT'), delimiter=' ')
    hivasok = []

    for line in reader:
      hivasok.append([int(line.pop(0)), int(line.pop(0)), int(line.pop(0)),
                      int(line.pop(0)), int(line.pop(0)), int(line.pop(0)),
                      next(reader).pop(0)])


    def mobile(x):
      if (x[:2] in ['39', '41', '71']):
        return True
      else:
        return False


    def hivasido(iko, ikp, ikm, ivo, ivp, ivm):
      km = int(3600 * iko + 60 * ikp + ikm)
      vm = int(3600 * ivo + 60 * ivp + ivm)
      return (vm-km)//60 + 1


    def csucsidoe(iko, ikp, ikm):
      km = (3600 * iko) + (60 * ikp) + ikm
      if km > (7*3600) and km < (18*3600):
        return True
      else:
        return False

    print('\t1. feladat')

    isz = input('Adj meg egy telefonszámot: ')

    if (mobile(isz)):
      print('A megadott szám mobiltelefonhoz tartozik')
    else:
      print('A megadott szám nem mobiltelefonhoz tartozik')

    print('\t2. feladat')

    ikt = input('Hívás kezdete (óra perc másodperc): ').split()

    for i in ikt:
      ikt.append(int(ikt.pop(0)))

    ivt = input('Hívás vége (óra perc másodperc): ').split()

    for i in ivt:
      ivt.append(int(ivt.pop(0)))

    print(hivasido(ikt[0], ikt[1], ikt[2], ivt[0], ivt[1], ivt[2]), ' perc')

    print('\t3. feladat')

    fajl = open('percek.txt', 'w')

    for row in hivasok:
      fajl.write(('{} {}\n').format(
        hivasido(row[0], row[1], row[2], row[3], row[4], row[5]), row[6])
      )

    fajl.close()

    print('\t4. feladat')

    cs = ncs = 0

    for row in hivasok:
      if (csucsidoe(row[0], row[1], row[2])):
        cs += 1
      else:
        ncs += 1

    print('Csúcsidős hívások:', cs, '-', 'csúcsidőn kívüli hívások:', ncs)

    print('\t5. feladat')

    mp = vp = 0

    for row in hivasok:
      if mobile(row[6]):
        mp += hivasido(row[0], row[1], row[2], row[3], row[4], row[5])
      else:
        vp += hivasido(row[0], row[1], row[2], row[3], row[4], row[5])

    print('Mobillal telefonált percek:', mp, '-',
          'vezetékessel telefonált percek:', vp)

    print('\t6. feladat')

    csp = 0

    for row in hivasok:
      if mobile(row[6]):
        if csucsidoe(row[0], row[1], row[2]):
          csp += 69.175 * hivasido(row[0], row[1], row[2],
                                   row[3], row[4], row[5])
      else:
        if csucsidoe(row[0], row[1], row[2]):
          csp += 30 * hivasido(row[0], row[1], row[2],
                               row[3], row[4], row[5])

    print(round(csp, 2), ' Ft')
