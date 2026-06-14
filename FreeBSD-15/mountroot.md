<img width="1024" height="768" alt="mountroot" src="https://github.com/user-attachments/assets/7c17261e-ee85-4a44-abbf-f18929847be4" />

# Kernel Config "TAPE3"
```
include GENERIC
ident TAPE3

device sa
```
root@bsd-1:/usr/src # make -j4 buildkernel KERNCONF=TAPE3 && make installkernel KERNCONF=TAPE3
