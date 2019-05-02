Assignement 1B responses are here

1. What are Channels and Kernels (according to EVA)?
**Answer 1:**: 
Channels:
They represent different characteristics of the image.
For example: An image is made of up different channels. Most popular is RGB and hence an image initially
to start with will have 3 channels and they represent pixel values.
Also, going further down through convolution layers, they represent edges and corners in the initial few convolutions.

Kernels:
Kernels can be referred to as filters. We may need filters to just detech  horizontal lines or just vertical lines.
These kernels which are usually 3X3 matirces multipy with the original image pixel values and detect the required edges / corners etc..


2. Why should we only (well mostly) use 3x3 Kernels?
**Answer 2:**: 
Most preferred kernels are of 3x3 in size. Reason being the  number of computations with 3x3 is very less when compared with other kernel
sizes.Also any filter size can be achieved with 3x3 filter. Two 3x3 filter in tandem results in a 5x5 filter. But the number of computations with one 5x5 filter will be much higher the computations done with two 3x3 filter. 


3. How many times do we need to perform 3x3 convolution operation to reach 1x1 from 199x199 (show calculations)

**Answer 3:**: 
imagesize | kernel      o/P
199 x 199 | 3x3   =      197x197 >>       
197 x 197 | 3x3   =      195x195 >>
195 x 195 | 3x3   =      193x193 >>
193 x 193 | 3x3   =      191x191 >>
191 x 191 | 3x3   =      189x189 >>
189 x 189 | 3x3   =      187x187 >>
187 x 187 | 3x3   =      185x185 >>
185 x 185 | 3x3   =      183x183 >>
183 x 183 | 3x3   =      181x181 >>
181 x 181 | 3x3   =      179x179 >>
179 x 179 | 3x3   =      177x177 >>
177 x 177 | 3x3   =      175x175 >>
175 x 175 | 3x3   =      173x173 >>
173 x 173 | 3x3   =      171x171 >>
171 x 171 | 3x3   =      169x169 >>
169 x 169 | 3x3   =      167x167 >>
167 x 167 | 3x3   =      165x165 >>
165 x 165 | 3x3   =      163x163 >>
163 x 163 | 3x3   =      161x161 >>
161 x 161 | 3x3   =      159x159 >>
159 x 159 | 3x3   =      157x157 >>
157 x 157 | 3x3   =      155x155 >>
155 x 155 | 3x3   =      153x153 >>
153 x 153 | 3x3   =      151x151 >>
151 x 151 | 3x3   =      149x149 >>
149 x 149 | 3x3   =      147x147 >>
147 x 147 | 3x3   =      145x145 >>
145 x 145 | 3x3   =      143x143 >>
143 x 143 | 3x3   =      141x141 >>
141 x 141 | 3x3   =      139x139 >>
139 x 139 | 3x3   =      137x137 >>
137 x 137 | 3x3   =      135x135 >>
135 x 135 | 3x3   =      133x133 >>
133 x 133 | 3x3   =      131x131 >>
131 x 131 | 3x3   =      129x129 >>
129 x 129 | 3x3   =      127x127 >>
127 x 127 | 3x3   =      125x125 >>
125 x 125 | 3x3   =      123x123 >>
123 x 123 | 3x3   =      121x121 >>
121 x 121 | 3x3   =      119x119 >>
119 x 119 | 3x3   =      117x117 >>
117 x 117 | 3x3   =      115x115 >>
115 x 115 | 3x3   =      113x113 >>
113 x 113 | 3x3   =      111x111 >>
111 x 111 | 3x3   =      109x109 >>
109 x 109 | 3x3   =      107x107 >>
107 x 107 | 3x3   =      105x105 >>
105 x 105 | 3x3   =      103x103 >>
103 x 103 | 3x3   =      101x101 >>
101 x 101 | 3x3   =       99x99  >>
99 x 199  | 3x3   =        97x97 >>       
97 x 97 | 3x3   =      95x95 >>
95 x 95 | 3x3   =      93x93 >>
93 x 93 | 3x3   =      91x91 >>
91 x 91 | 3x3   =      89x89 >>
89 x 89 | 3x3   =      87x87 >>
87 x 87 | 3x3   =      85x85 >>
85 x 85 | 3x3   =      83x83 >>
83 x 83 | 3x3   =      81x81 >>
81 x 81 | 3x3   =      79x79 >>
79 x 79 | 3x3   =      77x77 >>
77 x 77 | 3x3   =      75x75 >>
75 x 75 | 3x3   =      73x73 >>
73 x 73 | 3x3   =      71x71 >>
71 x 71 | 3x3   =      69x69 >>
69 x 69 | 3x3   =      67x67 >>
67 x 67 | 3x3   =      65x65 >>
65 x 65 | 3x3   =      63x63 >>
63 x 63 | 3x3   =      61x61 >>
61 x 61 | 3x3   =      59x59 >>
59 x 59 | 3x3   =      57x57 >>
57 x 57 | 3x3   =      55x55 >>
55 x 55 | 3x3   =      53x53 >>
53 x 53 | 3x3   =      51x51 >>
51 x 51 | 3x3   =      49x49 >>
49 x 49 | 3x3   =      47x47 >>
47 x 47 | 3x3   =      45x45 >>
45 x 45 | 3x3   =      43x43 >>
43 x 43 | 3x3   =      41x41 >>
41 x 41 | 3x3   =      39x39 >>
39 x 39 | 3x3   =      37x37 >>
37 x 37 | 3x3   =      35x35 >>
35 x 35 | 3x3   =      33x33 >>
33 x 33 | 3x3   =      31x31 >>
31 x 31 | 3x3   =      29x29 >>
29 x 29 | 3x3   =      27x27 >>
27 x 27 | 3x3   =      25x25 >>
25 x 25 | 3x3   =      23x23 >>
23 x 23 | 3x3   =      21x21 >>
21 x 21 | 3x3   =      19x19 >>
19 x 19 | 3x3   =      17x17 >>
17 x 17 | 3x3   =      15x15 >>
15 x 15 | 3x3   =      13x13 >>
13 x 13 | 3x3   =      11x11 >>
11 x 11 | 3x3   =      09x09 >>
09 x 09 | 3x3   =      07x07 >>
07 x 07 | 3x3   =      05x05 >>
05 x 05 | 3x3   =      03x03 >>
03 x 03 | 3x3   =      01x01 
