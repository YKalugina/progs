{\rtf1\ansi\ansicpg1252\cocoartf1404\cocoasubrtf470
{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
\margl1440\margr1440\vieww10800\viewh8400\viewkind0
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0

\f0\fs24 \cf0 There is an updated version of asympro.f that is free from overflow problems for large maxj values when dealing with small tau.  \
In order to get rid of the overflows due to factorials in wigner d-function (wigd), we have represented the factorial as a Gamma function which relates to the factorials as follows: G(n)=(n-1)! The Gamma function is defined in BSD library. The multiplication in factorials sections \'93pre1\'94 and \'93deform\'94 can be replaced by the summation if we take the logarithm of these values.  Then, to get back to \'93pre2=pre1/denorm\'94 used in calculation of wigd, we have to take the exponent of log(pre1/denorm). \
The resulting function gives the same answer as the one expressed in factorials but free from the overflow errors for large maxj values.\
  \
}