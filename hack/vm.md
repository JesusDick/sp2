            a   c    d   j
         111a 1234 5612 3123
0x1000 = 0001 0000 0000 0000   >> 12 == 0000 0000 0000 000a
         000a 0000 0000 0000   >> 12 == 0000 0000 0000 000a

0x0FC0 = 0000 1111 1100 0000   >> 6  == 0000 0000 00 c1..6
         0000  c1..6 00 0000   >> 6  == 0000 0000 00 c1..6

0x0038 = 0000 0000 0011 1000   >> 3  == 0000 0000 0000 0 d1..3
         0000 0000 00d1.3000   >> 3  == 0000 0000 0000 0 d1..3

0x0007 = 0000 0000 0000 0111   >> 0  == 0000 0000 0000 0 j1..3

      a = (I & 0x1000) >> 12;
      c = (I & 0x0FC0) >>  6;
      d = (I & 0x0038) >>  3;
      j = (I & 0x0007) >>  0;