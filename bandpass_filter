fp1=2000;

fp2=4000;

fs1=1500;

fs2=4500;

Fs=10000;

Wp1=2*pi*(fp1/Fs);

Ws1=2*pi*(fs1/Fs);

Wp2=2*pi*(fp2/Fs);

Ws2=2*pi*(fs2/Fs);

Ap=0.1;

As=50;

x=10^(-Ap/20);

y=10^(-As/20);

ds=y;

dp=1-x;

C=(-20*log10(sqrt(ds*dp))-13);

Q=14.6*(Ws2-Wp2)/(2*pi);

M=(C./Q)+1;

N=ceil(M-1);

Wca=Wp1/((10^(Ap/10)-1)^(0.5/N));

disp(Wca);

Wcb=Ws1/((10^(As/10)-1)^(0.5/N));

disp(Wcb);


Wn1=1.17;


Wcc=Wp2/((10^(Ap/10)-1)^(0.5/N));

disp(Wcc);

Wcd=Ws2/((10^(As/10)-1)^(0.5/N));

disp(Wcd);


Wn2=2.62;


f1=fir1(N,[Wn1/pi Wn2/pi],'bandpass');

freqz(f1,1,10000);
