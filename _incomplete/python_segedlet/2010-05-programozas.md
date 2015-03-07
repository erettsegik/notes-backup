    import csv

    reader = csv.reader(open('eladott.txt'), delimiter=' ')

    const = next(reader)

    ELADOTT_JEGYEK = int(const[0])
    VONAL_HOSSZ = int(const[1])
    OSSZEG_10 = int(const[2])
    ULESSZAM = 48

    jegyek = [[int(line[0]), int(line[1]), int(line[2])] for line in reader]


    def tavolsag(x):
      return x[2]-x[1]


    def jegyar(x):
      t = tavolsag(x)
      ft = t // 10 + 1
      ft = ft * OSSZEG_10

      if ft % 5 in [1, 2]:
        ft = ft - ft % 5
      elif ft % 5 in [3, 4]:
        ft = ft + (5 - ft % 5)

      return ft

    print('\t2. feladat')

    print('A legutolsó utas ülése:', jegyek[-1][0], ', '
          'az általa utazott távolság', tavolsag(jegyek[-1]), 'km.')

    print('\t3. feladat')

    print('A következő utasok utazták végig az utat: ', end='')

    i = 0

    for jegy in jegyek:
      i += 1
      if jegy[1] == 0 and jegy[2] == VONAL_HOSSZ:
        print(i, end=' ')

    print()

    print('\t4. feladat')

    osszb = 0

    for jegy in jegyek:
      osszb += jegyar(jegy)

    print('A társaság összbevétele:', osszb, 'Ft.')

    print('\t5. feladat')

    megallok = []

    for jegy in jegyek:
      if jegy[1] not in megallok:
        megallok.append(jegy[1])
      if jegy[2] not in megallok:
        megallok.append(jegy[2])

    megallok.sort()

    felszallok = leszallok = 0

    for jegy in jegyek:
      if jegy[2] == megallok[-2]:
        leszallok += 1
      if jegy[1] == megallok[-2]:
        felszallok += 1

    print('Az utolsó előtti megállónál', felszallok, 'felszálló és',
          leszallok, 'leszálló volt.')

    print('\t6. feladat')

    print('Összesen', len(megallok)-1, 'db megálló volt a végállomások közt.')

    print('\t7. feladat')

    km = int(input('Hányadik kilométernél készítsünk utaslistát? '))

    utaslista = []

    i = 0

    for jegy in jegyek:
      i += 1
      if jegy[1] <= km and jegy[2] > km:
        utaslista.append([i, jegy[0]])

    fajl = open('kihol.txt', 'w')

    for i in range(1, 49):
      foglalt = False
      fajl.write(str(i) + '. ülés: ')
      for utas in utaslista:
        if utas[1] == i:
          foglalt = True
          fajl.write(str(utas[0]) + '. utas\n')
      if not foglalt:
        fajl.write('üres\n')

    fajl.close()
