FizzBuzz Fortran 2008

gfortran-7 & intel fortran v.18

1: 75byte
print'(g0,t1a)',(i,'Fizz'(5**mod(i,3):)//'Buzz'(5**mod(i,5):),i=1,100);end

2: 76byte
do 1 i=1,100;1 print'(g0,t1,2a)',i,pack(['Fizz','Buzz'],0==mod(i,[3,5]));end

3: 77byte
print'(g0,t1a)',(i,'FizzBuzz'(5-4*2**mod(-i,3):4+4*2**mod(-i,5)),i=1,100);end


