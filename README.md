# 7 bit 128 code digital information encoding standard

dies128 is a conceptual rewrite of the ASCII standard. Various characters have
been reorganized and aligned, and vestigial non-printables have been discarded
in favor of newer, more useful ones.

Among its other innovations, it is capable of sending transmissions in a tree
structure, and transferring frames of arbitrary binary data.

This repository was created for the purpose of organizing information related to
dies128.

## basic signals

- 00 nil opposite yes
- 01 yes opposite nil
- 02 iah i am here
- 03 stp stop

## transmission control

- 04 asc tree ascent
- 05 dsc tree descent
- 06 oka accepted okay transmission
- 07 bad rejected bad transmission

## escape sequences

- 08 ser state escape return  (resume previous escape sequence)
- 09 cse control state escape <esc...> <nil>
- 10 gse graphic state escape <esc...> <nil>
- 11 bdf binary data frame    <length> <data...>

## arbirtary device control codes

- 12 ac0 arbitrary control 0
- 13 ac1 arbitrary control 1
- 14 ac2 arbitrary control 2
- 15 ac3 arbitrary control 3

## modifier and erasure keys

- 16 mki mod key in  <key id>
- 17 mko mod key out <key id>
- 18 dlb delete backward (backspace)
- 19 dlf delete forward  (delete)

## utility keys

- 20 esc escape key
- 21 ins insert key
- 22 prt print screen key
- 23 brk pause break key

## character manipulation

- 24 cmp compose key
- 25 cmb combine character <one> <two>
- 26 scs set charset       <charset>
- 27 rcs revert charset

## whitespace characters

- 28 nmr next major row (page)
- 29 nmc next major column (tab)
- 30 nrw next row (newline)
- 31 ncl next column (space)

## numeric/symbolic printable characters

- 32 · (also corresponds to dot diacritic)
- 33 ° (also corresponds to circle diacritic)
- 34 .
- 35 ,
- 36 :
- 37 ;
- 38 !
- 39 ?
- 40 +
- 41 *
- 42 #
- 43 ¤ (also corresponds to $)
- 44 %
- 45 &
- 46 @
- 47 ^
- 48 0
- 49 1
- 50 2
- 51 3
- 52 4
- 53 5
- 54 6
- 55 7
- 56 8
- 57 9
- 58 (
- 59 )
- 60 >
- 61 /
- 62 `
- 63 -

## lowercase printable characters

- 64 a
- 65 b
- 66 c
- 67 d
- 68 e
- 69 f
- 70 g
- 71 h
- 72 i
- 73 j
- 74 k
- 75 l
- 76 m
- 77 n
- 78 o
- 79 p
- 80 q
- 81 r
- 82 s
- 83 t
- 84 u
- 85 v
- 86 w
- 87 x
- 88 y
- 89 z
- 90 [
- 91 ]
- 92 =
- 93 |
- 94 " (also corresponds to ¨)
- 95 _

## uppercase printable characters

- 096 A
- 097 B
- 098 C
- 099 D
- 100 E
- 101 F
- 102 G
- 103 H
- 104 I
- 105 J
- 106 K
- 107 L
- 108 M
- 109 N
- 110 O
- 111 P
- 112 Q
- 113 R
- 114 S
- 115 T
- 116 U
- 117 V
- 118 W
- 119 X
- 120 Y
- 121 Z
- 122 {
- 123 }
- 124 <
- 125 \
- 126 ' (also corresponds to ´)
- 127 ~
