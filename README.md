

% circular convolution of two sequences and verification of properties cle;

close all;

clear all;

x=input('enter the first sequence').

h=input('enter the second sequence') LI-length (x)

L2-length(h)

N= max(L1,L2) X=fft(x,N)

H=fft(h,N) Y-X. H

Z=ifft(Y,N) n = 1:1:length(Z)

stem(n,Z)

xlabel('n') ylabel('amplitude')

title('Circular convolution of two sequences").

% verification of commutative property x*h=h"a %

Ye H. X

Ze=ifft(Ye,N) if Z==Zc

disp('circular convolution is commutative")

end

