with open('B000_0.20_01_l6l8.txt', 'w') as file3:
    with open('CF_l6_ConfigB000_0.20_01.dat', 'r') as file1:
        with open('CF_l8_ConfigB000_0.20_01.dat', 'r') as file2:
            for line1, line2 in zip(file1, file2):
                line1.rstrip()
                line2.rstrip()
                words1 = line1.split()
                words2 = line2.split()
                print >>file3, words1[5], words2[5]
