    import csv
    import string

    reader = csv.reader(open('Vtabla.dat'))
    vt = []

    for line in reader:
      vt.append(line.pop(0))


    def strips(s):
      s = s.upper()
      sz = ''

      for char in s:
        if char in string.ascii_uppercase:
          sz += char
        elif char in ['Ó', 'Ö', 'Ő']:
          sz += 'O'
        elif char in ['Ú', 'Ü', 'Ű']:
          sz += 'U'
        elif char in ['Á']:
          sz += 'A'
        elif char in ['É']:
          sz += 'E'
        elif char in ['Í']:
          sz += 'I'

      return sz

    print('\t1. feladat')
    szoveg = input('Adj meg egy szöveget: ')

    print('\t2. feladat')
    szoveg = strips(szoveg)

    print('\t3. feladat')
    print(szoveg)

    print('\t4. feladat')
    kulcs = input('Adj meg egy kulcsszót: ')
    kulcs = kulcs.upper()

    print('\t5. feladat')
    mtp = len(szoveg) // len(kulcs)
    tkulcs = kulcs * mtp
    mtp = len(szoveg) % len(kulcs)
    tkulcs += kulcs[:mtp]
    print(tkulcs)

    on = sn = 0

    kod = ''

    print('\t6. feladat')
    for i in range(len(szoveg)):
      for ssz in range(len(vt[0])):
        if szoveg[i] == vt[0][ssz]:
          sn = ssz
      for osz in range(len(vt[0])):
        if tkulcs[i] == vt[osz][0]:
          on = osz
      kod += vt[on][sn]

    print('\t7. feladat')
    print(kod)
    fajl = open('kodolt.dat', 'w')
    fajl.write(kod)
    fajl.close()
